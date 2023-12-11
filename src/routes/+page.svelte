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
.h4 {
  position: fixed;
  top: 37%;
  left: 24%;
  transform: translate(-50%, -50%);
  text-align: center;
  font-family: sans-serif;
  font-size: 34px;
  color: #fff;
  background-color: #ff9999;
  border-radius: 5px;
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
  