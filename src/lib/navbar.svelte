<script>
    import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte'
  </script>
  
  <Navbar let:hidden let:toggle>
    <NavBrand href="/">
      <img
        src="https://www.geosphere.at/static/media/Logo.013b0f3d.svg"
        class="mr-3 h-6 sm:h-9"
        alt="GSA Logo"
      />
      <span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">
        Thesaurus
      </span>
    </NavBrand>
    <NavHamburger on:click={toggle} />
    <NavUl {hidden}>
      <NavLi href="/" active={true}>Home</NavLi>
      <NavLi href="/about">About</NavLi>
      <NavLi href="/services">Services</NavLi>
      <NavLi href="/pricing">Pricing</NavLi>
      <NavLi href="/contact">Contact</NavLi>
    </NavUl>
  </Navbar>