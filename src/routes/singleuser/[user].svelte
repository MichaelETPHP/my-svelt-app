<script context="module">
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

	<div class="w-full md:w-1/2 xl:w-1/4 p-3">
        <div class="bg-white border border-coolGray-100 shadow-dashboard rounded-md">
          <div class="flex flex-col justify-center items-center px-4 pt-8 pb-6 border-b border-coolGray-100">
            <img class="mb-4" src="https://media-exp2.licdn.com/dms/image/C4D03AQH8KAgLTju9jw/profile-displayphoto-shrink_100_100/0/1565165547668?e=1663804800&v=beta&t=0ZfPL8picwKcQHnjs3XUhP4TfGB4XolZbaRI56uuqpU" alt="">
            <h2 class="text-sm font-medium text-coolGray-900">{user.body}</h2>
            <h3 class="mb-3 text-xs font-medium text-coolGray-400">johndoe@flex.co</h3>
           <a sveltekit:prefetch href={`/singleuser/${user.id}`}>
            <button class="flex items-center px-4 py-2 font-medium text-sm text-white bg-green-500 hover:bg-green-600 rounded-md">
              <svg class="mr-2" width="20" height="20" viewbox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M15.8333 3.33334H4.16666C3.50362 3.33334 2.86773 3.59673 2.39889 4.06557C1.93005 4.53441 1.66666 5.17029 1.66666 5.83334V14.1667C1.66666 14.8297 1.93005 15.4656 2.39889 15.9344C2.86773 16.4033 3.50362 16.6667 4.16666 16.6667H15.8333C16.4964 16.6667 17.1323 16.4033 17.6011 15.9344C18.0699 15.4656 18.3333 14.8297 18.3333 14.1667V5.83334C18.3333 5.17029 18.0699 4.53441 17.6011 4.06557C17.1323 3.59673 16.4964 3.33334 15.8333 3.33334V3.33334ZM4.16666 5H15.8333C16.0543 5 16.2663 5.0878 16.4226 5.24408C16.5789 5.40036 16.6667 5.61232 16.6667 5.83334L9.99999 9.9L3.33332 5.83334C3.33332 5.61232 3.42112 5.40036 3.5774 5.24408C3.73368 5.0878 3.94564 5 4.16666 5V5ZM16.6667 14.1667C16.6667 14.3877 16.5789 14.5996 16.4226 14.7559C16.2663 14.9122 16.0543 15 15.8333 15H4.16666C3.94564 15 3.73368 14.9122 3.5774 14.7559C3.42112 14.5996 3.33332 14.3877 3.33332 14.1667V7.73334L9.56666 11.5417C9.69334 11.6148 9.83704 11.6533 9.98332 11.6533C10.1296 11.6533 10.2733 11.6148 10.4 11.5417L16.6667 7.73334V14.1667Z" fill="#F0FDF4"></path>
              </svg>
              <p>Message</p>
            </button>
            </a>
          </div>
          <div class="flex flex-wrap pt-4 pb-6 -m-2">
            <div class="w-full md:w-1/3 p-2">
              <div class="text-center">
                <p class="mb-1 text-xs text-coolGray-900 font-semibold">{user.id}</p>
                <p class="text-xs text-coolGray-400 font-medium">Posts</p>
              </div>
            </div>
            <div class="w-full md:w-1/3 p-2">
              <div class="text-center">
                <p class="mb-1 text-xs text-coolGray-900 font-semibold">420</p>
                <p class="text-xs text-coolGray-400 font-medium">Following</p>
              </div>
            </div>
            <div class="w-full md:w-1/3 p-2">
              <div class="text-center">
                <p class="mb-1 text-xs text-coolGray-900 font-semibold">2.7k</p>
                <p class="text-xs text-coolGray-400 font-medium">Followers</p>
              </div>
            </div>
          </div>
        </div>
      </div>
</div>
