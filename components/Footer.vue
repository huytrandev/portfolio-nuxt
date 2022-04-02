<template>
  <footer class="w-full flex justify-center items-center">
    <div class="max-w-7xl px-4 m-auto text-center">
      <span class="text-sm text-gray-500 tracking-wide">© {{ currentYear }} Huy Tran. All Right Reserved.</span>
    </div>
  </footer>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'

@Component({})
export default class Footer extends Vue {
  currentYear = new Date().getFullYear()
}
</script>

<style lang="scss" scoped>
footer {
  height: 72px;
}
</style>
