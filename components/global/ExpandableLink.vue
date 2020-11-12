<template>
  <span>
    <a class="inline-block" href="#" @click.prevent="showKey = !showKey" title="Key"><slot></slot></a>
    <code-block v-if="showKey">
      {{ currentKey }}
    </code-block>
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
      type: Number,
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
