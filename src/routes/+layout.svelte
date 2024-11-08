<script>
import Header from "$lib/components/Header.svelte";
import Footer from "$lib/components/Footer.svelte";
import "../app.css";
</script>

<div class="wrapper">
    <Header/>
    <main>
	<slot/>
    </main>
    <Footer/>
</div>

<style>
.wrapper {
    background-image: var(--bg-pattern);
}
</style>
