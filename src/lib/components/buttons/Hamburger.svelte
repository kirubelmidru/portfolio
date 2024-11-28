<script>
import { open } from "$lib/stores/stores.js";

$: enabled = $open;
</script>

<button on:click={()=>open.update((open) => !open)}>
    <div class:enabled class="hamburger-wrapper">
    <span></span>
    <span></span>
    <span></span>
    </div>
    {#if $open}
	<p>Close</p>
    {:else}
	<p>Menu</p>
    {/if}
</button>

<style>
button {
    padding: .5rem 0;
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 1rem;
}
button p {
    font-size: 14px;
    text-transform: uppercase;
    letter-spacing: .25em;
}
.hamburger-wrapper {
    width: 1.5rem;
    display: flex;
    flex-direction: column;
    gap: 4px;
}
.hamburger-wrapper span {
    height: 2px;
    background: white;
    transition: all .25s;
}
button:hover span:nth-child(1) {
    transform: translateY(3px);
}
button:hover span:nth-child(2) {
    opacity: 0;
}
button:hover span:nth-child(3) {
    transform: translateY(-3px);
}
.enabled span:nth-child(1) {
    transform: translateY(6px) rotate(45deg);
}
.enabled span:nth-child(2) {
    opacity: 0;
}
.enabled span:nth-child(3) {
    transform: translateY(-6px) rotate(-45deg);
}
@media only screen and (max-width: 960px) {
    button p {
	visibility: hidden;
    }
}
</style>
