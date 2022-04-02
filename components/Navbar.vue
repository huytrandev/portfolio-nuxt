<template>
  <nav
    class="w-full bg-white backdrop-blur bg-opacity-25 sticky top-0 text-center"
  >
    <div
      class="nav-container max-w-3xl w-full px-4 inline-flex justify-between items-center h-14 py-2"
    >
      <div class="nav-wrapper">
        <nuxt-link to="/">
          <span class="text-lg font-bold tracking-wide">Huy Tran</span>
        </nuxt-link>
        <nuxt-link
          to="/works"
          class="nav-item hover:underline underline-offset-4 hidden sm:inline"
        >
          <span class="">Works</span>
        </nuxt-link>
        <nuxt-link
          to="/posts"
          class="nav-item hover:underline underline-offset-4 hidden sm:inline"
        >
          <span class="">Posts</span>
        </nuxt-link>
        <nuxt-link
          to="/source"
          class="nav-item hover:underline underline-offset-4 hidden sm:inline"
        >
          <span class="">Source</span>
        </nuxt-link>
      </div>
      <div class="inline-flex">
        <button
          class="h-10 w-10 rounded-xl bg-purple-600 flex items-center justify-center text-white hover:bg-purple-700 duration-200"
        >
          <MoonIcon class="w-5" />
        </button>
        <button
          class="flex sm:hidden h-10 w-10 rounded-xl bg-transparent items-center justify-center duration-200 ml-2 border-2 border-gray-200 focus:ring focus:ring-purple-500"
        >
          <MenuIcon class="w-5" @click="showMenu = !showMenu" />
        </button>
      </div>
    </div>

    <!-- Menu -->
    <div
      v-if="showMenu"
      class="mobile-menu fixed right-3 bg-white shadow-sm w-1/2 rounded duration-200 flex flex-col text-left px-4 py-2"
    >
      <nuxt-link to="/">
        <span>About</span>
      </nuxt-link>
      <nuxt-link to="/works">
        <span>Works</span>
      </nuxt-link>
      <nuxt-link to="/posts">
        <span>Posts</span>
      </nuxt-link>
      <nuxt-link to="/source">
        <span>Source</span>
      </nuxt-link>
    </div>
  </nav>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'
import { SunIcon, MenuIcon } from '@vue-hero-icons/outline'
import { MoonIcon } from '@vue-hero-icons/solid'

@Component({
  components: {
    SunIcon,
    MoonIcon,
    MenuIcon
  }
})
export default class Navbar extends Vue {
  showMenu: boolean = false
}
</script>

<style lang="scss" scoped>
.nav-container {
  .nav-wrapper {
    & a:not(:last-child) {
      margin-right: 2rem;
    }
  }
}

.mobile-menu {
  a:not(:last-child) {
    @apply mb-3 focus:bg-opacity-50;
  }
}
</style>
