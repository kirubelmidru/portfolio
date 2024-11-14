<script>
import BlogPost from "$lib/components/articles/BlogPost.svelte";
</script>

<div class="blog-wrapper">
    <h2>My Personal Blog</h2>
    <div class="posts">
	<BlogPost/>
	<BlogPost/>
	<BlogPost/>
    </div>
</div>

<style>
.blog-wrapper {
    padding: 2rem;
}
h2 {
    padding: 8rem;
    font-size: 52px;
    text-align: center;
}
.posts {
    max-width: 1500px;
    margin-left: auto;
    margin-right: auto;
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
}
@media only screen and (max-width: 1500px) {
    .posts {
	max-width: 960px;
	grid-template-columns: repeat(2, minmax(0, 1fr));
    }
}
@media only screen and (max-width: 960px) {
    .blog-wrapper {
	padding: 0 1rem;
    }
    .posts {
	max-width: 540px;
	grid-template-columns: repeat(1, minmax(0, 1fr));
    }
}
</style>
