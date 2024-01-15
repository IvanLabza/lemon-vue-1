<template>
	<div class="container">
		<HeaderBlock />
		<AlwaysBlock />
		<CrossedBlock />
		<PrebuildsBlock />
		<DesignBlock />
		<DevelopersBlock />
		<StartedBlock />
	</div>
	<FooterBlock />
</template>

<script>
import HeaderBlock from "@/components/HeaderBlock/HeaderBlock.vue";
import AlwaysBlock from "@/components/AlwaysBlock/AlwaysBlock.vue";
import CrossedBlock from "@/components/СrossedBlock/СrossedBlock.vue";
import PrebuildsBlock from "@/components/PrebuildsBlock/PrebuildsBlock.vue";
import DesignBlock from "@/components/DesignBlock/DesignBlock.vue";
import DevelopersBlock from "@/components/DevelopersBlock/DevelopersBlock.vue";
import StartedBlock from "@/components/StartedBlock/StartedBlock.vue";
import FooterBlock from "@/components/FooterBlock/FooterBlock.vue";

export default {
	name: "HomePage",
	data() {
		return {
			isChecked: false,
		};
	},
	methods: {},
	components: { HeaderBlock, AlwaysBlock, CrossedBlock, PrebuildsBlock, DesignBlock, DevelopersBlock, StartedBlock, FooterBlock },
};
</script>
