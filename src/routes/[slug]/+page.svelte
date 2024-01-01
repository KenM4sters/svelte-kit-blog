<script lang="ts">
    export let data;
</script>

<svelte:head>
    <title>{data.meta.title}</title>
    <meta property="og:type" content="article" />
    <meta property="og:title" content={data.meta.title} />
</svelte:head>

<section class="bg-gradient-to-tr from-gray-900 to-teal-900">
    <section class="flex justify-center items-center h-[30vh] ">
        <div class="flex justify-center items-center">
            <button class=" bg-slate-200 text-slate-600 hover:bg-red-600 hover:text-white transition-all rounded-lg p-3"><a href="./"> Return To Home </a></button>
        </div>
    </section>
    
    
    <article class="flex-col justify-center ml-[25%] mt-10 pb-[20vh] ">
        <hgroup>
            <h1 class="font-semibold text-[2rem] pb-5 text-gray-200">{data.meta.title}</h1>
            <p class="text-red-800"> Published at: {data.meta.date}</p>
        </hgroup>
        
        <div class="tags text-gray-200 pt-5">
            {#each data.meta.categories as category}
            <span class="text-gray-200">&num; {category}</span>
            {/each}
        </div>
        
        <div class="prose prose-lg text-gray-300">
            <svelte:component this={data.content} />
        </div>
    </article>
</section>