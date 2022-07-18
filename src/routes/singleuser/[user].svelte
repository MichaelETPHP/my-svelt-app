<script context="module">
	// import { page } from '$app/stores';
	export async function load({  fetch, params }) {
		// console.log(params.id)
		const id = params.user
		const res = await fetch(`https://jsonplaceholder.typicode.com/posts/${id}`);
		const user = await res.json();
		// const response = await fetch(url);
	if (res.ok) {
			return {
				props: {
					user
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
	export let user;
</script>

<div>
	<a href="/">HOME</a> || <a href="../about">ABOUT</a> || <a href="">Contact</a>
	<h1>{user.title}</h1>
</div>
