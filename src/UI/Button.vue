<script>
export default {
	props: {
		text: String,
		color: String,
		bg: String,
	},
};
</script>

<template>
	<button :style="'background-color:' + bg + ';color:' + color" class="btn">
		{{ text }}
	</button>
</template>

<style scoped>
.btn {
	border-radius: 6px;
	border: none;

	padding: 10px 15px;
	font-family: "Inter";
	font-style: normal;
	font-weight: 500;
	font-size: 14px;
	line-height: 20px;
	text-align: center;
	font-feature-settings: "salt" on, "liga" off;
}
</style>
