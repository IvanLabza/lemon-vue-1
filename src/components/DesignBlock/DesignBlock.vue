<template>
  <div class="design">
    <div class="design__title">Remote-first. Secure by design.</div>
    <div class="design__img">
      <img src="@/assets/code2.png" alt="code two" />
    </div>
    <div class="design__desc">
      You no longer need an over-powered laptop to code, Gitpod works just as
      smoothly on a Chromebook or iPad. All you need is a browser. Gitpod
      centralizes all source code and never stores it on insecure machines and
      networks.
    </div>
    <div class="design-btn">
      <div class="design-btn__bg">
        <a href="/" class="design-btn__chrome"
          ><img src="@/assets/icons/gchrome.svg" alt="Chrome" />Chrome
          Extension</a
        >
      </div>
      <div class="design-btn__bg">
        <a href="/" class="design-btn__firefox"
          ><img src="@/assets/icons/firefox.svg" alt="Firefox" />Firefox
          Extension</a
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
@import '@/components/DesignBlock/DesignBlock.scss';
</style>
