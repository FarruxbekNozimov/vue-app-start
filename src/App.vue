<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";
import Card from "./UI/Card.vue";
import { arr } from "./db/user";

export default {
	data() {
		return {
			number: 0,
			array: arr,
		};
	},
	components: {
		Header,
		Main,
		Footer,
	},

	methods: {
		info() {
			console.log(arr);
		},
	},
};
</script>

<template>
	<Header />
	<main>
		<div class="wrapper">
			<Card v-for="(el, index) in this.array" :data="el" :key="el.id" />
		</div>
	</main>
	<Footer />
</template>

<style lang="scss" scoped>
main {
	min-height: 100vh;

	.wrapper {
		display: flex;
		gap: 50px;
		justify-content: center;
		padding-top: 5px;
	}
	.card {
		width: 240px;
		box-shadow: 10px 10px 10px silver;
		.card-body {
			border-radius: 10px;
			padding: 10px;
			background: #9999998e;
			border: 1px solid black;
		}
		.card-img {
			border: 1px solid black;
			border-radius: 10px;
		}
	}
}
</style>
