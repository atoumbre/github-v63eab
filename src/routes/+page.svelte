<script lang="ts">
    import { Alert } from 'flowbite-svelte';
    import { Navbar, NavBrand, NavHamburger, NavUl, NavLi, Avatar, Chevron, MegaMenu,DarkMode,
    Card, Button, Toggle,ImagePlaceholder,Hr  } from 'flowbite-svelte'
</script>

<Navbar let:hidden let:toggle>
  <!-- <NavBrand href="/">
    <img src="https://flowbite.com/docs/images/logo.svg" class="mr-3 h-6 sm:h-9" alt="Flowbite Logo"/>
    <span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">Flowbite</span>
  </NavBrand> -->
  <NavHamburger on:click={toggle} />
  <NavUl {hidden}>
    <NavLi href="/services">Services</NavLi>
    <NavLi href="/services">Products</NavLi>
    <NavLi href="/services">Contact</NavLi>
 

  </NavUl>

   <DarkMode/>


</Navbar>


<div>

    <Card>

        <ImagePlaceholder  />

        <Hr/>

        <h5 class="pt-5 mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy technology acquisitions 2021</h5>
        <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">
        Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.
        </p>

        <Button >
        Read more <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5 ml-2"><path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5L21 12m0 0l-7.5 7.5M21 12H3" /></svg>
        </Button>

    </Card>

    <Avatar class="absolute" />

</div>
