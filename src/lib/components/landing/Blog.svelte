<script>
import BlogPost from "$lib/components/articles/BlogPost.svelte";
</script>

<div class="blog-wrapper">
    <h2>Blog</h2>
    <div class="posts">
	<BlogPost/>
	<BlogPost/>
	<BlogPost/>
    </div>
</div>

<style>
.blog-wrapper {
    padding: 4rem;
    display: flex;
    flex-direction: column;
    gap: 8rem;
}
h2 {
    font-size: 64px;
    text-align: center;
}
.posts {
    padding: 0 8rem;
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 2rem;
}
</style>
