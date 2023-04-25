<script>
import Button from "./../UI/Button.vue";

export default {
	components: {
		Button,
	},
};
</script>

<template>
	<header>
		<div class="container">
			<nav>
				<a href="#" class="logo"><img src="./../assets/logo.png" alt="" /></a>
				<ul class="nav__list">
					<li class="nav__list-item">Home</li>
					<li class="nav__list-item">Featrue</li>
					<li class="nav__list-item">Product</li>
					<li class="nav__list-item">Testimonial</li>
					<li class="nav__list-item">FAQ</li>
				</ul>
				<div class="btns">
					<Button text="Login" color="#4CAF4F" bg="white" />
					<Button text="Sign up" color="white" bg="#4CAF4F" />
				</div>
			</nav>
		</div>
	</header>
</template>

<style lang="scss" scoped>
header {
	nav {
		height: 80px;
		display: flex;
		justify-content: space-between;
		align-items: center;

		.nav__list {
			display: flex;
			width: 50%;
			justify-content: space-around;
		}

		.nav__list-item {
			list-style-type: none;
			font-family: "Inter";
			font-style: normal;
			font-weight: 400;
			font-size: 16px;
			line-height: 24px;
			color: #18191f;
		}
		.btns {
			display: flex;
			gap: 10px;
		}
	}
}
</style>
