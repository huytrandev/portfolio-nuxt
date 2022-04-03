<template>
  <section class="w-full">
    <p
      class="title text-xl font-bold border-b-4 text-gray-800 border-gray-800 inline-block mb-3"
    >
      Work
    </p>
    <p class="text-gray-800 indent-8 leading-7 mb-3">
      Lorem ipsum dolor, sit amet consectetur adipisicing elit. Fugiat ipsum
      quas assumenda cum velit eum dolor? Labore doloremque harum debitis,
      similique fuga nihil eos officiis exercitationem, saepe sit ipsum
      temporibus! Lorem ipsum dolor sit amet consectetur adipisicing elit. Est
      consectetur quis iure modi aliquam dolor, quaerat, eveniet, provident
      totam asperiores voluptatem earum architecto vel voluptatibus? Iste alias
      optio sequi dolore!
    </p>
    <div class="text-center">
      <Button
        class="w-40 bg-teal-600 hover:bg-teal-700 text-white duration-300"
        :content="buttonContent"
      />
    </div>
  </section>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'
import Button from '@/components/shared/Button.vue'

@Component({
  components: {
    Button
  }
})
export default class Work extends Vue {
  buttonContent: string = 'My Portfolio'
}
</script>
