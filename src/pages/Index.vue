<template>
  <q-page class="flex flex-center">
    {{ address }}
    <img
      alt="Quasar logo"
      src="~assets/quasar-logo-full.svg"
    >
  </q-page>
</template>

<script>
import { defineComponent } from 'vue';
import bsv from 'bsv'
import { ref } from 'vue'

export default defineComponent({
  name: 'PageIndex',
  setup() {
    const privkey = bsv.PrivateKey.fromRandom()
    const address = privkey.toAddress().toString()
    return {
      address: ref(address)
    }
  }
})
</script>
