<script>
export default {
	props: {
		data: Object,
	},
};
</script>

<template>
	<div v-for="el in this.array" class="card">
		<img
			:src="'https://picsum.photos/id/12' + el.id + '/240/200'"
			alt="img"
			class="card-img" />
		<div class="card-body">
			<h3 class="card-title">{{ el.title }}</h3>
			<p class="card-text">
				Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ratione
				voluptatum aliquam laudantium, ullam blanditiis in, sed repellendus
				nesciunt non facilis ex delectus reiciendis sit. Pariatur ut id aut
				labore! Molestias!
			</p>
		</div>
	</div>
</template>

<style lang="scss" scoped>
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
</style>
