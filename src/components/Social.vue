<template>
   <ul class="social">
      <li v-for="(social, i) in socialList" :key="i">
         <a :href="social.link" target="_blank" rel="noreferrer"
            ><img class="svg" :src="social.src" alt="social"
         /></a>
      </li>
   </ul>
   <!-- End. social -->
</template>

<script>
export default {
   data() {
      return {
         socialList: [
            {
               link: 'https://www.facebook.com/',
               src: require('../assets/img/svg/social/facebook.svg'),
            },
            {
               link: 'https://www.instagram.com/',
               src: require('../assets/img/svg/social/instagram.svg'),
            },
            {
               link: 'https://github.com/moseswescombe',
               src: require('../assets/img/svg/social/github.svg'),
            },
            {
               link: 'https://linkedin.com',
               src: require('../assets/img/svg/social/linkedin.svg'),
            },
         ],
      };
   },
};
</script>

<style lang="scss" scoped></style>
