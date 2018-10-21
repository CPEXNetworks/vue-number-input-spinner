<template>
  <div id="app" style="text-align: center; padding: 10vw; max-width: 960px; width: 90vw">
    <div>
      <NumberInputSpinner />
      <hr>
      {{ test }}
      <NumberInputSpinner :integerOnly="true"  :step=".5" :min="1" :value='10' v-model="test"/>
    </div>
  </div>
</template>

<script>
import NumberInputSpinner from 'components/NumberInputSpinner.vue';

export default {
    components: {
        NumberInputSpinner,
    },

    data: function () {
        return {
            test: 10,
        };
    },
};
</script>
