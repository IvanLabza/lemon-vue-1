<template>
	.
</template>

<script>
export default {
	name: "AboutPage",
	data() {
		return {
			items: [
				{ id: 1, name: "Item 1.1" },
				{ id: 2, name: "Item 2.1" },
				{ id: 3, name: "Item 3.1" },
			],
			isVisible: true,
			isChecked: false,
		};
	},
	methods: {
		handleClick() {
			alert("Button clicked!");
		},
	},
};
</script>

<style lang="scss">
h1 {
	color: $red;
}
</style>