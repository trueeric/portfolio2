<template>
	<div>
		<p>This page will be displayed at the /about route.</p>
	</div>
	<div>
		<button @click="enableCustomLayout">Update Layout</button>
	</div>
</template>

<script setup>
useHead({
	title: 'About',
})
</script>
