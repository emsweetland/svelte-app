<!-- npm run dev to start app -->
<script>
  // app is composed from components which are imported here
  // self contained blocks of code with HTML/CSS/JS

  //tutorial components
  import Hello from "./lib/Hello.svelte";
  import Kitty from "./lib/Kitty.svelte";
  import Sparkle from "./lib/Sparkle.svelte";
  import HTML from "./lib/HTML.svelte";
  import Counter from "./lib/Counter.svelte";
  import Array from "./lib/Array.svelte";
  import Secret from "./lib/Secret.svelte";
  import Info from "./lib/SpreadProps/SpreadInfo.svelte";
  import CatFood from "./lib/CatFood.svelte";
  import Loop from "./lib/Loop.svelte";
  import Key from "./lib/BlockKeyLoops/Key.svelte";
  
</script>

<!-- app markup -->

<main>

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
    <Counter />
  </div>

  <div class="card">
    <Array />
  </div>

  <div class="card">
    <Secret answer={'420'} />
    <!-- without an answer prop, it defailts to 'a secret' -->
    <Secret />
  </div>

  <div class="card">
    <Info />
  </div>

  <div class="card">
    <CatFood />
  </div>

  <div class="card">
    <Loop />
  </div>

  <div class="card">
    <Key />
  </div>
  
</main>

<style>
</style>
