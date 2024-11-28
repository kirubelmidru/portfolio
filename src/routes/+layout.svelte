<script>
import Header from "$lib/components/navbar/Header.svelte";
import Footer from "$lib/components/Footer.svelte";
import "../app.css";
</script>

<Header/>
<main>
    <slot/>
</main>
<Footer/>
