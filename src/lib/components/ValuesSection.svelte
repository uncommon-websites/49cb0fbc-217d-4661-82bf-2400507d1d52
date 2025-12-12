<script lang="ts">
  const testimonials = [
    {
      name: "Liesbeth Rector",
      role: "HR Advisor & Recruiter",
      quote: "Judith has the ability to bring out the best in people. In a friendly way she asks critical questions, analyzes and points out the 'common thread' in your life course.",
      img: "https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?auto=format&fit=crop&q=80&w=400"
    },
    {
      name: "Jan",
      role: "Mid-Career Professional, 50",
      quote: "Through her professional approach and personal empathy in my situation, she helped me discover new opportunities and stimulated possibilities to develop myself.",
      img: "https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?auto=format&fit=crop&q=80&w=400"
    },
    {
      name: "Anita Vilé – van der Lee",
      role: "Team Coordinator, Mercedes Benz",
      quote: "She shows integrity and demonstrates empathy, people skills and expertise. She makes you think, but above all she is very pleasant to work with.",
      img: "https://images.unsplash.com/photo-1580489944761-15a19d654956?auto=format&fit=crop&q=80&w=400"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-xl mb-16">
    <h3 class="text-lg font-bold mb-2">What our clients say</h3>
    <p class="text-gray-500 text-sm leading-relaxed">
      Real transformations from professionals who found clarity, direction, and renewed energy in their careers through our coaching and development programs.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each testimonials as testimonial}
      <div>
        <div class="aspect-[3/4] rounded-lg overflow-hidden mb-4 bg-gray-100">
          <img src={testimonial.img} alt={testimonial.name} class="w-full h-full object-cover grayscale" />
        </div>
        <h4 class="text-xs font-bold mb-1">{testimonial.name}</h4>
        <p class="text-[10px] text-gray-400 mb-2">{testimonial.role}</p>
        <p class="text-[11px] text-gray-600 leading-relaxed italic">"{testimonial.quote}"</p>
      </div>
    {/each}
  </div>
</section>
