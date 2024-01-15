<template>
	<div class="header">
		<router-link to="/" class="header__logo">
			<img src="@/assets/logo.svg" alt="gitpod" />
		</router-link>
		<div class="header__nav" :class="{ 'is-active': isActive }" @click="isActive = false">
			<router-link to="/">Features</router-link>
			<router-link to="/">Pricing</router-link>
			<router-link to="/">Blog</router-link>
			<router-link to="/">Docs</router-link>
			<router-link to="/">Changelog</router-link>
			<router-link to="/">We're hiring</router-link>
			<div class="header__close" @click="isActive = false"><CloseIcon /></div>
		</div>
		<div class="header__burger" v-if="!isActive" @click="isActive = !isActive">
			<MenuIcon />
		</div>
		<div class="header__btn">
			<router-link to="/">Login</router-link>
		</div>
	</div>
</template>

<script>
import MenuIcon from "vue-material-design-icons/Menu.vue";
import CloseIcon from "vue-material-design-icons/Close.vue";
export default {
	name: "HeaderBlock",
	data() {
		return {
			isActive: false,
		};
	},
	components: {
		MenuIcon,
		CloseIcon,
	},
};
</script>

<style lang="scss" scoped>
@import '@/components/HeaderBlock/HeaderBlock.scss';
</style>
