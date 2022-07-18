<script context="module">
	export async function load({ fetch }) {
		const res = await fetch('https://jsonplaceholder.typicode.com/posts');
		const users = await res.json();
		// console.log(users);
		if (res.ok) {
			return {
				props: {
					users
				}
			};
		}

		return {
			status: res.status,
			error: new Error('Could not fetch the Users')
		};
	}
</script>
<script>
	export let users;
</script>
<a href="/">HOME</a> || <a href="about">ABOUT</a>

<center><h1>List off Post</h1></center>
{#each users as user}
	<a sveltekit:prefetch href={`/singleuser/${user.id}`}>{user.title}</a>
	<hr />
{/each}
