<template>
  <section
    class="w-full flex flex-col sm:flex-row justify-between items-center sm:items-start"
  >
    <div class="introduce flex flex-col items-center sm:items-start">
      <p class="name text-4xl font-medium">Huy Tran Thanh</p>
      <p class="description font-light tracking-wide mt-2">
        Full-stack Developer
      </p>
    </div>
    <div
      class="avatar w-24 h-24 rounded-full overflow-hidden border-2 border-white mt-4 sm:mt-0"
    >
      <img :src="require(`~/assets/images/default-logo.png`)" alt="avatar" />
    </div>
  </section>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'

@Component({})
export default class Personal extends Vue {}
</script>
