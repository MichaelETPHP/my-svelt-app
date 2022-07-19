
<script>
import NavBar from '$lib/NavBar.svelte'
import Footer from '$lib/Footer.svelte'
import '../styles/style.css'
</script>



<header>
    <NavBar/>
</header>


<main>
    <slot></slot>
</main>


<footer>
<Footer/>
</footer>
