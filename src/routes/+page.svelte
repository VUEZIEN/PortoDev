<script>
  import Nav from "./nav.svelte";
  import photos from "$lib/images/imageme.jpeg";
  import Fa from "svelte-fa";
  import { faTwitter } from "@fortawesome/free-brands-svg-icons";
  import { faGithub } from "@fortawesome/free-brands-svg-icons";
  import { faArrowUpRightFromSquare } from "@fortawesome/free-solid-svg-icons";
  import Accordion from "../components/Accordion.svelte";
  import ProjectsGroup from "../components/ProjectsGroup.svelte";
  import SkillsGroup from "../components/SkillsGroup.svelte";
</script>

<svelte:head>
  <title>PortoDev</title>
  <meta name="description" content="Svelte demo app" />
</svelte:head>

<section
  class="static text-white flex flex-col justify-between w-full p-24 sm:p-32 md:max-w-496 md:h-screen lg:py-88 lg:pl-88 md:pr-72 lg:pr-0"
>
  <div class="flex flex-col static xl:fixed gap-10 w-[408px]">
    <div class="">
      <h1
        class="text-[2xl] font-bold leading-tight lg:text-[64px] lg:leading-none text-zenith"
      >
        Ariiq Maazin
      </h1>
      <h2
        class="mt-4 text-[22px] font-600 font-semibold leading-tight text-sunrise"
      >
        Front end web developers
      </h2>
      <div class="leading-loose text-white/80 text-[14px]">
        <p class="mt-4">
          I can create front-end websites using React and Typescript technology.
        </p>
        <p>
          In my spare time, I create independent projects to build my front-end
          skills.
        </p>
      </div>
    </div>
  </div>
  <Nav />
  <div class=" flex items-center static xl:fixed  w-full mt-32 md:mt-[29rem] gap-8">
    <img
      src={photos}
      alt=""
      draggable="false"
      class="w-[50px] h-[50px] object-cover rounded-full"
    />
    <span class="flex gap-3 items-center"
      ><Fa class="w-4" icon={faTwitter} /><a
        href="https://x.com/Kingostyl"
        class="text-[14px]"
        target="_blank">Twitter</a
      ><Fa class="w-4" icon={faArrowUpRightFromSquare} /></span
    >
    <span class="flex gap-3 items-center"
      ><Fa class="w-4" icon={faGithub} /><a
        href="https://github.com/VUEZIEN"
        class="text-[14px]"
        target="_blank">Github</a
      ><Fa class="w-4" icon={faArrowUpRightFromSquare} /></span
    >
  </div>
</section>
