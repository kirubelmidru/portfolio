<script>
import Button from "$lib/components/buttons/Button.svelte";
</script>

<footer>
    <div class="contact-wrapper">
	<p style="font-size: 48px; color: white;"> Impressed By What You See?</p>
	<Button/>
    </div>
</footer>

<style>
footer {
    background: var(--secondary-color);
}
.contact-wrapper {
    text-align: center;
    padding: 2rem;
    background: #080808;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 2rem;
}
</style>
