<script>
import Logo from "$lib/components/misc/Logo.svelte";
import Hamburger from "$lib/components/buttons/Hamburger.svelte";
import LinkButton from "$lib/components/buttons/LinkButton.svelte";
import Sidebar from "$lib/components/navbar/Sidebar.svelte";

import { open } from "$lib/stores/stores.js";
$: enabled = $open;
</script>

<header class:enabled>
    <div class="header-wrapper">
	<Hamburger/>
	<a href="/">
	    <Logo/>
	</a>
	<LinkButton text="Get Started" link="/contact"/>
    </div>
</header>

{#if $open}
<Sidebar/>
{/if}

<style>
header {
    position: sticky;
    top: 0;
    background: var(--background-color);
    z-index: 99;
}
.header-wrapper {
    max-width: var(--max-width);
    margin: 0 auto;
    padding: 1.5rem;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
}
.enabled {
    background: #0f6efc;
}
</style>
