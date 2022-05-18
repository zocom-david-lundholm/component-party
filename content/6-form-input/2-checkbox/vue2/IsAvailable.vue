<script>
export default {
	data() {
		return {
			isAvailable: true,
		};
	},
};
</script>

<template>
  <span>
    <input
      id="is-available"
      v-model="isAvailable"
      type="checkbox"
    >
    <label for="is-available">Is available</label>
  </span>
</template>
