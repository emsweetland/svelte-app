<script>
	let cash = 1;
	let card = 2;
    $: tips = cash + card;
</script>


<label>
    <p>cash</p>
	<input type=number bind:value={cash} >

</label>

<label>
    <p>card</p>
	<input type=number bind:value={card} >

</label>


<p>tip total</p>
<p>{tips}</p>



<style>
	label { display: flex }
	input, p { margin: 6px }
</style>