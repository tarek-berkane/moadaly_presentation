<script setup lang="ts">
import { defineProps, defineComponent } from 'vue'
import Default from './default.vue'

const components = defineComponent({ Default })
const props = defineProps({
  eventLogo: {
    type: String,
  },
  eventUrl: {
    type: String,
  },
  twitter: {
    type: String,
  },
  twitterUrl: {
    type: String,
  },
  presenterImage: {
    type: String,
  },
})
</script>

<template>
  <default
    class="presenter"
    :logo-header="logoHeader"
    :event-logo="eventLogo"
    :event-url="eventUrl"
    :twitter="twitter"
    :twitter-url="twitterUrl"
  >
    <h1>أعضاء الفريق</h1>
    <div class="flex items-center align-center justify-center">
      <figure class="flex justify-center align-center  ">
        <div class="mx-2 text-center">
          <img
            src="ta.jpeg"
            class="
              relative
              rounded-full
              object-cover
              h-42
              w-42
              border border-8 border-secondary-400
              z-10
            "
          />
          <h3>Tarek berkane</h3>
        </div>
        <div class="mx-2 text-center">
          <img
            src="za.jpg"
            class="
              relative
              rounded-full
              object-cover
              h-42
              w-42
              border border-8 border-secondary-400
              z-10
            "
          />
          <h3>Taha Zerrouki</h3>
        </div>
        <div class="mx-2 text-center">
          <img
            src="mj.jpeg"
            class="
              relative
              rounded-full
              object-cover
              h-42
              w-42
              border border-8 border-secondary-400
              z-10
            "
          />
          <h3>Smail <br> Abd El Madjid</h3>
        </div>

        <div class="mx-2 text-center">
          <img
            src="f2.jpg"
            class="
              relative
              rounded-full
              object-cover
              h-42
              w-42
              border border-8 border-secondary-400
              z-10
            "
          />
          <h3>Aouf Ali</h3>
        </div>
      </figure>
    </div>
  </default>
</template>
