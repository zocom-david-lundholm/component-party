<script>
export default {
	data() {
		return {
			name: 'John',
		};
	},
	mounted() {
		this.name = 'Jane';
	},
};
</script>

<template>
  <h1>Hello {{ name }}</h1>
</template>
