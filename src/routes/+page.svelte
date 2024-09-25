<script>
  import Hero from "../components/hero.svelte";
  import Header from "../components/header.svelte";
  import Properties from "../components/properties.svelte";
  import Footer from "../components/footer.svelte";
  import Testimonial from "../components/testimonial.svelte";
</script>

<div class="p-5 md:px-10">
  <Header />
  <Hero />
  <div class="w-full h-1 bg-neutral-200" />
  <Properties />
  <Testimonial />
</div>
<Footer />
