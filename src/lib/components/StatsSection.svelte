<script lang="ts">
  const stats = [
    {
      label: "25+ Years Experience",
      desc: "Judith Manssen brings over 25 years of expertise in human development, combining backgrounds as a creative therapist, business economist, and reintegration consultant. As a Noloc certified register career coach and Insights Discovery practitioner, she has witnessed firsthand the cost of underutilized talent and is driven to help professionals unlock their potential.",
      img: "https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?auto=format&fit=crop&q=80&w=200"
    },
    {
      label: "Insights Discovery Certified",
      desc: "We're certified practitioners of the Insights Discovery personality profiling system, a powerful tool that helps individuals understand their natural working style, communication preferences, and unique strengths. This methodology forms the foundation of our talent discovery approach.",
      img: "https://images.unsplash.com/photo-1434030216411-0b793f4b4173?auto=format&fit=crop&q=80&w=200"
    },
    {
      label: "10+ Major Clients",
      desc: "Trusted by leading Dutch organizations including Waternet, Hoogheemraadschap Delfland, Kwik Fit, Mercedes Benz Global Training Nederland, HAN, and more. We specialize in working with organizations of 50 to 1,500 employees, delivering measurable talent development outcomes.",
      img: "https://images.unsplash.com/photo-1542744173-8e7e53415bb0?auto=format&fit=crop&q=80&w=200"
    },
    {
      label: "Flexible Delivery",
      desc: "We meet you where you are with versatile formats: 1-on-1 coaching, online programs, in-company training, hybrid solutions, and e-learning. Our approach emphasizes learning as a continuous process rather than one-off events, combining training, coaching, and strategic advice for lasting impact.",
      img: "https://images.unsplash.com/photo-1516321318423-f06f85e504b3?auto=format&fit=crop&q=80&w=200"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white border-t border-gray-100">
  <div class="mb-16">
    <p class="text-gray-500 max-w-xl">
      Built on decades of experience and proven methodology, MPMC helps mid-career professionals transform their careers through structured talent discovery.
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
