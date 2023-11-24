<script lang="ts">
    export let data;
</script>

<svelte:head>
    <title>{data.meta.title}</title>
    <meta property="og:type" content="article" />
    <meta property="og:title" content={data.meta.title} />
</svelte:head>

<article class="flex-col justify-center ml-[25%] mt-10 mb-10">
    <hgroup>
        <h1 class="font-semibold text-[2rem] pb-10">{data.meta.title}</h1>
        <p> Published at: {data.meta.date}</p>
    </hgroup>
    
    <div class="tags">
        {#each data.meta.categories as category}
        <span>&num; {category}</span>
        {/each}
    </div>
    
    <div class="prose prose-lg text-black">
        <svelte:component this={data.content} />
    </div>
</article>