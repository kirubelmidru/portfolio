<script>
import SideButton from "$lib/components/buttons/SideButton.svelte";

let tabs = [
    {text: "About", link: "/about"},
    {text: "Services", link: "/services"},
    {text: "Works", link: "/works"},
    {text: "Blog", link: "/blog"},
];
</script>

<div class="sidebar-wrapper">
    {#each tabs as tab}
	<SideButton text={tab.text} link={tab.link}/>
    {/each}
</div>

<style>
.sidebar-wrapper {
    position: fixed;
    top: 0;
    left: 0;
    height: 100vh;
    width: 100vw;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background-color: #0f6efc;
    z-index: 50;
}
</style>
