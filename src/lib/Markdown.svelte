<script lang="ts">
	import { marked } from 'marked';

	const { content }: { content: string } = $props();

	const html = $derived(marked.parse(content));
</script>

{@html html}
