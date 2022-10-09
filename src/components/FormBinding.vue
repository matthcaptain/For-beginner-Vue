<script setup>
	import { ref } from 'vue'

	const text = ref('Edit me')
	const checked = ref(true)
	const checkedNames = ref(['Jack'])
	const picked = ref('One')
	const selected = ref('A')
	const multiSelected = ref(['A'])
</script>

<template>
	<h2>Text Input</h2>
	<input v-model="text">{{ text }}

	<h2>Checkbox</h2>
	<input type="checkbox" id="checkbox" v-model="checked">
	<label for="checkbox">Checked: {{ checked }}</label>

	
</template>