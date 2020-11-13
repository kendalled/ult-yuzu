<template>
  <span>
    <a class="inline-block" href="#" @click.prevent="showKey = !showKey" title="Key"><slot></slot></a>
    <alert v-if="showKey && opt === 'game'">
      {{ key1 }}
    </alert>
    <alert v-if="showKey && opt === 'prod'">
      {{ key2 }}
    </alert>
  </span>
</template>

<script>
export default {
  name: 'ExpandableLink',
  data () {
    return {
      showKey: false,
      key1: 'aHR0cHM6Ly9kcml2ZS5nb29nbGUuY29tL2ZpbGUvZC8xQXRpSl90Sm9EMGE4R0JrYUg0cXRFM1FKOEhNNER3ZDcvdmlldz91c3A9c2hhcmluZw',
      key2: 'aHR0cHM6Ly9kcml2ZS5nb29nbGUuY29tL2RyaXZlL2ZvbGRlcnMvMXdvbUZITGc2UGl5U3hCZl8ycU1ucTJFSFc4VTlLOXdSP3VzcD1zaGFyaW5n'
    }
  },
  props: {
    opt: {
      type: String,
      default: 'game'
    }
  },
  computed: {
    currentKey () {
      return (this.opt === 'game' ? this.key1 : this.key2)
    }
  }
}
</script>
