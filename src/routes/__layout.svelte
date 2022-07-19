
<script>
import Nav from '$lib/nav.svelte'
import '../styles/global.css'
import Footer from '$lib/footer.svelte'  
import About from "./about.svelte";
import Home from "./about.svelte";
  
</script>



<header>
    <Nav/>
</header>

<main>
    <slot></slot>
</main>
<footer>
   <Footer/>
</footer>
