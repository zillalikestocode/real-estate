<script>
  import { Mail, Phone } from "lucide-svelte";
  import logo from "$lib/assets/logo.svg";
</script>

<footer class="bg-primary w-full">
  <div class="grid grid-cols-2 text-white border-b border-white/60">
    <div class="pl-24 py-10 pr-20">
      <img src={logo} alt="logo" />
      <p class="text-sm opacity-80 mt-5">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illum totam
        autem ab, commodi cumque eaque dolorum officiis, fugit, deserunt harum
      </p>

      <div class="mt-10 flex justify-between">
        <div class="flex gap-2.5 items-center">
          <Phone class="opacity-70" size={30} /> +2348010000000
        </div>

        <div class="flex gap-2.5 items-center">
          <Mail class="opacity-70" size={30} /> mail@starrville.com
        </div>
      </div>
    </div>
    <div class="text-white pl-20 pr-24 py-10 border-l border-white/60">
      <h4 class="font-semibold text-xl">Newsletter</h4>
      <p class="text-sm opacity-80 mt-5">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Atque assumenda
        ad voluptatum sequi autem eius, saepe id dicta a perferendis aut.
      </p>
      <div
        class="p-2 pl-4 gap-2.5 flex items-center rounded-full border border-white/60 mt-10"
      >
        <Mail />
        <input
          placeholder="Enter your email"
          class="bg-transparent text-sm focus:outline-none placeholder:text-white/60 focus:border-none"
        />
        <button
          class="ml-auto text-sm font-medium bg-secondary px-4 p-2 rounded-full"
          >Subscribe</button
        >
      </div>
    </div>
  </div>
  <div class="flex items-center py-10 px-24 text-sm text-white justify-between">
    <button>About us</button>
    <button>Blog</button>
    <button>About us</button>
    <button>FAQs</button>
    <button>Privacy Policy</button>
    <button>About us</button>
    <button>Contact</button>
    <button>About us</button>
    <button>Terms of use</button>
  </div>
  <h4 class="m-auto text-center text-sm pb-5 text-white/90">
    © 2024 Starrville
  </h4>
</footer>
