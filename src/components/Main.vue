<script>
import Section from "./Section.vue";
import Button from "./../UI/Button.vue";

export default {
	components: {
		Section,
		Button,
	},
};
</script>

<template>
	<div class="container">
		<main>
			<div class="main-left">
				<h2 class="big-main-text">
					Lessons and insights <span>from 8 years</span>
				</h2>
				<p>
					Where to grow your business as a photographer: site or social media?
				</p>
				<Button text="Register" color="white" bg="#4CAF4F" />
			</div>
			<div class="main-right">
				<img src="../assets/img.png" alt="" />
			</div>
		</main>
	</div>
</template>

<style lang="scss" scoped>
main {
	min-height: calc(100vh - 70px - 70px);
	display: flex;
	justify-content: center;
	align-items: center;
	padding: 20px;
	.main-right {
		text-align: center;
		width: 40%;

		img {
			height: 100%;
			width: 100%;
		}
	}

	.main-left {
		text-align: start;
		width: 60%;

		.big-main-text {
			font-family: "Inter";
			font-style: normal;
			font-weight: 600;
			font-size: 64px;
			line-height: 76px;
			color: #4d4d4d;

			span {
				color: #4caf4f;
			}
		}

		p {
			padding: 25px 0;
			font-family: "Inter";
			font-style: normal;
			font-weight: 400;
			font-size: 16px;
			line-height: 24px;
			color: #717171;
		}
	}
}
</style>
