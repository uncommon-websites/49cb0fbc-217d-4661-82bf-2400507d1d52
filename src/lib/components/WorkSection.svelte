<script lang="ts">
  const services = [
    {
      name: "Individual Coaching",
      desc: "One-on-one career development, leadership coaching, and personal growth journeys tailored to your unique situation.",
      bg: "bg-gray-100",
      img: "https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?auto=format&fit=crop&q=80&w=800",
      dark: false
    },
    {
      name: "Insights Discovery Profile",
      desc: "Discover your natural talents and working style through our certified personality profiling system. From €205.",
      bg: "bg-gradient-to-br from-[oklch(0.696_0.17_162.48)] to-[oklch(0.508_0.118_165.612)]",
      img: "https://images.unsplash.com/photo-1434030216411-0b793f4b4173?auto=format&fit=crop&q=80&w=800",
      dark: true
    },
    {
      name: "Team Training",
      desc: "Custom programs designed for team growth, collaboration, and unlocking collective potential.",
      bg: "bg-gray-100",
      img: "https://images.unsplash.com/photo-1552664730-d307ca884978?auto=format&fit=crop&q=80&w=800",
      dark: false
    },
    {
      name: "Career Program",
      desc: "15-week group program 'More Shine and Energy in Your Career' - A structured 10-step journey to career clarity.",
      bg: "bg-black",
      img: "https://images.unsplash.com/photo-1522202176988-66273c2fd55f?auto=format&fit=crop&q=80&w=800",
      dark: true
    },
    {
      name: "Management Development",
      desc: "Strategic L&D trajectories with ongoing structure and follow-up for lasting leadership impact.",
      bg: "bg-gray-50",
      img: "https://images.unsplash.com/photo-1542744173-8e7e53415bb0?auto=format&fit=crop&q=80&w=800",
      dark: false,
      full: true
    },
    {
      name: "Development Conversations",
      desc: "Training for meaningful career conversations that drive growth and engagement. Open training from €495.",
      bg: "bg-gray-100",
      img: "https://images.unsplash.com/photo-1556761175-b413da4baf72?auto=format&fit=crop&q=80&w=800",
      dark: false
    },
    {
      name: "Custom L&D Programs",
      desc: "Flexible formats: 1-on-1, online, in-company, hybrid, and e-learning solutions tailored to your organization.",
      bg: "bg-gray-100",
      img: "https://images.unsplash.com/photo-1531482615713-2afd69097998?auto=format&fit=crop&q=80&w=800",
      dark: false
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-white">
  <div class="max-w-3xl mb-16">
    <h2 class="text-2xl md:text-3xl font-medium leading-tight">
      <span class="font-bold">We combine soft skills expertise with strategic business insight</span> to help professionals discover and leverage their natural talents for more energy, satisfaction, and success in their careers.
    </h2>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-2 gap-x-6 gap-y-12">
    {#each services as service}
      <div class="group cursor-pointer {service.full ? 'md:col-span-2' : ''}">
        <div class={`aspect-[4/3] w-full rounded-lg overflow-hidden relative ${service.bg} mb-4 ${service.full ? 'md:aspect-[2.5/1]' : ''}`}>
          {#if service.img}
             <img src={service.img} alt={service.name} class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
          {:else}
             <div class="w-full h-full flex items-center justify-center">
                <span class={`text-2xl font-bold ${service.dark ? 'text-white' : 'text-black'}`}>{service.name}</span>
             </div>
          {/if}
        </div>
        <h3 class="text-sm font-bold mb-1">{service.name}</h3>
        <p class="text-sm text-gray-600">{service.desc}</p>
      </div>
    {/each}
  </div>
</section>
