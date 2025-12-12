<script lang="ts">
  import Header from "$lib/components/Header.svelte";
  import HiringHero from "$lib/components/hiring/HiringHero.svelte";
  import HiringBenefits from "$lib/components/hiring/HiringBenefits.svelte";
  import HiringProcess from "$lib/components/hiring/HiringProcess.svelte";
  import HiringCTA from "$lib/components/hiring/HiringCTA.svelte";
  import Footer from "$lib/components/Footer.svelte";
  import FloatingNav from "$lib/components/FloatingNav.svelte";
</script>

<main class="font-sans antialiased text-black bg-white selection:bg-purple-200 selection:text-purple-900">
  <Header />
  <HiringHero />
  <HiringBenefits />
  <HiringProcess />
  <HiringCTA />
  <Footer />
  <FloatingNav />
</main>
