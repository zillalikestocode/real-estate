<script>
  import Logo from "../components/logo.svelte";
</script>

<header>
  <nav class="flex text-neutral-600 font-medium items-center gap-10">
    <div class="flex items-center gap-10">
      <button><h4>Home</h4></button>
      <button><h4>Buy</h4></button>
      <button><h4>Sell and Rent</h4></button>
    </div>
    <div class="mx-auto -translate-y-2">
      <Logo />
    </div>
    <div class="flex items-center gap-5">
      <button><h4>Our projects</h4></button>
      <button><h4>Join Us</h4></button>
      <button><h4>About us</h4></button>
      <button
        class="rounded-full px-3 py-1 text-sm border border-secondary text-secondary"
        >Log in</button
      >
    </div>
  </nav>
</header>
