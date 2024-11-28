<script>
import LinkButton from "$lib/components/buttons/LinkButton.svelte";
</script>

<div class="error-wrapper">
    <h2>404 | Page Not Found</h2>
    <p>The Page You Requested is Currently On Vacation.</p>
    <LinkButton text="Go Home" link="/"/>
</div>

<style>
.error-wrapper {
    max-width: var(--max-width);
    margin: 0 auto;
    padding: var(--padding);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 2rem;
    text-align: center;
}
.error-wrapper h2 {
    font-size: 16px;
    text-transform: uppercase;
    letter-spacing: .25em;
}
.error-wrapper p {
    font-size: 48px;
}
</style>
