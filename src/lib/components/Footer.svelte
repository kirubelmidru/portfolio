<script>
import LinkButton from "$lib/components/buttons/LinkButton.svelte";
let tabs = [
    {text: "About", link: "/about"},
    {text: "Services", link: "/services"},
    {text: "Works", link: "/works"},
    {text: "Blog", link: "/blog"},
];
</script>

<footer>
    <div class="footer-wrapper">
	<div class="">

	</div>
	<div class="roadmap">
	    <h2>RoadMap</h2>
	    {#each tabs as tab}
		<LinkButton text={tab.text} link={tab.link}/>
	    {/each}
	</div>
    </div>
</footer>

<style>
footer {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    background: #0f6efc;
}
.footer-wrapper {
    max-width: var(--max-width);
    margin: 0 auto;
    padding: var(--padding);
}
.footer-wrapper h2 {
    font-size: 48px;
    text-transform: uppercase;
}
</style>
