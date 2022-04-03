<template>
  <div class="relative bg-light-color min-h-screen">
    <Navbar />
    <main>
      <nuxt :key="$route.fullPath" />
    </main>
    <Footer />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'
import Navbar from '@/components/Navbar.vue'
import Footer from '@/components/Footer.vue'

@Component({
  head: { title: 'Huy Tran - Home page' },
  components: {
    Navbar,
    Footer
  }
})
export default class DefaultLayout extends Vue {}
</script>
