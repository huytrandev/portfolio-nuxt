<template>
  <div style="height: 100vh" class="container max-w-xl w-full m-auto py-5 px-8 sm:px-6">
    <Banner :banner-content="bannerContent" class="mb-8" />
    <Personal />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'
import Banner from '@/components/Banner.vue'
import Personal from '@/components/Personal.vue'

@Component({
  components: {
    Banner,
    Personal
  }
})
export default class Index extends Vue {
  bannerContent: string = `Hello, I'm a full-stack developer in Vietnam!`
}
</script>
