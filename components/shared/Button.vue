<template>
  <button class="h-10 rounded-md font-medium" v-text="content" />
</template>

<script lang="ts">
import { Component, Vue, Prop } from 'nuxt-property-decorator'

@Component({})
export default class Button extends Vue {
  @Prop({ default: 'Button' }) content!: string
}
</script>
