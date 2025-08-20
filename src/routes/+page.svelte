<script>
  import Hero from "../hp-sections/hero.svelte";
  import CaseStudy from "../hp-sections/case-study.svelte";

  let case_studies = [
    {
      title: "Box Office News!",
      subtitle: "Stay updated with the latest box office trends.",
      button_text: "Get Started",
    },
    {
      title: "Tech Innovations",
      subtitle: "Explore the latest in tech advancements.",
      button_text: "Learn More",
    },
  ];
</script>

<Hero />
{#each case_studies as study}
  <CaseStudy {...study} />
{/each}
<div class="text-center py-8">
  <button class="btn btn-primary uppercase">See Our Work</button>
</div>
