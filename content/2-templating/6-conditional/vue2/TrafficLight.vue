<script>
const TRAFFIC_LIGHTS = ['red', 'orange', 'green'];
export default {
	data() {
		return {
			lightIndex: 0,
		};
	},
	computed: {
		light() {
			return TRAFFIC_LIGHTS[this.lightIndex];
		},
	},
	methods: {
		nextLight() {
			if (this.lightIndex.value + 1 > TRAFFIC_LIGHTS.length - 1) {
				this.lightIndex.value = 0;
			} else {
				this.lightIndex.value++;
			}
		},
	},
};
</script>

<template>
  <div>
    <button @click="nextLight">
      Next light
    </button>
    <p>Light is: {{ light }}</p>
    <p>
      You must
      <span v-if="light === 'red'">STOP</span>
      <span v-else-if="light === 'orange'">SLOW DOWN</span>
      <span v-else-if="light === 'green'">GO</span>
    </p>
  </div>
</template>
