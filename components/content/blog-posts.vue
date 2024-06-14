<template>
	<!-- 不使用markdown格式 "not-prose" -->
	<section class="not-prose">
		<ul>
			<li v-for="post in posts" :key="post._path">
				<NuxtLink :to="post._path">
					{{ post.title }}
				</NuxtLink>
			</li>
		</ul>
	</section>
</template>
<script setup>
const { data: posts } = await useAsyncData('blog-list', () =>
	queryContent('/blog')
		.where({ _path: { $ne: '/blog' } })
		.only(['_path', 'title'])
		.find()
)
// $ne Match if item not equals condition
console.log(posts)
</script>
