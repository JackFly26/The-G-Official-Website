<style>
	img {
		width: 100%;
		align-self: center;
	}
	div.img-container {
		max-height: 20%;
		overflow: hidden;
		display: flex;
	}
	div.navbar {
		background: rgb(100, 0, 0);
		display: flex;
		height: 3rem;
		align-items: stretch;
		justify-content: space-around;
		position: sticky;
		top: 0;
		font-family: 'Teko';
	}
</style>
<script>
	import NavItem from './NavItem.svelte'
	export let setPage
</script>
<div class="img-container"><img src="assets/logo.png" alt="Logo"></div>
<div class="navbar">
	<NavItem text="Home" {setPage}/>
	<NavItem text="About Us" {setPage}/>
	<NavItem text="Our Music" {setPage}/>
	<NavItem text="Contact" {setPage}/>
</div>
