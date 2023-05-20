<script lang="ts">
  import Theme from '$lib/Theme.svelte';
	import '$lib/style.css';
    import Header from "./Header.svelte";
</script>

<Theme>
    <main>
        <Header />
        <slot />
    </main>
</Theme>

<style>
    main {
        display: grid;
        grid-template-rows: auto 1fr;
    }
</style>