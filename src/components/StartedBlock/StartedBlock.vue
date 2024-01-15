<template>
  <div class="started">
    <div class="started__title">Get started now</div>
    <div class="started__content">
      <div class="started-connect">
        <div class="started-connect__title">Connect Git repository</div>
        <div class="started-connect__desc">
          Select a Git provider to start with an existing project from any Git
          context.
        </div>
        <div class="started-connect__buttons">
          <a href="/" class="started-connect__btn first"
            ><img src="@/assets/icons/repos/gitla.svg" alt="gitlab" />Continue
            with GitLab</a
          >
          <a href="/" class="started-connect__btn second"
            ><img src="@/assets/icons/repos/github1.svg" alt="" />Continue with
            GitHub</a
          >
          <a href="/" class="started-connect__btn third"
            ><img src="@/assets/icons/repos/blue.svg" alt="" />Continue with
            Bitbucket</a
          >
        </div>
        <div class="started__desc">
          Or prefix any GitLab, GitHub or Bitbucket URL with
        </div>
        <div class="started__gitpod">gitpod.io/#</div>
      </div>
      <div class="started-launch">
        <div class="started-launch__title">Launch an example workspace</div>
        <div class="started-launch__desc">
          Dive into one of our example workspaces
        </div>
        <div class="started-launch__languages">
          <div class="started-launch__language">
            <input type="text" readonly class="started-launch__field" />
            <div class="started-launch__wrapper">
              <div class="started-launch__icon">
                <img
                  src="@/assets/icons/lang/TypeScript.svg"
                  alt="Programming Language 1" />
                <span>Node or TypeScript</span>
              </div>
            </div>
            <button class="started-launch__button">Launch workspace</button>
          </div>
          <div class="started-launch__language">
            <input type="text" readonly class="started-launch__field" />
            <div class="started-launch__wrapper">
              <div class="started-launch__icon">
                <img src="@/assets/icons/lang/Python.svg" alt="Python" />
                <span>Python</span>
              </div>
            </div>
            <button class="started-launch__button">Launch workspace</button>
          </div>
          <div class="started-launch__language">
            <input type="text" readonly class="started-launch__field" />
            <div class="started-launch__wrapper">
              <div class="started-launch__icon">
                <img src="@/assets/icons/lang/Go.svg" alt="Go" />
                <span>Go</span>
              </div>
            </div>
            <button class="started-launch__button">Launch workspace</button>
          </div>
          <div class="started-launch__language">
            <input type="text" readonly class="started-launch__field" />
            <div class="started-launch__wrapper">
              <div class="started-launch__icon">
                <img src="@/assets/icons/lang/Rust.svg" alt="Rust" />
                <span>Rust</span>
              </div>
            </div>
            <button class="started-launch__button">Launch workspace</button>
          </div>
          <div class="started-launch__language">
            <input type="text" readonly class="started-launch__field" />
            <div class="started-launch__wrapper">
              <div class="started-launch__icon">
                <img src="@/assets/icons/lang/Java.svg" alt="Java" />
                <span>Java</span>
              </div>
            </div>
            <button class="started-launch__button">Launch workspace</button>
          </div>
          <div class="started-launch__language">
            <input type="text" readonly class="started-launch__field" />
            <div class="started-launch__wrapper">
              <div class="started-launch__icon">
                <img src="@/assets/icons/lang/Svelte.svg" alt="Svelte" />
                <span>Svelte</span>
              </div>
            </div>
            <button class="started-launch__button">Launch workspace</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
@import '@/components/StartedBlock/StartedBlock.scss';
</style>
