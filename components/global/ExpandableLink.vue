<template>
  <span>
    <a class="inline-block" href="#" @click.prevent="showKey = !showKey" title="Key"><slot></slot></a>
    <p class="italic font-medium" v-if="showKey">
      {{ key }}
    </p>
  </span>
</template>

<script>
export default {
  name: 'ExpandableLink',
  data () {
    return {
      showKey: false,
      key: 'aHR0cHM6Ly9kcml2ZS5nb29nbGUuY29tL2RyaXZlL2ZvbGRlcnMvMURVVUwxeFdWNGRjZ2NpOUdmMXM2X3Q0QmV1UGdQSlJDP3VzcD1zaGFyaW5n'
    }
  }
}
</script>
