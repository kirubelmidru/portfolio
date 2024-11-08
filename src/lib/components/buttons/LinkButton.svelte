<script>
export let text;
export let link;
</script>

<a href={link}>
    {text}
</a>

<style>
a {
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 1rem 2rem;
    border-radius: 9999px;
    color: white;
    overflow: hidden;
    transition: transform 1s, background 1s;
    background: transparent;
    transform: scale(100%); 
}
a:hover {
    background: #000099;
    opacity: 80%;
    transform: scale(85%);
}
a::before {
    display: block;
    position: absolute;
    content: "";
    padding: 6rem;
    background: #0000ff;
    border-radius: 9999px;
    transition: transform 1.5s, opacity 1s;
    transform: scale(0);
    opacity: 50%;
}
a:hover::before {
    transform: scale(1);
    opacity: 0%;
}
</style>
