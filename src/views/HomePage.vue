<template>
	<div class="container">
		<HeaderBlock />
	</div>
</template>

<script>
import HeaderBlock from "@/components/HeaderBlock/HeaderBlock.vue";

export default {
	name: "HomePage",
	data() {
		return {
			isChecked: false,
		};
	},
	methods: {},
	components: { HeaderBlock },
};
</script>
