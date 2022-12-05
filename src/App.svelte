<!-- npm run dev to start app -->
<script>
  // app is composed from components which are imported here
  // self contained blocks of code with HTML/CSS/JS

  //tutorial components
  import Hello from "./lib/Hello.svelte";
  import Kitty from "./lib/Kitty.svelte";
  import Sparkle from "./lib/Sparkle.svelte";
  import HTML from "./lib/HTML.svelte";
  import Array from "./lib/Array.svelte";
  import Secret from "./lib/Secret.svelte"

  import Counter from "./lib/Counter.svelte";

  //tip calculator
  import Calculator from "./lib/Calculator.svelte";
</script>

<!-- app markup -->

<main>
  <!-- tip calculator -->
  <div class="card">
    <Calculator />
  </div>

  <div class="card">
    <Counter />
  </div>

  <!-- svelt.dev tutorials -->
  <div class="card">
    <Hello />
  </div>

  <div class="card">
    <Kitty />
  </div>

  <div class="card">
    <Sparkle />
    <p>this is another paragraph</p>
  </div>

  <div class="card">
    <HTML />
  </div>

  <div class="card">
    <Array />
  </div>

  <div class="card">
    <Secret answer={'420'} />
    <!-- without an answer prop, it defailts to 'a secret' -->
    <Secret />
  </div>
  
</main>

<style>
</style>
