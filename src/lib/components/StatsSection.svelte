<script lang="ts">
  const stats = [
    {
      label: "$50B Ops Market",
      desc: "We're capturing a massive opportunity—the operational systems market for startups. Founders spend billions on full-time COOs or struggle alone. Vira delivers the same impact at a fraction of the cost through our fractional model.",
      img: "https://images.unsplash.com/photo-1551288049-bebda4e38f71?auto=format&fit=crop&q=80&w=200"
    },
    {
      label: "YC Office Hours",
      desc: "We reach overwhelmed founders where they are—through Y Combinator office hours, startup communities, and direct referrals. Our go-to-market strategy focuses on building trust with founders who need help now.",
      img: "https://images.unsplash.com/photo-1560179707-f14e90ef3623?auto=format&fit=crop&q=80&w=200"
    },
    {
      label: "Fractional Model",
      desc: "No full-time overhead, no equity dilution. Our embedded fractional COO model gives you immediate operational capacity without the commitment of a full-time hire. Scale up or down as you grow.",
      img: "https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?auto=format&fit=crop&q=80&w=200"
    },
    {
      label: "Founder-Led",
      desc: "Led by Mateo Costa (CEO) and Agustin Campos (Strategy Director), Vira is built by operators who understand the chaos of early-stage startups. We've been in your shoes—and we know what it takes to scale.",
      img: "https://images.unsplash.com/photo-1519085360753-af0119f7cbe7?auto=format&fit=crop&q=80&w=200"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white border-t border-gray-100">
  <div class="mb-16">
    <p class="text-gray-500 max-w-xl">
      Here's what makes Vira different—our approach, our model, and the opportunity we're capturing.
    </p>
  </div>

  <div class="space-y-16">
    {#each stats as stat}
      <div class="flex flex-col md:flex-row md:items-start justify-between gap-8 border-b border-gray-100 pb-16 last:border-0">
        <h3 class="text-2xl md:text-4xl font-medium w-full md:w-1/3">{stat.label}</h3>
        <div class="w-full md:w-1/3">
           <p class="text-xs leading-relaxed text-gray-500">{stat.desc}</p>
        </div>
        <div class="w-full md:w-1/6 flex justify-end">
           <img src={stat.img} alt={stat.label} class="w-20 h-20 object-cover rounded bg-gray-100" />
        </div>
      </div>
    {/each}
  </div>
</section>
