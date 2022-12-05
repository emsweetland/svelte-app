<script>
	let string = `this string contains some <strong>HTML!!!</strong>`;
</script>

<!-- strings inserted as plain text mean < and > have no special meaning -->
<p>{string}</p>

<!-- to render HTML directly into a component, use the {@html ...} tag -->
<p>{@html string}</p>

<!-- Svelte doesn't perform any sanitization of the expression inside {@html ...} before it gets inserted into the DOM.  -->
<!-- In other words, if you use this feature it's critical that you manually escape HTML that comes from sources you don't trust,  -->
<!-- otherwise you risk exposing your users to XSS attacks. -->