<script>
export let title;
export let subtitle;
</script>
<div class="landing-post">
    <div class="sub-landing">
    <h2>{title}</h2>
    <h3>{subtitle}</h3>
    </div>
    <slot/>
</div>

<style>
.landing-post {
    max-width: 720px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    gap: 2rem;
    text-align: center;
}
.landing-post h2 {
    font-size: 14px;
    text-transform: uppercase;
    letter-spacing: .25em;

}
.landing-post h3 {
    font-size: 64px; 
}
</style>
