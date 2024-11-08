<button>
    <div class="hamburger">
	<span/>
	<span/>
	<span/>
    </div>
    <p style="font-size: 20px;">MENU</p>
</button>

<style>
button {
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: .5rem;
    background: transparent;
}
button:hover span{
    background: red;
}
button:hover p {
    color: red;
}
.hamburger {
    width: 2rem;
    display: flex;
    flex-direction: column;
    gap: 4px;
}
.hamburger span {
    height: 2px;
    background: black;
}
</style>
