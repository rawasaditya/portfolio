<script>
  import pms from "$lib/images/pms.png";
  import rawasui from "$lib/images/rawasui.png";
  import pokedex from "$lib/images/pokedex.png";
  import Cards from "./cards.svelte";
</script>

<div>
  <h2 class="work">
    <span class="top-title"><span class="holder">My Work.</span></span>
  </h2>
  <div class="grid grid-cols-1 gap-8 mt-10 md:grid-cols-8">
    <div class="col-span-4">
      <Cards
        src={rawasui}
        href={"https://github.com/rawasaditya/RawasUI"}
        className="green"
        title="RawasUI"
      />
    </div>
    <div class="col-span-4">
      <Cards
        src={pms}
        href={"https://github.com/rawasaditya/projectManagement"}
        className="purple"
        title="Project Management System"
      />
    </div>
    <div class="col-span-4">
      <Cards
        src={pokedex}
        href={"https://poke-dex-fawn.vercel.app/"}
        className="orange"
        title="Poke Dex"
      />
    </div>
  </div>
</div>

<style>
  .work {
    @apply mt-32  text-[#8FDCC2] text-4xl font-bold;
  }
</style>
