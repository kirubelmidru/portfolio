<script>
import Logo from "$lib/components/banners/Logo.svelte";
import LinkButton from "$lib/components/buttons/LinkButton.svelte";
import Button from "$lib/components/buttons/Button.svelte";
import Hamburger from "$lib/components/buttons/Hamburger.svelte";

let tabs = [
    {text: "Home", link: "/"},
    {text: "About", link: "/about"},
    {text: "Services", link: "/services"},
    {text: "Works", link: "/works"},
    {text: "Blog", link: "/blog"},
];
</script>

<header>
    <div class="hamburger-button">
	<Hamburger/>
    </div>
    <Logo/>
    <div class="contact-button">
	<Button/>
    </div>
</header>

<style>
header {
    position: sticky;
    top: 0;
    padding: .5rem var(--padding-desktop);
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    backdrop-filter: blur(5px);
    z-index: 999;
}
.hamburger-button {
    position: absolute;
    top: 0;
    right: 0;
}
@media only screen and (max-width: 960px) {
    .contact-button {
	visibility: hidden;
    }
}
</style>
