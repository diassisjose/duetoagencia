<template>
  <b-col class="switchdeact mx-1 my-1 " v-on:click="checked = !checked" :class="{checked: checked}">
      <h4 class="h-switch">{{ title }}</h4>
      <p class="p-switch">{{ content }}</p>
      <b-col align="right" class="footer-switch">
        <input class="footer-switch" type="checkbox" v-bind:value="value" name="" v-model="checked">
      </b-col>
  </b-col>
</template>

<script>
export default {
  props: [
        'title', 'content', 'value'
    ],
  data() {
    return {
      checked: false,
    }
  }
}
</script>