<script context="module">
	export const load = async ({ fetch }) => {
		const resp = await fetch(`http://backend:4000`);
		const data = await resp.text();

		return {
			props: {
				message: data
			}
		};
	};
</script>

<script>
	export let message;
</script>

<h1>Heyyyyyyyy</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
