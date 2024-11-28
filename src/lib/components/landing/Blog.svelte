<script>
import BlogPost from "$lib/components/articles/BlogPost.svelte";
</script>

<div class="blog-wrapper">
    <h2>Blog</h2>
    <div class="posts">
	<BlogPost/>
	<BlogPost/>
	<BlogPost/>
	<BlogPost/>
	<BlogPost/>
	<BlogPost/>
    </div>
</div>

<style>
.blog-wrapper {
    max-width: 1240px;
    margin: 0 auto;
    padding: var(--padding);
}
h2 {
    padding: 4rem 0;
    font-size: 52px;
    text-align: center;
    text-transform: uppercase;
}
.posts {
    max-width: 1240px;
    margin: 0 auto;
    padding: 1rem;
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 2rem;
}
@media only screen and (max-width: 1500px) {
    .posts {
	max-width: 960px;
	grid-template-columns: repeat(2, minmax(0, 1fr));
    }
}
@media only screen and (max-width: 960px) {
    .posts {
	max-width: 540px;
	grid-template-columns: repeat(1, minmax(0, 1fr));
    }
}
</style>
