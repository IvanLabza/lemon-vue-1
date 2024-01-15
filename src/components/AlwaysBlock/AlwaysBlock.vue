<template>
  <div class="always">
    <div class="always__info">
      <div class="always__title">Always <br />Ready to Code.</div>
      <div class="always__desc">
        Spin up fresh, automated dev environments for each task, in the cloud,
        in seconds.
      </div>
      <div class="always-link">
        <div class="always-link__components">
          <a href="/" class="always-link__btn">Try Now</a>
          <div class="always-link__desc">
            Open a workspace. <br />Start from any Git context.
          </div>
        </div>

        <div class="always-link__icon">
          <a href="/">
            <img src="@/assets/icons/gitlab.svg" alt="gitlab" />
          </a>
          <a href="/">
            <img src="@/assets/icons/git.svg" alt="git" />
          </a>
          <a href="/">
            <img src="@/assets/icons/bitbucket.svg" alt="bitbucket" />
          </a>
        </div>
      </div>
    </div>
    <div class="always__img">
      <img src="@/assets/workplace.png" alt="workplace" />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
@import "@/components/AlwaysBlock/AlwaysBlock.scss";
</style>