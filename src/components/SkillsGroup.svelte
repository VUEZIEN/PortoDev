<script>
  import Skills from "./Skills.svelte";
</script>

<div class="flex flex-wrap w-1/2 gap-3">
  <Skills
    title="ReactJS"
    since="starting at June 2023"
    desc="I've studied for 1.5 years with several projects"
  />
  <Skills
    title="Tailwind CSS"
    since="starting at January 2023"
    desc="I have been studying for 2 years by combining several projects."
        children="xl:translate-y-[10%]"
  />

  <Skills
    title="NestJS"
    since="starting at June 2023"
    desc="I have been studying for 1.5 years with several projects but I didn't deepen it"
    children="xl:-translate-y-[20%]"
  />

  <Skills
    title="Svelte"
    since="starting at October 2024"
    desc="I have been studying for 2 months with my portfolio project"
     children="xl:-translate-y-[10%]"
  />
</div>
