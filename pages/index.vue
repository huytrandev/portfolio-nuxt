<template>
  <div class="container max-w-xl w-full m-auto py-5 px-8 sm:px-6">
    <Banner :banner-content="bannerContent" class="mb-8" />
    <Personal class="mb-8" />
    <Work class="mb-8" />
    <Bio class="mb-8" />
    <Hobby class="mb-8" />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'
import Banner from '@/components/Banner.vue'
import Personal from '@/components/Personal.vue'
import Work from '@/components/Work.vue'
import Bio from '@/components/Bio.vue'
import Hobby from '@/components/Hobby.vue'

@Component({
  components: {
    Banner,
    Personal,
    Work,
    Bio,
    Hobby
  }
})
export default class Index extends Vue {
  bannerContent: string = `Hello, I'm a full-stack developer in Vietnam!`
}
</script>
