<script>
  // @ts-nocheck

  import "../app.css";
  import { afterNavigate } from "$app/navigation";


  afterNavigate(() => {
    window.HSStaticMethods.autoInit();
  });
</script>

<div class="app ">
  <main class="">
    <slot />
  </main>
</div>

<style lang="postcss">
  :global(html) {
    background-color: #161616;
  }
  
</style>
