<script lang="ts">
	import Post from '$lib/components/Post.svelte';
	import type { PageData } from './$houdini';

	export let data: PageData;

	$: ({ Posts } = data);

	$: posts = $Posts.data?.posts?.edges.map(({ node }) => node) || [];
</script>

<main class="p-6">
	<ul class="grid grid-cols-1 gap-4 sm:grid-cols-2 md:grid-cols-3">
		{#each posts as post}
			<li>
				<Post {post} />
			</li>
		{/each}
	</ul>
</main>
