<script lang="ts">
    import Logo from "$lib/svg/Logo.svelte";
</script>

<header>
    <div class="Logo">
        <Logo />
    </div>
    <menu>
        <li>
            <a href="/">Home</a>
        </li>
        <li>
            <a href="/library">Library</a>
        </li>
        <li>
            <a href="/hardware">Hardware</a>
        </li>
    </menu>
</header>

<style>
    header {
        display: flex;
        justify-content: start;
        gap: 2rem;
        align-items: center;
        padding: 1rem;
        border-bottom: 1px solid var(--border);
        background: var(--bg);
    }
    .Logo {
        height: 1rem;
    }
    .Logo :global(svg) {
        fill: var(--text);
    }
    menu {
        display: flex;
        gap: 1rem;
        margin: 0;
        padding: 0;
        list-style: none;
    }
    a {
        font-weight: bold;
    }
</style>