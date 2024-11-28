<script>
export let title;
export let date;
</script>

<a>
    <img class="post-image" src="../first.jpg"/>
    <p class="tag">Erlang</p>
    <h3>{title}</h3>
    <svg width="44" height="18" viewBox="0 0 44 18" fill="none" xmlns="http://www.w3.org/2000/svg">
	<path d="M3.45612 9.76992L3.45612 7.82811L38.3367 7.82655L32.3726 1.86242L33.7596 0.475415L42.0816 8.79745L33.7596 17.1195L32.3726 15.7325L38.3367 9.76836L3.45612 9.76992Z" fill="#0f6efc"/>
    </svg>
</a>

<style>
a {
    padding: 2rem 0;
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
    overflow: hidden;
    transition: gap .5s;
}
img {
    height: 32rem;
    object-fit: cover;
}
p {
    color: #0f6efc;
    text-transform: uppercase;
    letter-spacing: .2em;
}
h3 {
    font-size: 28px;
    text-transform: uppercase;
}
svg {
    transform: translateX(-20px);
    transition: transform .5s;
}
a:hover {
    gap: 1rem;
}
a:hover h3 {
    color: #0f6efc;
}
a:hover svg {
    transform: translateX(0);
}
</style>
