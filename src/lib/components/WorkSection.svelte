<script lang="ts">
  const projects = [
    {
      client: "Revenue Operations",
      desc: "Built scalable systems from chaotic spreadsheets to predictable growth.",
      bg: "bg-gray-950",
      img: "", // Placeholder logic handled in template
      dark: true
    },
    {
      client: "Team Structure",
      desc: "Designed org charts and hiring roadmaps for rapid scaling.",
      bg: "bg-gray-200",
      img: "https://images.unsplash.com/photo-1552664730-d307ca884978?auto=format&fit=crop&q=80&w=800",
      dark: false
    },
    {
      client: "Process Automation",
      desc: "Eliminated bottlenecks with workflow systems that save 20+ hours weekly.",
      bg: "bg-primary-950",
      img: "https://images.unsplash.com/photo-1460925895917-afdab827c52f?auto=format&fit=crop&q=80&w=800",
      dark: true
    },
    {
      client: "Financial Planning",
      desc: "Created budget models and KPI dashboards for investor-ready reporting.",
      bg: "bg-black",
      img: "",
      dark: true
    },
    {
      client: "Go-to-Market Strategy",
      desc: "Launched products with clear positioning and execution frameworks.",
      bg: "bg-[#f0f0f0]",
      img: "https://images.unsplash.com/photo-1557804506-669a67965ba0?auto=format&fit=crop&q=80&w=800",
      dark: false,
      full: true
    },
    {
      client: "Customer Success",
      desc: "Built onboarding systems that increased retention by 40%.",
      bg: "bg-[#e0e0e0]",
      img: "https://images.unsplash.com/photo-1573164713714-d95e436ab8d6?auto=format&fit=crop&q=80&w=800",
      dark: false
    },
    {
      client: "OKR Framework",
      desc: "Implemented goal-setting systems that aligned teams and accelerated execution.",
      bg: "bg-primary-100",
      img: "https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?auto=format&fit=crop&q=80&w=800",
      dark: false
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-white">
  <div class="max-w-3xl mb-16">
    <h2 class="text-2xl md:text-3xl font-medium leading-tight">
      <span class="font-bold">We build operational systems that scale</span> so you can focus on what matters—leading your company, not managing chaos.
    </h2>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-2 gap-x-6 gap-y-12">
    {#each projects as project}
      <div class="group cursor-pointer {project.full ? 'md:col-span-2' : ''}">
        <div class={`aspect-[4/3] w-full rounded-lg overflow-hidden relative ${project.bg} mb-4 ${project.full ? 'md:aspect-[2.5/1]' : ''}`}>
          {#if project.img}
             <img src={project.img} alt={project.client} class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
          {:else}
             <!-- Placeholder for logos on solid bg -->
             <div class="w-full h-full flex items-center justify-center">
                <span class={`text-2xl font-bold ${project.dark ? 'text-white' : 'text-black'}`}>{project.client} Logo</span>
             </div>
          {/if}
        </div>
        <h3 class="text-sm font-bold mb-1">{project.client}</h3>
        <p class="text-sm text-gray-600">{project.desc}</p>
      </div>
    {/each}
  </div>
</section>
