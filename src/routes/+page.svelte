<script>
  import Header from "$lib/components/Header.svelte";
  import Footer from "$lib/components/Footer.svelte";
</script>

<Header />

<main>
  <h4 class="h4">Angry Ballpit Bubblegum Footer</h4>
</main>

<Footer />

<style>
  main {
    padding: 20px;
    box-sizing: border-box;
  }

  .h4 {
    position: relative;
    text-align: center;
    font-size: 5vw; /* Responsive font size */
    color: #1F1919;
    background-color: #ff9999;
    border-radius: 5px;
    padding: 10px;
    animation: bounce 2s infinite ease-in-out;
  }

  @keyframes bounce {
    0%, 100% {
      transform: translateY(0);
    }
    50% {
      transform: translateY(-10px);
    }
  }
</style>