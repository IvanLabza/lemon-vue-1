<template>
	<h1>vIf</h1>
	<p v-if="isVisible">This paragraph is visible.</p>
	<h1>vModel</h1>
	<input type="checkbox" v-model="isChecked" />
	<p>{{ isChecked ? "Checked" : "Not Checked" }}</p>

	<h1>vFor</h1>
	<ul>
		<li v-for="item in items" :key="item.id">{{ item.name }}</li>
	</ul>
	<h1>@click</h1>
	<button @click="handleClick">Click me</button>
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
