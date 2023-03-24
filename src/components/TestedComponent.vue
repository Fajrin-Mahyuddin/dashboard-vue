<script lang="ts">
export default {
	data() {
		return {
			text: "this a text"
		}
	},
	props: { title: String, fun: Function },
}
</script>

<template>
	<div>{{ text }} - {{ title }}</div>
	<button @click="fun && fun()">click button</button>
</template>