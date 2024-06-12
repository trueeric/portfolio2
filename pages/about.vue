<template>
	<div>
		<p>This page will be displayed at the /about route.</p>
	</div>
	<div>
		<button @click="enableCustomLayout">Update Layout</button>
	</div>
</template>

<script setup>
// definePageMeta({
// 	layout: 'another',
// })
// function enableCustomLayout(){
// 	setPageLayout(layout:'another')
// }

function enableCustomLayout() {
	setPageLayout('another')
}
</script>
