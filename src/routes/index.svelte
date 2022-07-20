
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

  <script lang="ts">
  import { Col, Container, Row } from 'sveltestrap';
	export let users;
</script>


        
 
      
 

<Container>


  <Row>
    {#each users as user}
    <Col xs="6" sm="3">
       <div class="post-slide">
          <div class="post-img">
            <img src="https://images.unsplash.com/photo-1596265371388-43edbaadab94?crop=entropy&cs=tinysrgb&fit=crop&fm=jpg&h=301&ixid=eyJhcHBfaWQiOjF9&ixlib=rb-1.2.1&q=80&w=501" alt="">
            <a href="#" class="over-layer"><i class="fa fa-link"></i></a>
          </div>
          <div class="post-content">
            <h3 class="post-title">
             <a sveltekit:prefetch class="read-more" href={`/singleuser/${user.id}`}>{user.title}</a>
            </h3>
            <span class="post-date"><i class="fa fa-clock-o"></i>Out 27, 2019</span>
            <a sveltekit:prefetch class="read-more" href={`/singleuser/${user.id}`}>read more</a>
          </div>
        </div>
    </Col>
  {/each}

  </Row>

  </Container>

  



