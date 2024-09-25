<script>
  import { register } from "swiper/element/bundle";
  import img2 from "$lib/assets/image2.jpg";
  import img3 from "$lib/assets/image3.jpg";
  import img4 from "$lib/assets/image4.jpg";
  import img5 from "$lib/assets/image5.jpg";
  import { ChevronLeft, ChevronRight } from "lucide-svelte";
  register();

  const listings = [
    {
      name: "Saint Milano Village",
      image: img2,
      address: "121 Iyana Apaja, Lagos",
      description: "5 bedrooms, Parking Lot",
    },
    {
      name: "Lekki Bay View",
      image: img3,
      address: "Bay view lekki, Lagos.",
      description: "5 bedrooms, Parking Lot",
    },
    {
      name: "Makani Suites",
      image: img4,
      address: "8 Victory lane Gwagalada, Abuja",
      description: "5 bedrooms, Parking Lot",
    },
    {
      name: "La Casa Del Supreme",
      image: img5,
      address: "Supreme Estate, Port Harcourt",
      description: "5 bedrooms, Parking Lot",
    },
    {
      name: "Lekki Bay View",
      image: img3,
      address: "Bay view lekki, Lagos.",
      description: "5 bedrooms, Parking Lot",
    },
  ];
</script>

<div class="flex mt-10 justify-between items-end">
  <div class="">
    <h4 class="font-semibold text-3xl">Top 10 Properties</h4>
    <p class="text-lg text-neutral-500">
      Find the properties that fits your standard and comfort
    </p>
  </div>
  <div class="flex items-center gap-2.5 cursor-pointer">
    <button
      class="p-4 slide-prev hover:bg-secondary/50 transition-all duration-500 rounded-full bg-neutral-100"
    >
      <ChevronLeft size={20} />
    </button>
    <button
      class="p-4 slide-next hover:bg-secondary/50 transition-all cursor-pointer duration-500 rounded-full bg-neutral-100"
    >
      <ChevronRight size={20} />
    </button>
  </div>
</div>

<div class="mt-5">
  <swiper-container
    navigation={{ nextEl: ".slide-next", prevEl: ".slide-prev" }}
    slides-per-view="4"
    loop="true"
    speed="500"
    space-between="40"
  >
    {#each listings as listing}
      <swiper-slide
        ><div class="relative w-full">
          <div
            class="bg-primary p-2 py-1 rounded-md absolute top-0 left-0 font-medium text-white"
          >
            15% off
          </div>
          <div
            class="w-full aspect-square rounded-tl-md rounded-r-3xl rounded-bl-3xl bg-neutral-300"
          >
            <img
              src={listing.image}
              class="object-cover w-full rounded-tl-md rounded-r-3xl rounded-bl-3xl h-full"
              alt={listing.name}
            />
          </div>
        </div>
        <h4 class="font-semibold text-lg mt-2.5">{listing.name}</h4>
        <h4 class="text-neutral-500 text-sm">{listing.address}</h4>
        <h4 class="text-sm text-neutral-400">{listing.description}</h4>
      </swiper-slide>
    {/each}
  </swiper-container>
</div>
