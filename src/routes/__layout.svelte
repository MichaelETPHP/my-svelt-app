<svelte:head>
  <link rel="stylesheet" href="bootstrap.min.css">
</svelte:head>
<script>
import NavBar from '$lib/NavBar.svelte'
import Footer from '$lib/Footer.svelte'
import '../styles/style.css'
import '../styles/global.css'

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
