<template>
  <div>
    <label class="typo__label">Single select</label>
    <multiselect v-model="value" :options="options" :searchable="false" :close-on-select="false" :show-labels="false" placeholder="Pick a value"></multiselect>
    <pre class="language-json"><code>{{ value  }}</code></pre>

  </div>
  <!-- <multiselect v-model="value" :options="options"></multiselect> -->
  
</template>

<script>
import Multiselect from 'vue-multiselect';

// register globally
// Vue.component('multiselect', Multiselect);

export default {
  // OR register locally
  components: { 
    Multiselect
  },

  data () {
    return {
      value: '',
      options: ['Select option', 'options', 'selected', 'mulitple', 'label', 'searchable', 'clearOnSelect', 'hideSelected', 'maxHeight', 'allowEmpty', 'showLabels', 'onChange', 'touched']
    };
  }
};
</script>
<style src="vue-multiselect/dist/vue-multiselect.min.css"></style>

