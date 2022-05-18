<script>
export default {
	data() {
		return {
			canCome: true,
		};
	},
	methods: {
		onAnswerNo() {
			this.canCome = false;
		},
		onAnswerYes() {
			this.canCome = true;
		},
	},
};
</script>

<template>
  <div>
    <p>Can I come ?</p>
    <AnswerButton
      @yes="onAnswerYes"
      @no="onAnswerNo"
    />
    <p style="font-size: 50px">
      {{ canCome ? '😀' : '😥' }}
    </p>
  </div>
</template>
