<script>
export let text;
export let link;
</script>

<a href={link}>
    <svg width="12" height="12" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
	<path d="M1.29231 13.5433L1.29231 10.9587H19.0154L11.0769 3.02021L12.9231 1.17405L24 12.251L12.9231 23.3279L11.0769 21.4817L19.0154 13.5433L1.29231 13.5433Z" fill="white"/>
    </svg>
    {text}
</a>

<style>
a {
    padding: .5rem 0;
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 1rem;
    font-size: 14px;
    text-transform: uppercase;
    letter-spacing: .25em;
}
a svg {
    transition: transform .25s;
    transform: rotate(-45deg);
}
a:hover svg{
    transform: rotate(0deg);
}
</style>
