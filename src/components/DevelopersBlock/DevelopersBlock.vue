<template>
  <div class="developers developers_container">
    <div class="developers__title">Used by 400,000+ developers.</div>

    <div class="developers__card">
      <SwiperBlock />
    </div>
    <div class="developers-company">
      <div class="developers-company__row">
        <img src="@/assets/company/Frame.png" alt="" class="developers-company__img">
        <img src="@/assets/company/codecamp.png" alt="" class="developers-company__img">
        <img src="@/assets/company/wave.png" alt="" class="developers-company__img">
        <img src="@/assets/company/google.png" alt="" class="developers-company__img">
        <img src="@/assets/company/amazon.png" alt="" class="developers-company__img">
        <img src="@/assets/company/facebook.png" alt="" class="developers-company__img">
        <img src="@/assets/company/uber.png" alt="" class="developers-company__img">
      </div>
      <div class="developers-company__rowtwo">
        <img src="@/assets/company/openai.png" alt="" class="developers-company__img">
        <img src="@/assets/company/intel.png" alt="" class="developers-company__img">
        <img src="@/assets/company/theia.png" alt="" class="developers-company__img">
        <img src="@/assets/company/code.png" alt="" class="developers-company__img">
        <img src="@/assets/company/4geeks.png" alt="" class="developers-company__img">
      </div>
    </div>
  </div>
</template>

<script>
import SwiperBlock from '@/components/SwiperBlock/SwiperBlock.vue'

export default {
  components: {
    SwiperBlock,
  },

};


</script>

<style lang="scss">
@import '@/components/DevelopersBlock/DevelopersBlock.scss';
</style>
