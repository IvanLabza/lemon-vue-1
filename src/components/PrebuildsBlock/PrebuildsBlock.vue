<template>
    <div class="prebuild">
        <div class="prebuild__info">
            <div class="prebuild__title">Think CI/CD for dev environments</div>
            <div class="prebuild__desc">
                We invented prebuilds so application code, configuration and
                infrastructure can all be stored as machine-executable code in your git
                repositories and applied to dev environments automatically and
                continuously.
            </div>
            <div class="prebuild-btn">
                <a href="/" class=" btn prebuild-btn__first">
                    More on prebuilds
                </a>
                <a href="/" class="btn prebuild-btn__second">
                    Documentation
                </a>
            </div>
        </div>
        <div class="prebuild__img">
            <img src="@/assets/code1.png" alt="code one">
        </div>
    </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
@import '@/components/PrebuildsBlock/PrebuildsBlock.scss';
</style>
