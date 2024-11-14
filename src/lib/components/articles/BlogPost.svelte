<script>
export let title;
export let date;
</script>

<a>
    <div class="tags">
	<p>7 feb 2025</p>
	<p>Blog</p>
    </div>
    <img class="post-image" src="../first.png"/>
    <h3>Exploring Functional Programming: My Experience With Erlang</h3>
</a>

<style>
a {
    display: flex;
    flex-direction: column;
    border-radius: 1rem;
    overflow: hidden;
}
h3 {
    background: #080808;
    padding: 1rem;
    z-index: 1;
}
.post-image {
    height: 18rem;
    z-index: 0;
    transition: transform 1s, filter 1s;
    filter: grayscale(100%);
}
a:hover .post-image {
    filter: grayscale(0%);
    transform: scale(1.2);
}
.tags {
    position: absolute;
    padding: 1rem;
    display: flex;
    flex-direction: row;
    gap: .5rem;
    z-index: 1;
}
.tags p {
    padding: 6px 12px;
    background: #171717;
    border-radius: 4px;
    font-size: 10px;
    text-transform: uppercase;
}
</style>
