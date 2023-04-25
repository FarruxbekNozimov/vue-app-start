<script>
export default {
	props: {
		text: {
			type: String,
			required: true,
		},
		color: String,
	},
};
</script>

<template>
	<section class="intro" :style="'background-color:' + color">
		<div class="container">
			<div class="text-center">{{ text }}</div>
		</div>
	</section>
</template>

<style lang="scss" scoped>
.intro {
	min-height: 80vh;
	// background-color: coral;
	display: flex;
	justify-content: center;
	align-items: center;
	.text-center {
		text-align: center;
		font-weight: bold;
		font-size: 30px;
	}
}
</style>
