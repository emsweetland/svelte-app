<script>
	let cats = [
		{ id: 'J---aiyznGQ', name: 'Keyboard Cat' },
		{ id: 'z_AbfPXTKms', name: 'Maru' },
		{ id: 'OUtn3pvWmpg', name: 'Henri The Existential Cat' }
	];
</script>

<h1>The Famous Cats of YouTube</h1>

<ul>
	{#each cats as { id, name }, i}
		<li><a target="_blank" href="https://www.youtube.com/watch?v={id}" rel="noreferrer">
			{i + 1}: {name}
		</a></li>
	{/each}
</ul>

<!-- If you need to loop over lists of data, use an each block:

The expression (cats, in this case) can be any array or array-like object (i.e. it has a length property). 
You can loop over generic iterables with each [...iterable].

If you prefer, you can use destructuring — each cats as { id, name } — 
and replace cat.id and cat.name with id and name. -->