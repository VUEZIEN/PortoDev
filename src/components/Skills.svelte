<script lang="ts">
  export let title: string;
  export let desc: string;
  export let since: string;
  export let children: string = "";
  import Fa from "svelte-fa";
  import { faArrowUpRightFromSquare } from "@fortawesome/free-solid-svg-icons";
</script>

<article
  class={`my-8 ease-out flex flex-col justify-between w-[320px] transition-transform transform duration-300 hover:scale-110 h-auto p-2 min-h-inherit bg-[#202022] hover:bg-opacity-100 group ${children}`}
>
  <div class="flex flex-col gap-4 p-6">
    <h3 class="text-[10px] font-bold tracking-widest uppercase">{title}</h3>
    <h3 class=" text-[14px] text-white/70">{since}</h3>
    <h2 class=" mt-2 text-[24px] text-white font-bold">{desc}</h2>
    <span class="flex gap-3 items-center"
      ><a href="https://github.com/VUEZIEN" class="text-[14px]" target="_blank"
        >See Repo</a
      ><Fa class="w-4" icon={faArrowUpRightFromSquare} /></span
    >
  </div>
</article>
