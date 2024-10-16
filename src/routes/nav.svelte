<script lang="ts">
  import { onMount } from "svelte";
  let openSection = 1;
  import ProjectsGroup from "../components/ProjectsGroup.svelte";
  import SkillsGroup from "../components/SkillsGroup.svelte";

  function toggleAccordion(section: number) {
    openSection = section === openSection ? 0 : section;
  }
</script>

<div class="accordion">
  <button
    class="pb-3 static xl:fixed inline-flex items-center mt-64 gap-x-3 w-full font-semibold text-[14px] text-white/80 hover:text-white/80 focus:outline-none focus:text-white/80 rounded-lg disabled:opacity-50 disabled:pointer-events-none"
    aria-expanded={openSection === 1}
    aria-controls="accordion-content-1"
    on:click={() => toggleAccordion(1)}
  >
    01 <span
      class={`h-[1px] transition-all ease-in-out ${openSection === 1 ? "w-14 bg-white" : "bg-white/80 w-6"}`}
    ></span> Projects
  </button>
  <div
    id="accordion-content-1"
    class={`transform transition-transform duration-500 ${openSection === 1 ? "scale-100 opacity-100" : "scale-95 opacity-0 pointer-events-none"} xl:absolute xl:top-10 xl:translate-x-[760px]`}
    aria-labelledby="accordion-toggle-1"
  >
    <ProjectsGroup />
  </div>

  <button
    class="pb-3 static xl:fixed inline-flex mt-72 items-center gap-x-3 w-full font-semibold text-[14px] text-white/80 hover:text-white/80 focus:outline-none focus:text-white/80 rounded-lg disabled:opacity-50 disabled:pointer-events-none"
    aria-expanded={openSection === 2}
    aria-controls="accordion-content-2"
    on:click={() => toggleAccordion(2)}
  >
    02 <span
      class={`h-[1px] transition-all ease-in-out ${openSection === 2 ? "w-14 bg-white" : "bg-white/80 w-6"}`}
    ></span> Skills
  </button>
  <div
    id="accordion-content-2"
    class={`transform transition-transform duration-500 ${openSection === 2 ? "scale-100 opacity-100" : "scale-95 opacity-0 pointer-events-none"} xl:absolute xl:top-10 xl:translate-x-[600px]`}
    aria-labelledby="accordion-toggle-2"
  >
    <SkillsGroup />
  </div>
</div>
