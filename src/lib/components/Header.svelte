<script>
import Logo from "$lib/components/banners/Logo.svelte";
import LinkButton from "$lib/components/buttons/LinkButton.svelte";
import Button from "$lib/components/buttons/Button.svelte";

let tabs = [
    {text: "Home", link: "/"},
    {text: "About", link: "/about"},
    {text: "Services", link: "/services"},
    {text: "Works", link: "/works"},
    {text: "Blog", link: "/blog"},
];
</script>

<nav>
    <Logo/>
    <div class="nav-menu">
	{#each tabs as tab}
	    <LinkButton text={tab.text} link={tab.link}/>
	{/each}
    </div>
    <Button/>
</nav>

<style>
nav {
    position: sticky;
    top: 0;
    padding: 1rem var(--padding-desktop);
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    backdrop-filter: blur(5px);
    z-index: 999;
}
.nav-menu {
    padding: 4px 2px;
    background:#06081a;
    display: flex;
    flex-direction: row;
    text-transform: uppercase;
    border-radius: 9999px;
    box-shadow: 0 0 0 1px #292f65;
}
</style>
