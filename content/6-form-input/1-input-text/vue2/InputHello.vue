<script>
export default {
	data() {
		return {
			text: '',
		};
	},
};
</script>

<template>
  <div>
    <p>{{ text }}</p>
    <input v-model="text">
  </div>
</template>
