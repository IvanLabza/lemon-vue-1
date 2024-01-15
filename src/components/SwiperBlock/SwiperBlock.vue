<template>
  <div class="swiper">
    <swiper :slides-per-view="'auto'" :space-between="30" :grid="{
      }" :pagination="{
  clickable: true,
}" class="mySwiper">
      <swiper-slide v-for="(developer, index) in developers" :key="`${developer.name}-${index}`">
        <div class="developers-item">
          <div class="developers-item__info small-developers-item">
            <span class="title">{{ developer.title }}</span>
            <br /><br />
            <span class="opinion">{{ developer.opinion }}</span>

          </div>

          <div class="developers-item__developer">
            <div class="developers-item__img">
              <img :src="developer.avatar" :alt="developer.name" />
            </div>
            <div class="developers-item__info">
              <div class="developers-item__name">{{ developer.name }}</div>
              <div class="developers-item_position">
                {{ developer.position }} <span>{{ developer.company }}</span>
              </div>
            </div>
          </div>
        </div>

      </swiper-slide>
    </swiper>
    <swiper :direction="'vertical'"  :space-between="24" :pagination="{
        clickable: true,
      }" class="mySwiper-mobile">
      <swiper-slide v-for="(developer, index) in developers" :key="`${developer.name}-${index}`">
        <div class="developers-item ">
          <div class="developers-item__info ">
            <span class="title">{{ developer.title }}</span>
            <br /><br />
            <span class="opinion">{{ developer.opinion }}</span>

          </div>

          <div class="developers-item__developer">
            <div class="developers-item__img">
              <img :src="developer.avatar" :alt="developer.name" />
            </div>
            <div class="developers-item__info">
              <div class="developers-item__name">{{ developer.name }}</div>
              <div class="developers-item_position">
                {{ developer.position }} <span>{{ developer.company }}</span>
              </div>
            </div>
          </div>
        </div>

      </swiper-slide></swiper>
  </div>
</template>

<script>
import SwiperCore, { Navigation, } from 'swiper/core';
import { Swiper, SwiperSlide } from 'swiper/vue';

import 'swiper/swiper-bundle.css';

SwiperCore.use([Navigation,]);

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    const developers = [
      {
        title: 'GitPod is incredibly cool.',
        opinion:
          "In my opinion, this is a big step in open source software contribution. I'm excited to see where we go from here.",
        name: 'Ben Halpern',
        position: 'Creator and Co-founder',
        company: '@forem and @ThePracticalDev',
        avatar: require('@/assets/avatars/1.png'),
      },
      {
        title: 'Overwhelmed by smooth GitPod workspaces.',
        opinion:
          'Let\'s say we were overwhelmed how smooth @gitpod workspaces creation & own Docker image for workspaces worked. Plus, installing @code extensions from the store and integrating @gitlab CI. That blew my mind entirely, and that is hard ;)',
        name: 'Michael Friedrich',
        position: 'Developer Evangelist',
        company: '@GitLab',
        avatar: require('@/assets/avatars/2.png'),
      },
      {
        title: 'Full coding environment for PRs.',
        opinion:
          'Look at any PR (pull request) in a full coding environment where you can edit, build, and test the PR code, by just prepending "gitpod.io#" to the PR URL. Super useful for reviewing/testing stuff without having to check it out locally!',
        name: 'Julius Volz',
        position: 'Creator',
        company: '@forem and @PrometheusIO',
        avatar: require('@/assets/avatars/3.png'),
      },
      {
        title: 'In love with GitPod.',
        opinion:
          "I think I’m in love with @gitpod. It’s such a powerful tool. I’ve learned so much in the past week just from stumbling across Github repos that interest me and appending “http://gitpod.io/#” to the URL. A+ tool all around.",
        name: 'David Ressler',
        position: 'Engineering Manager',
        company: '@instagram',
        avatar: require('@/assets/avatars/4.png'),
      },
    ];


    return {
      developers,

    };
  },

  

}
</script>

<style lang="scss">
@import '@/components/DevelopersBlock/DevelopersBlock.scss';

.developers-item {


  .title {
    color: var(--black);
    font-size: 16px;
    font-weight: 700;
    line-height: 24px;
  }

  .opinion {
    color: var(--black);
    font-size: 16px;
    font-weight: 400;
    line-height: 24px;
    margin-bottom: 14px;
  }

}


.mySwiper {
  @include mobile {
    display: none;
  }

  .swiper-wrapper {
    @include mobile {
      padding-left: 45px;
      height: 350px;
    }

  }

}

.mySwiper-mobile {
  display: none;

  @include mobile {
    display: block;
  }

}


.swiper-slide {
  width: 384px;

}

.swiper-container {
  width: 100%;
}

.swiper-wrapper {
  @include mobile {
    height: 350px;
  }

}
</style>