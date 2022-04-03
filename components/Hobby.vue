<template>
  <section class="w-full">
    <p
      class="title text-xl font-bold border-b-4 text-gray-800 border-gray-800 inline-block mb-3"
    >
      I &hearts;
    </p>
    <p class="text-gray-800 indent-8 leading-7 mb-3">
      Music, Drawing, Playing Guitar, Cooking, Gym.
    </p>
  </section>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'

@Component({
  components: {}
})
export default class Hobby extends Vue {}
</script>
