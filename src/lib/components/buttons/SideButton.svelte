<script>
export let text;
export let link;
</script>

<a href={link}>
    {text}
</a>

<style>
a {
    font-size: 96px;
    font-weight: 700;
    text-transform: uppercase;
}
@media only screen and (max-width: 960px) {
    a {
	font-size: 48px;
    }
}
</style>
