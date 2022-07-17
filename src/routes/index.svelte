<script>
  import { onMount } from 'svelte';
  import { gsap } from 'gsap';

  let text1;
  let text2;

  onMount(() => {
    gsap.from(text1, {
      x: -100,
      opacity: 0,
      duration: 1.5,
      ease: "power1.out",
    })
    gsap.from(text2, {
      x: -200,
      opacity: 0,
      duration: 1.5,
      ease: "power1.out",
    })
  })
</script>

<section class="greeting">
  <div class="greeting-text">
    <h1 bind:this="{text1}">Hey there! 👋</h1>
    <p bind:this="{text2}">I'm Vladislav, a fullstack developer</p>
  </div>
  <div class="greeting-image">
    greeting-image
  </div>
</section>
<section class="about">
  about
</section>
<section class="work">
  work
</section>