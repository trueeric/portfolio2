<template>
	<div>
		<h1>Welcome to the homepage</h1>
		<AppAlert> This is an auto-imported component </AppAlert>
	</div>
</template>

<script setup>
useSeoMeta({
	title: 'Main page',
	description: 'This is a main page.',
	ogTitle: 'Main page',
	ogDescription: '[og:description]',
	ogImage: '[og:image]',
	ogUrl: '[og:url]',
	twitterTitle: 'Main page',
	twitterDescription: 'This is a main page.',
	twitterImage: '[twitter:image]',
	twitterCard: 'summary',
})

useHead({
	htmlAttrs: {
		lang: 'en',
	},
	link: [
		{
			rel: 'icon',
			type: 'image/png',
			href: '/favicon.png',
		},
	],
})
</script>
