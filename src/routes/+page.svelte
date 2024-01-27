<script lang="ts">
    import * as config from "$lib/config";

    export let data;
</script>

<svelte:head>
    <title>{config.title}</title>
</svelte:head>
  


<section id="astronomy" class=" text-gray-300 p-[10vh] pt-[5vh]">
    <section class="flex justify-around items-center ">
        <div id="update-wrapper" class="flex flex-col justify-center items-center gap-5  p-10 rounded-xl">
            <h1 class=" text-[4rem] font-bold"> Update! </h1>
            <p>If you're visiting to see my portfolio, then please follow the link below.</p>
            <a href="https://portfolio-2024-bz5uhqereq-nw.a.run.app" target="_blank" class=" underline hover:text-cyan-400 transition-all duration-500">click here</a>
            <p>Many thanks, and I apologise for the inconveniance.</p>
        </div>
    </section> 
    <div class="flex justify-center items-center ">
        <div class="flex justify-center items-center flex-col w-[75vw] mt-[10vh]">
            <div class=" flex flex-col justify-center text-center items-center gap-y-[5vh] ">
                <div>
                    <h1 class="text-[3rem] font-bold text-gray-200 ">Astronomy</h1>
                </div>
                <p class="text-[1.2rem] text-gray-300 text-center ">
                    Aside from computer programming, one of my primiary interests is <strong>astrophysics.</strong>
                    Many years ago,<br> I started writing down everything that I had learned from reading books and watching 
                    free youtube videos and decided it would be an ample opportunity to explore <strong>frontend 
                        technologies,</strong><br> with the aim to put together a neat little blog. 
                </p>
                <span class=" hover:font-semibold hover:border-b-red-500 hover:border-b transition-all w-[10vw]"> <a href={data.posts[6].slug}>Learn more here</a></span>
            </div>
        </div>
    </div>
    <section class="mt-[10vh]">
        <ul class="posts flex justify-center gap-x-8 gap-y-10 flex-wrap">
            {#each data.posts as post }
            <a href={post.slug} class="h-[16rem]">
                <li class="post bg-slate-300 w-[15rem] h-[100%] p-4 hover:bg-sky-50  transition-colors rounded-md text-black">
                    <p class="title font-bold text-[1.1rem] pb-2 ">{post.title}</p>
                    <p class="date pb-2">{post.date}</p>
                    <p class="description">{(post.description).substring(0, 90).concat("...")}</p>
                </li>
            </a>
            {/each} 
        </ul>
    </section>
</section>


