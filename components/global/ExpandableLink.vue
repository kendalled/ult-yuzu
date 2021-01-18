<template>
  <span>
    <a class="inline-block" href="#" @click.prevent="showKey = !showKey" title="Key"><slot></slot></a>
    <code-group v-if="showKey" class="my-4">
      <code-block label="Game dump" active v-if="opt === 'game'">
        <code>{{key1}}</code>
      </code-block>
      <code-block label="Keys folder" active v-if="opt === 'prod'">
        <code>
          {{key2}}
        </code>
      </code-block>
    </code-group>
  </span>
</template>

<script>
export default {
  name: 'ExpandableLink',
  data () {
    return {
      showKey: false,
      key1: 'aHR0cHM6Ly9kcml2ZS5nb29nbGUuY29tL2ZpbGUvZC8xQXRpSl90Sm9EMGE4R0JrYUg0cXRFM1FKOEhNNER3ZDcvdmlldz91c3A9c2hhcmluZw1',
      key2: 'aHR0cHM6Ly9kcml2ZS5nb29nbGUuY29tL2RyaXZlL2ZvbGRlcnMvMXdvbUZITGc2UGl5U3hCZl8ycU1ucTJFSFc4VTlLOXdSP3VzcD1zaGFyaW5n1'
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
