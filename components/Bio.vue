<template>
  <section class="w-full">
    <p
      class="title text-xl font-bold border-b-4 text-gray-800 border-gray-800 inline-block mb-3"
    >
      Bio
    </p>
    <div class="event">
      <p
        v-for="(event, index) in events"
        :key="index"
        class="text-gray-800 mb-2 flex w-ful"
      >
        <span class="font-bold" v-text="event.year" />
        <span class="ml-4" v-text="event.event"></span>
      </p>
    </div>
  </section>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'
import { EventDto } from '~/types/common'

@Component({
  components: {}
})
export default class Bio extends Vue {
  events: EventDto[] = [
    {
      year: 1999,
      event: 'Born in Vinh Long, Vietnam'
    },
    {
      year: 2021,
      event: 'Worked at TPS Software Corporation'
    },
    {
      year: 2022,
      event:
        'Graduated from Cantho University with a bachelor’s degree in Software Engineering'
    }
  ]
}
</script>
