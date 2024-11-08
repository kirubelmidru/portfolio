<a href="/contact">
    <div class="btn-left">
	Let's Work Together
    </div>
    <div class="btn-right">
	<svg width="36px" height="36px" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
	    <path d="M16 12L8 12" stroke="black" stroke-width="1" stroke-linecap="sharp" stroke-linejoin="round"/>
	    <path d="M13 15L15.913 12.087V12.087C15.961 12.039 15.961 11.961 15.913 11.913V11.913L13 9" stroke="black" stroke-width="1" stroke-linecap="sharp" stroke-linejoin="sharp"/>
	</svg>
    </div>
</a>

<style>
a {
    display: flex;
    flex-direction: row;
    transition: all .5s;
}
.btn-left {
    padding: 1.5rem;
    display: flex;
    align-items: center;
    background: var(--accent-color);
    border-bottom-left-radius: 9999px;
    border-top-left-radius: 9999px;
    transition: all .5s;
    transform: translateX(1%);
}
a:hover .btn-left {
    border-bottom-right-radius: 9999px;
    border-top-right-radius: 9999px;
    transform: translateX(-10%);
}
.btn-right {
    padding: .5rem 1rem;
    display: flex;
    align-items: center;
    background: var(--accent-color);
    border-bottom-right-radius: 9999px;
    border-top-right-radius: 9999px;
    transition: all .5s;
}
a:hover .btn-right {
    border-bottom-left-radius: 9999px;
    border-top-left-radius: 9999px;
    transform: translateX(-10%);
}
.btn-right svg {
    transition: transform .5s;
}
a:hover svg {
    transform: rotate(-45deg);
}
</style>
