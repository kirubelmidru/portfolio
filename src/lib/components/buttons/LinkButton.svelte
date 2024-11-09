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
    padding: 12px 24px;
    border-radius: 9999px;
    color: white;
    overflow: hidden;
    transition: transform 1s;
    transform: scale(100%); 
}
a:hover {
    transform: scale(85%);
}
a::before {
    display: block;
    position: absolute;
    content: "";
    padding: 6rem;
    background: #0000ff;
    border-radius: 9999px;
    transition: transform 1s, opacity 1s;
    transform: scale(0);
    opacity: 100%;
}
a:hover::before {
    transform: scale(1);
    opacity: 20%;
}
</style>
