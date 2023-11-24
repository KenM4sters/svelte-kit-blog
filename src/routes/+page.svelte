<script lang="ts">
    import * as config from "$lib/config";

    export let data;
</script>

<svelte:head>
    <title>{config.title}</title>
</svelte:head>

<section class="mt-8">
    <ul class="posts flex justify-center gap-x-8 h-[500vh] flex-wrap">
        {#each data.posts as post }
        <a href={post.slug} class=" h-[40vh] ">
            <li class="post bg-slate-50 w-[20vw] border border-slate-100 h-[100%] p-4 hover:bg-slate-300 transition-colors rounded-md ">
                <p class="title text-[1.5rem] pb-2 ">{post.title}</p>
                <p class="date pb-2">{post.date}</p>
                <p class="description">{post.description}</p>
            </li>
        </a>
        {/each} 
    </ul>
</section>
