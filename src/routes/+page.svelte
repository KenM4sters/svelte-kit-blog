<script lang="ts">
    import * as config from "$lib/config";

    export let data;
</script>

<svelte:head>
    <title>{config.title}</title>
</svelte:head>

<section>
    <ul class="posts flex justify-center gap-4 h-[100vh]">
        {#each data.posts as post }
        <li class="post w-[20vw] text-lg border h-[40vh]">
            <a href={post.slug} class="title">{post.title}</a>
            <p class="date">{post.date}</p>
            <p class="description">{post.description}</p>
        </li>
        {/each}
    </ul>
</section>
