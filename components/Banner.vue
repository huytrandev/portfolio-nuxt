<template>
  <section
    class="w-full bg-opacity-40 rounded-md py-3"
    :class="`${backgroundColor} ${textAlign}`"
  >
    <span class="font-normal">{{ bannerContent }}</span>
  </section>
</template>

<script lang="ts">
import { Component, Vue, Prop } from 'nuxt-property-decorator'

@Component({})
export default class Banner extends Vue {
  @Prop({ default: 'Banner content', required: true }) bannerContent!: string
  @Prop({ default: 'bg-white', required: false }) backgroundColor!: string
  @Prop({ default: 'text-center', required: false }) textAlign!: string
}
</script>
