<script lang="ts">
    export let data;
</script>

<svelte:head>
    <title>{data.meta.title}</title>
    <meta property="og:type" content="article" />
    <meta property="og:title" content={data.meta.title} />
</svelte:head>

<article>
    <hgroup>
        <h1>{data.meta.title}</h1>
        <p> Published at: {data.meta.date}</p>
    </hgroup>
    
    <div class="tags">
        {#each data.meta.categories as category}
        <span>&num; {category}</span>
        {/each}
    </div>
    
    <div class="prose ">
        <svelte:component this={data.content} />
    </div>
</article>