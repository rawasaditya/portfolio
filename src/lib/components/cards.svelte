<script>
  export let src;
  export let title;
  export let href;
  export let className;
</script>

<a {href} target="_blank" class={`mockup-browser card ${className}`}>
  <div class="mockup-browser-toolbar">
    <div class="text-center bg-white border input border-base-300">{title}</div>
  </div>
  <img {src} />
</a>

<style>
  .card {
    @apply rounded-3xl  text-[#364442]  cursor-pointer;
  }

  .card:hover img {
    scale: 0.9;
    @apply rounded-3xl;
  }

  img {
    transition: 300ms all ease-in-out;
  }

  .purple {
    background-color: hsla(284, 61%, 74%, 1);
  }
  .green {
    background-color: hsla(172, 45%, 75%, 1);
  }

  .orange {
    background-color: #e8b89c;
  }
</style>
