<template>
  <p>{{ event.organizerName }}</p>
  <p>{{ event.address }}</p>
</template>

<script>
export default {
  props: ['event']
}
</script>
