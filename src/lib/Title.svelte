<script lang="ts">
    export let t: string | string[] = "";
    if(Array.isArray(t)) {
        t = t.join(" • ");
    }
</script>

<svelte:head>
    <title>{t} | WhateverDSP</title>
</svelte:head>