<svelte:head>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.0/dist/css/bootstrap.min.css">
   <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.5.0/font/bootstrap-icons.css">
</svelte:head>
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
