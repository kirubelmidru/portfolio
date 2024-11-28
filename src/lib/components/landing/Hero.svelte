<script>
import LandingPost from "$lib/components/articles/LandingPost.svelte";
import Button from "$lib/components/buttons/Button.svelte";

let landings = [
    {
	title: "Works", 
	subtitle: "What I've Done So Far", 
	content: "NJI partners with ambitious organizations. We excel at disrupting the status quo of public affairs marketing and communications. We’re local, from Capitol Hill to Westminster and far beyond. We understand how innovative design moves markets and changes minds. Fancy an invite?",
	button: "Explore Work",
    },
    {
	title: "Services", 
	subtitle: "What I Can Provide", 
	content: "",
	button: "View Story",

    },
    {
	title: "Clients", 
	subtitle: "Notable Mentions", 
	content: "",
	button: "Read about Me",
    },
];
</script>

<div class="landing">
    <div class="hero-wrapper">
	<h2 class="hero-text">Let's Create Your Wildest Dreams</h2>
	{#each landings as landing}
	    <LandingPost title={landing.title} subtitle={landing.subtitle}>
		<p style="font-size: 18px;">{landing.content}</p>
		<Button content={landing.button}/>
	    </LandingPost>
	{/each}
    </div>
</div>

<style>
.landing {
    max-width: var(--max-width);
    margin: 0 auto;
    padding: var(--padding);
}
.hero-wrapper {
    display: flex;
    flex-direction: column;
    gap: 2rem;
}
.hero-text {
    font-size: 64px;
    font-weight: 700;
    text-align:center;
    text-transform: uppercase;
}
svg {
    transform: translateX(920px) translateY(-90px);
}
</style>
