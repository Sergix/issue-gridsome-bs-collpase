<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <Collapse>
      <p>Toggling is working fine w/o any errors here.</p>

      <template #code>
&lt;p&gt;I am some code&lt;/p&gt;
      </template>
    </Collapse>
  </div>
</template>

<script>
// @ is an alias to /src
import Collapse from '@/components/Collapse.vue'

export default {
  name: 'Home',
  components: {
    Collapse
  }
}
</script>
