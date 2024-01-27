<script lang="ts">
    export let data;
</script>

<svelte:head>
    <title>{data.meta.title}</title>
    <meta property="og:type" content="article" />
    <meta property="og:title" content={data.meta.title} />
</svelte:head>

<section id="article-wrapper">
    <section class="flex justify-center items-center h-[30vh] ">
        <div class="flex justify-center items-center">
            <button class=" bg-slate-200 text-slate-600 hover:bg-cyan-600 hover:text-white transition-all duration-500 rounded-lg p-3"><a href="./"> Return To Home </a></button>
        </div>
    </section>
    
    
    <article id="article page" class="flex-col justify-center ml-[25%] mt-10 pb-[20vh]">
        <hgroup>
            <h1 class="font-semibold text-[2rem] pb-5 text-gray-300">{data.meta.title}</h1>
            <p class="text-cyan-500"> Published at: {data.meta.date}</p>
        </hgroup>
        
        <div class="tags text-indigo-700 pt-5">
            {#each data.meta.categories as category}
            <span> &num; {category}</span>
            {/each}
        </div>
        
        <div class="prose prose-lg text-gray-300">
            <svelte:component this={data.content} />
        </div>
    </article>
</section>