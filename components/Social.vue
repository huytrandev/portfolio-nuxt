<template>
  <section class="w-full">
    <p
      class="title text-xl font-bold border-b-4 text-gray-800 border-gray-800 inline-block mb-3"
    >
      On the web
    </p>
    <div class="socials">
      <a
        href="https://www.facebook.com/tranthanhhuy.fb"
        target="_blank"
        class="text-gray-800 rounded-md bg-transparent hover:bg-purple-200 mb-2 flex w-fit pl-4 pr-5 py-1 items-center duration-300"
      >
        <img
          src="~/assets/icons/facebook.svg"
          class="w-8"
          alt="facebook-logo"
        />
        <span class="font-semibold hover:underline underline-offset-4 ml-2"
          >@tranthanhhuy.fb</span
        >
      </a>
      <a
        href="https://www.instagram.com/hyouwhy"
        target="_blank"
        class="text-gray-800 rounded-md bg-transparent hover:bg-purple-200 mb-2 flex w-fit pl-4 pr-5 py-1 items-center duration-300"
      >
        <img
          src="~/assets/icons/instagram.svg"
          class="w-8"
          alt="instagram-logo"
        />
        <span class="font-semibold hover:underline underline-offset-4 ml-2">@hyouwhy</span>
      </a>
      <a
        href="https://www.linkedin.com/in/huy-tran-5b5348163/"
        target="_blank"
        class="text-gray-800 rounded-md bg-transparent hover:bg-purple-200 mb-2 flex w-fit pl-4 pr-5 py-1 items-center duration-300"
      >
        <img
          src="~/assets/icons/linkedin.svg"
          class="w-8"
          alt="linkedin-logo"
        />
        <span class="font-semibold hover:underline underline-offset-4 ml-2">Huy Tran</span>
      </a>
    </div>
  </section>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'

@Component({
  components: {}
})
export default class Social extends Vue {}
</script>
