<script>
export default {
	components: {},

	methods: {
		getImgUrl(index) {
			return require("./../assets/" + index + ".png");
		},
	},
};
</script>

<template>
	<div class="container">
		<div class="client">
			<h3 class="section-title">Our Clients</h3>
			<p class="section-text">
				We have been working with some Fortune 500+ clients
			</p>
			<ul>
				<li v-for="index in 7">
					<img :src="'./../assets/' + index + '.png'" v-bind:alt="index" />
					<img src="./../assets/5.png" />
					<!-- './../assets/' + index + '.png' -->
				</li>
			</ul>
		</div>
	</div>
</template>

<style lang="scss" scoped>
.client {
	text-align: center;
	padding: 20px;
	.section-title {
		font-family: "Inter";
		font-style: normal;
		font-weight: 600;
		font-size: 36px;
		line-height: 44px;
		text-align: center;
		color: #4d4d4d;
	}

	.section-text {
		font-family: "Inter";
		font-style: normal;
		font-weight: 400;
		font-size: 16px;
		line-height: 24px;
		text-align: center;
		color: #717171;
		padding: 20px 0;
	}

	ul {
		display: flex;
		text-align: center;
		align-items: center;
		justify-content: space-evenly;
		li {
			list-style-type: none;
			padding: 10px;

			img {
				background: #000;
			}
		}
	}
}
</style>
