<script>
    let cat = { fed: false };

    function toggle() {
        cat.fed = !cat.fed;
    }
</script>

<!-- HTML doesn't have a way of expressing logic, like conditionals and loops. Svelte does. -->
<!-- To conditionally render some markup, we wrap it in an if block: -->
{#if cat.fed} <!-- A # character always indicates a block opening tag. -->
    <button on:click={toggle}> cat fed </button>
    <!-- since the conditions are mutually exclusive, we can use an else block -->
{:else} <!--  A : character, as in {:else}, indicates a block continuation tag. -->
    <button on:click={toggle}> feed cat </button>
{/if} <!-- A / character always indicates a block closing tag. -->
