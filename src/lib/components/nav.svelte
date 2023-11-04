<script>
  import { page } from "$app/stores";
</script>

<nav>
  <ul>
    <li class:active={$page.route.id === "/"}>
      <a class="test" href="/">Home</a>
    </li>
    <li class:active={$page.route.id === "/about"}>
      <a class="test" href="/about">About</a>
    </li>
    <li class:active={$page.route.id === "/blogs"}>
      <a class="test" href="/blogs">Blogs</a>
    </li>
    <li class:active={$page.route.id === "/contact"}>
      <a class="test" href="/contact">Contact</a>
    </li>
  </ul>
</nav>

<style>
  nav {
    @apply my-10;
  }
  nav ul {
    @apply flex w-full justify-center gap-10;
  }
  li {
    @apply px-7 py-1 rounded-full;
    color: hsla(159, 42%, 88%, 1);
  }

  li.active {
    background-color: hsla(160, 52%, 71%, 0.1);
  }
</style>
