<script lang="ts">
	export let post;
</script>

<article class="rounded-md border border-slate-200 bg-slate-100 p-4">
	<h2 class="mb-2 text-lg font-bold">{post.title}</h2>
	{@html post.content || '<p>Aucun contenu</p>'}
</article>
