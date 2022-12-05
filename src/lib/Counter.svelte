<script>
  // count is our variable
  let count = 0;

  // reactive variables stay in sync
  $: doubled = count * 2;

  // reactive statement
  $: {
    console.log("the count is " + count);
  }

  // also works with if statements
  $: if (count >= 1) {
    alert("I SAID THE COUNT IS " + count);
  }

  // also works with blocks
  $: if (count >= 10) {
    // triggers an alert if count reaches 10
    alert("count is dangerously high!");
    // the count returns to 9
    count = 9;
  }

  // event handler
  function handleClick() {
    // uhh increment lol
    count += 1;
  }
</script>

<!-- when this button is clicked, handleClick() -->
<button on:click={handleClick}>
  <!-- button is labeled with count -->
  Clicked {count}
  <!-- conditionally followed by time or times -->
  {count === 1 ? "time" : "times"}
</button>

<p>{count} doubled is {doubled}</p>
<!-- Reactive values become particularly valuable when you need to reference them multiple times, -->
<!-- or you have values that depend on other reactive values. -->
