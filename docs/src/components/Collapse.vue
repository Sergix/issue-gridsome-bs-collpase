<template>
  <div class="container p-4 bg-light">
    <b-button
      class="code-toggler feather icon-code cursor-pointer"
      :aria-expanded="!code_visible ? 'true' : 'false'"
      @click="code_visible = !code_visible"
    >
    Toggle
    </b-button>

    <div class="card-content">
      <!-- Card Content -->
      <slot />

      <!-- Code Content -->
      <b-collapse
        v-model="code_visible"
        class="card-code"
      >
        <slot name="code" />
      </b-collapse>
    </div>
  </div>
</template>

<script>
import { BButton, BCollapse } from 'bootstrap-vue'

export default {
  components: {
    BButton,
    BCollapse,
  },
  data: () => ({
    code_visible: false,
  }),
}
</script>
