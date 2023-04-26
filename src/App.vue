<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import OurClients from "./components/OurClients.vue";
import Footer from "./components/Footer.vue";
import Card from "./UI/Card.vue";
import { arr } from "./db/user";

export default {
	data() {
		return {
			number: 0,
		};
	},
	components: {
		Header,
		Main,
		OurClients,
	},
};
</script>

<template>
	<Header />
	<Main />
	<OurClients />
</template>

<style lang="scss" scoped></style>
