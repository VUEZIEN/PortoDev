<script lang="ts">
  export let leangue: string;
  export let title: string;
  export let content: string;
  export let link: string;
</script>

<article
  class=" transition-transform ease-out md:hover:scale-110 w-[504px] bg-[#202022] my-4 z-10"
>
  <a class="block p-6" href={link} target="_blank" rel="noopener noreferrer">
    <p class="text-[10px] font-bold tracking-widest uppercase">
      {leangue}
    </p>
    <h3 class="mt-3 text-[24px] font-semibold leading-tight" itemprop="name">
      {title}
    </h3>
    <p class="mt-2 text-[14px] text-white/70">
      {content}
    </p>
  </a>
</article>
