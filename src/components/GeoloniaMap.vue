<template>
  <div class="geolonia">
  </div>
</template>

<script>
export default {
  name: 'GeoloniaMap',
  props: {},
  mounted() {
	const geoloniaEmbed = document.createElement('script')
	geoloniaEmbed.setAttribute('src', 'https://cdn.geolonia.com/v1/embed?geolonia-api-key=YOUR-API-KEY')
	document.body.append(geoloniaEmbed)
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.geolonia {
	margin: auto;
	width: 300px;
	height: 300px;
}
</style>
