<p>this is a paragraph</p>

<!-- <style> tag rules are scoped to the component. You won't accidentally change the style of <p> elements elsewhere in your app -->
	<!-- styles from App.svelte don't leak in -->
<style>
	p {
		color: rgb(115, 163, 101);
		font-family: 'Comic Sans MS', cursive;
		font-size: 2em;
	}
</style>