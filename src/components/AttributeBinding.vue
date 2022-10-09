<script setup>
	import { ref } from 'vue'

	const message = ref('No Pain, No Gain')
	const isRed = ref(true)
	const coor = ref('green')

	function toggleRe() {
		isRed.value = !isRed.value
	}

	function toggleColor() {
		color.value = color.value ==="green" ? "blue" : "green"
	}
</script>

<template>
	<p>
		<span :title="message">
			Hover your moue over me for a few seconds to see my dynamical bound title.
		</span>
	</p>
	<p :class="{ red: isRed }" @click="toggleRed">
		This should be red... but click me to toggle it.
	</p>
	<p :style="{ color }" @click="toggleColor">
		This should be green, and should toggle between greeen and blue on click.
	</p>

</template>

<style>
	.red {
		color:  red;
	}
</style>