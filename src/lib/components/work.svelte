<script>
  import pms from "$lib/images/pms.png";
  import rawasui from "$lib/images/rawasui.png";
</script>

<h2 class="work">
  <span class="top-title"><span class="holder">My Work.</span></span>
</h2>
<div class="grid grid-cols-1 gap-8 mt-10 md:grid-cols-8">
  <div class="col-span-4">
    <a
      href="https://github.com/rawasaditya/RawasUI"
      target="_blank"
      class="border mockup-browser card green"
    >
      <div class="mockup-browser-toolbar">
        <div class="border input border-base-300">RawasUI</div>
      </div>
      <img src={rawasui} />
    </a>
  </div>
  <div class="col-span-4">
    <a
      c
      href="https://github.com/rawasaditya/projectManagement"
      target="_blank"
      class="border mockup-browser card purple"
    >
      <div class="mockup-browser-toolbar">
        <div class="border input border-base-300">
          Project Management System
        </div>
      </div>
      <img src={pms} />
    </a>
  </div>
</div>

<style>
  .work {
    @apply mt-32  text-[#8FDCC2] text-4xl font-bold;
  }

  .card {
    @apply rounded-3xl  text-[#364442]  cursor-pointer;
  }
  .purple {
    background-color: hsla(284, 61%, 74%, 1);
  }
  .green {
    background-color: hsla(172, 45%, 75%, 1);
  }

  img {
    transition: 300ms all ease-in-out;
  }

  .card:hover img {
    scale: 0.9;
    @apply rounded-3xl;
  }
</style>
