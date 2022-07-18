<script context="module">
	export function load({ error }) {
		return {
			props: { message: error.message }
		};
	}
</script>

<script>
export let message
</script>


<h1>Opps </h1>
<p>{message}</p>
<a href="/">Back to Home </a>
