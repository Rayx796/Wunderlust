<script>
  import Header from "./components/Header.svelte";
  import Hero from "./components/Hero.svelte";
  import About from "./components/About.svelte";
  import Service from "./components/Service.svelte";
  import Faq from "./components/FAQ.svelte";
  import Footer from "./components/Footer.svelte";
  import Team from "./components/Team.svelte"
  import Cards from "./components/Cards.svelte";
</script>

<main>
  <Header/>
  <div>
    <article>
      <Hero/>
      <About/>
      <Cards/>
      <Service/>
      <Team/>
      <Faq/>
    </article>
  </div>
  <Footer/>
</main>


 
