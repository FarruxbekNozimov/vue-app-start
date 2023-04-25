<script>
export default {};
</script>

<template>
	<header>
		<div class="container">
			<nav><a href="#" class="logo">LOGO</a></nav>
		</div>
	</header>
</template>

<style lang="scss" scoped>
header {
	background-color: rgb(0, 255, 0);
	margin: 10px;
	border-radius: 50px;
	padding: 0 15px;

	nav {
		height: 70px;
		display: flex;
		justify-content: space-between;
		align-items: center;

		.logo {
			font-weight: bold;
			font-size: 25px;
			font-family: sans-serif;
			text-decoration: none;
			color: #000;
		}
	}
}
</style>
