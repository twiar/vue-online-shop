<template>
	<div class="v-main-wrapper">
		<p>{{ title }}</p>
		<v-catalog />
		<v-cart />
	</div>
</template>

<script>
import vCart from "./v-cart";
import vCatalog from "./v-catalog";

export default {
	name: "v-main-wrapper",
	components: {
		vCatalog,
		vCart,
	},
	props: {},
	data() {
		return {
			title: "Main wrapper",
		};
	},
	computed: {},
	methods: {},
	watch: {},
	mounted() {
		console.log("Hello i am alive!");
	},
};
</script>

<style scoped>
.v-main-wrapper {
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	max-width: 900px;
	margin: 0 auto;
}
</style>
