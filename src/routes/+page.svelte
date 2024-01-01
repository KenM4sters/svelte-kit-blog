<script lang="ts">
    import * as config from "$lib/config";
    import { scrollTo, scrollRef, scrollTop } from 'svelte-scrolling'


    export let data;
</script>


<svelte:head>
    <title>{config.title}</title>
</svelte:head>

<section class="flex justify-around items-center h-[200vh]">
    <section class=" w-[100%] h-[100%] flex flex-col justify-center items-center gap-y-[10vh] relative bg-gradient-to-tr from-gray-900 to-teal-900">
        <div class=" w-[100%] flex justify-center items-center text-center">
            <div class=" w-[100%] flex flex-col justify-center items-center text-center gap-y-[10vh]">
                <h1 class="text-[5rem] font-bold text-gray-200">Welcome.</h1>
                <ul class="flex gap-x-8 ">
                    <a href="/" download="/CV.pdf"><li class=" bg-slate-500 rounded-xl hover:bg-white hover:text-black text-white w-[5vw] h-10 flex justify-center items-center transition"> Resume </li></a>
                    <a href="mailto: sam.brookman414@hotmail.com"><li class=" bg-blue-500 rounded-xl hover:bg-white hover:text-black text-white w-[5vw] h-10 flex justify-center items-center transition"> Contact </li></a>
                    <a href="https://github.com/KenM4sters"><li class=" bg-slate-800 rounded-xl hover:bg-slate-200 hover:text-black text-white w-[5vw] h-10 flex justify-center items-center transition"> Github </li></a>
                </ul>
            </div>
        </div>
        <section class=" text-gray-300  w-[100%]  items-center">
            <div class="w-[100%] flex justify-center items-center flex-col relative ">
                <div class="flex flex-col justify-center items-center w-[100%] gap-y-4 ">
                    <div class=" rounded-xl w-[75%] p-5">
                        <p class="text-[1.4rem] text-gray-300 text-center ">
                            <strong>Hi!</strong> 
                            My name is <strong>Samuel Brookman</strong>, and I'm an aspiring software developer  
                            looking to implement<br> my skills into the real world.
                            I have a passion for <strong>low level programming</strong> in <strong class="">C++</strong> and enjoy<br>
                            exploring the fields of computer graphics and <strong class="">machine learning</strong>. 
                        </p>
                    </div>
                </div>
            </div>
        </section>
        <div class="w-[100%] flex flex-col gap-y-[10vh] justify-center items-center">
        <div class="flex flex-col justify-center relative gap-y-[10vh] ">
            <div class="flex justify-center ">
                <div>
                    <h1 class="text-[3rem] font-bold text-gray-200 ">Projects</h1>
                </div>
            </div>
            <div>
                <ul class="flex justify-center items-center gap-x-[2vw] w-[100%] ">
                    <a href="#enginemk1">
                        <li class="flex flex-col justify-center  text-gray-200 items-center gap-y-4 transition-all group w-[15vw] h-[25vh] bg-cyan-950  rounded-xl  hover:bg-cyan-800 shadow-lg shadow-cyan-700">
                            <h1 class="text-[1.3rem] group  transition-all duration-1000  ">Game Engine MK1</h1>
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.0" stroke="white" class="w-[10vw] h-[10vh] group group-hover:rotate-[360deg] transition-all duration-1000">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M14.25 6.087c0-.355.186-.676.401-.959.221-.29.349-.634.349-1.003 0-1.036-1.007-1.875-2.25-1.875s-2.25.84-2.25 1.875c0 .369.128.713.349 1.003.215.283.401.604.401.959v0a.64.64 0 0 1-.657.643 48.39 48.39 0 0 1-4.163-.3c.186 1.613.293 3.25.315 4.907a.656.656 0 0 1-.658.663v0c-.355 0-.676-.186-.959-.401a1.647 1.647 0 0 0-1.003-.349c-1.036 0-1.875 1.007-1.875 2.25s.84 2.25 1.875 2.25c.369 0 .713-.128 1.003-.349.283-.215.604-.401.959-.401v0c.31 0 .555.26.532.57a48.039 48.039 0 0 1-.642 5.056c1.518.19 3.058.309 4.616.354a.64.64 0 0 0 .657-.643v0c0-.355-.186-.676-.401-.959a1.647 1.647 0 0 1-.349-1.003c0-1.035 1.008-1.875 2.25-1.875 1.243 0 2.25.84 2.25 1.875 0 .369-.128.713-.349 1.003-.215.283-.4.604-.4.959v0c0 .333.277.599.61.58a48.1 48.1 0 0 0 5.427-.63 48.05 48.05 0 0 0 .582-4.717.532.532 0 0 0-.533-.57v0c-.355 0-.676.186-.959.401-.29.221-.634.349-1.003.349-1.035 0-1.875-1.007-1.875-2.25s.84-2.25 1.875-2.25c.37 0 .713.128 1.003.349.283.215.604.401.96.401v0a.656.656 0 0 0 .658-.663 48.422 48.422 0 0 0-.37-5.36c-1.886.342-3.81.574-5.766.689a.578.578 0 0 1-.61-.58v0Z" />
                            </svg>  
                        </li>  
                    </a>
                    <a href="#api">
                        <li class="flex flex-col justify-center text-gray-200 transition-all items-center gap-y-4 group w-[15vw] h-[25vh] bg-cyan-950  rounded-xl  hover:bg-cyan-800 shadow-lg shadow-cyan-700">
                            <h1 class=" text-[1.3rem] group  transition-all duration-1000  ">API</h1>
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.0" stroke="white" class="w-[10vw] h-[10vh] group group-hover:rotate-[360deg] transition-all duration-1000">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M20.25 6.375c0 2.278-3.694 4.125-8.25 4.125S3.75 8.653 3.75 6.375m16.5 0c0-2.278-3.694-4.125-8.25-4.125S3.75 4.097 3.75 6.375m16.5 0v11.25c0 2.278-3.694 4.125-8.25 4.125s-8.25-1.847-8.25-4.125V6.375m16.5 0v3.75m-16.5-3.75v3.75m16.5 0v3.75C20.25 16.153 16.556 18 12 18s-8.25-1.847-8.25-4.125v-3.75m16.5 0c0 2.278-3.694 4.125-8.25 4.125s-8.25-1.847-8.25-4.125" />
                                </svg>  
                        </li>  
                    </a>
                    <a href="#astronomy">
                        <li class="flex flex-col justify-center text-gray-200 transition-all items-center gap-y-4 group w-[15vw] h-[25vh] bg-cyan-950  rounded-xl  hover:bg-cyan-800 shadow-lg shadow-cyan-700">
                            <h1 class=" text-[1.3rem] group  transition-all duration-1000 ">Blog</h1>
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.0" stroke="white" class="w-[10vw] h-[10vh] group group-hover:rotate-[360deg] transition-all duration-1000">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M12 7.5h1.5m-1.5 3h1.5m-7.5 3h7.5m-7.5 3h7.5m3-9h3.375c.621 0 1.125.504 1.125 1.125V18a2.25 2.25 0 0 1-2.25 2.25M16.5 7.5V18a2.25 2.25 0 0 0 2.25 2.25M16.5 7.5V4.875c0-.621-.504-1.125-1.125-1.125H4.125C3.504 3.75 3 4.254 3 4.875V18a2.25 2.25 0 0 0 2.25 2.25h13.5M6 7.5h3v3H6v-3Z" />
                                </svg>
                                
                        </li>  
                    </a>
                    <a href="#enginemk2">
                        <li class="flex flex-col justify-center text-gray-200  transition-all items-center gap-y-4 group w-[15vw] h-[25vh] bg-cyan-950  rounded-xl  hover:bg-cyan-800 shadow-lg shadow-cyan-700">
                            <h1 class=" text-[1.3rem]  group  transition-all duration-1000 ">Game Engine MK2</h1>
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.0" stroke="currentColor" class="w-[10vw] h-[10vh] group group-hover:rotate-[360deg] transition-all duration-1000">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M11.42 15.17 17.25 21A2.652 2.652 0 0 0 21 17.25l-5.877-5.877M11.42 15.17l2.496-3.03c.317-.384.74-.626 1.208-.766M11.42 15.17l-4.655 5.653a2.548 2.548 0 1 1-3.586-3.586l6.837-5.63m5.108-.233c.55-.164 1.163-.188 1.743-.14a4.5 4.5 0 0 0 4.486-6.336l-3.276 3.277a3.004 3.004 0 0 1-2.25-2.25l3.276-3.276a4.5 4.5 0 0 0-6.336 4.486c.091 1.076-.071 2.264-.904 2.95l-.102.085m-1.745 1.437L5.909 7.5H4.5L2.25 3.75l1.5-1.5L7.5 4.5v1.409l4.26 4.26m-1.745 1.437 1.745-1.437m6.615 8.206L15.75 15.75M4.867 19.125h.008v.008h-.008v-.008Z" />
                                </svg>                          
                        </li>  
                    </a>
                </ul>
            </div>
        </div>
            <div class="flex flex-col gap-y-8 justify-center w-[30vw] items-center">
                <div class="flex justify-center">
                    <div>
                        <h1 class="text-[3rem] font-bold text-gray-200 ">Skills</h1>
                    </div>
                </div>
                <div>
                    <ul class="flex justify-center flex-wrap gap-x-8 gap-y-8 ">
                        <li class=" hover:text-gray-50 text-black hover:bg-slate-500 rounded-md px-4 py-1 bg-white transition-all flex justify-center items-center  border-gray-800 shadow-sm shadow-black cursor-default "> C++ </li>
                        <li class=" hover:text-gray-50 text-black hover:bg-slate-300 rounded-md px-4 py-1 bg-white transition-all flex justify-center items-center  border-gray-800 shadow-sm shadow-black cursor-default "> C </li>
                        <li class=" hover:text-gray-50 text-black hover:bg-teal-500 rounded-md px-4 py-1 bg-white transition-all flex justify-center items-center  border-gray-800 shadow-sm shadow-black cursor-default "> Python </li>
                        <li class=" hover:text-gray-50 text-black hover:bg-red-500 rounded-md px-4 py-1 bg-white transition-all flex justify-center items-center  border-gray-800 shadow-sm shadow-black cursor-default "> Typescript </li>
                        <li class=" hover:text-gray-50 text-black hover:bg-purple-300 rounded-md px-4 py-1 bg-white transition-all flex justify-center items-center  border-gray-800 shadow-sm shadow-black cursor-default "> Arm64 ASM </li>
                        <li class=" hover:text-gray-50 text-black hover:bg-orange-300 rounded-md px-4 py-1 bg-white transition-all flex justify-center items-center  border-gray-800 shadow-sm shadow-black cursor-default "> Rust </li>
                        <li class=" hover:text-gray-50 text-black hover:bg-red-300 rounded-md px-4 py-1 bg-white transition-all flex justify-center items-center  border-gray-800 shadow-sm shadow-black cursor-default "> Vulkan </li>
                        <li class=" hover:text-gray-50 text-black hover:bg-teal-300 rounded-md px-4 py-1 bg-white transition-all flex justify-center items-center  border-gray-800 shadow-sm shadow-black cursor-default "> OpenGL </li>
                        <li class=" hover:text-gray-50 text-black hover:bg-slate-500 rounded-md px-4 py-1 bg-white transition-all flex justify-center items-center  border-gray-800 shadow-sm shadow-black cursor-default "> Git </li>
                        <li class=" hover:text-gray-50 text-black hover:bg-sky-300 rounded-md px-4 py-1 bg-white transition-all flex justify-center items-center  border-gray-800 shadow-sm shadow-black cursor-default "> Linux </li>
                        <li class=" hover:text-gray-50 text-black hover:bg-yellow-300 rounded-md px-4 py-1 bg-white transition-all flex justify-center items-center  border-gray-800 shadow-sm shadow-black cursor-default "> Blender </li>
                        <li class=" hover:text-gray-50 text-black hover:bg-blue-300 rounded-md px-4 py-1 bg-white transition-all flex justify-center items-center  border-gray-800 shadow-sm shadow-black cursor-default "> Docker </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
</section>

<section id="enginemk1" class=" bg-cyan-700 h-[50vh] items-center">
    <div class="flex justify-around h-[100%] items-center ">
        <div class="flex justify-around w-[90%]">
            <div class="text-white w-[50vw] flex flex-col gap-y-8 justify-center">
                <h1 class=" font-semibold text-[3rem]">First Game - C, OpenGL </h1>
                <p class=" "> This was my very first serious C program, as well as my first 
                    exposure to graphics APIs. Although it's really just a very simple game, everything from 
                    storing vertices to rendering bullets and handling user input is done by scratch.
                </p>
                <span class=" hover:font-semibold hover:border-b-red-500 hover:border-b transition-all w-[10vw]"> <a href={data.posts[9].slug}>Learn more here</a></span>
            </div>
            <div>
                <div class=" bg-black rounded-lg p-4">
                    <video muted width="300" height="100" autoplay loop playsinline disablepictureinpicture>
                        <source src="/game_demo.mp4" type="video/mp4"/>
                    </video>
                </div>
            </div>
        </div> 
    </div>
</section>

<section class="h-[10vh] bg-gray-950">
    <div></div>
</section>

<section id="api" class=" bg-teal-700 h-[50vh] items-center">
    <div class="flex justify-center h-[100%] items-center ">
        <div class="flex justify-around w-[90%] gap-x-[5vw]">
            <div class="">
                <div class="bg-black rounded-lg p-4">
                    <img height="100" width="300" alt="" src="api.png"  />
                </div>
            </div>
            <div class="text-black flex flex-col justify-center gap-y-8 w-[60vw] ">
                <h1 class="font-semibold text-[3rem]">Rest API - Rust, PostgreSQL </h1>
                <p class=""> Continuous development in C inspired me to explore into other low-level technologies, namely 
                    Arm64 Assembly and Rust. Given its almost unrivaled speed and memory safety, I figured it would 
                    be as good of a time as any to write my own Rest API using Rust, Actix Web and PostgreSQL, among other 
                    technologies such as Docker.       
                </p>
                <span class=" hover:font-semibold hover:border-b-red-500 hover:border-b transition-all w-[10vw]"> <a href={data.posts[0].slug}>Learn more here</a></span>
            </div>
        </div>
    </div>
</section>

<section class="h-[10vh] bg-gray-950">
    <div></div>
</section>

<section id="enginemk2" class=" bg-blue-500 h-[50vh]  items-center">
    <div class="flex justify-center h-[100%] items-center ">
        <div class="flex justify-center w-[90%] gap-x-[5vw]">
            <div class="text-white flex flex-col justify-center gap-y-8 w-[60vw]">
                <h1 class="font-semibold text-[3rem]">Game Engine - C++, Vulkan </h1>
                <p class=""> My most recent and largest project to date, developing a 3D game engine 
                    using C++ and the Vulkan API has been extremely interesting, exciting and yet challenging
                    at the same time. Both technologies are known for having a steep learing-curve, and that's
                    with good reason I feel. <br><br> Being able to combine my passion for Mathematics, low-level programming
                    and 3D graphics has resulted in a project that's both fun and rewarding
                </p>
                <span class=" hover:font-semibold hover:border-b-red-500 hover:border-b transition-all w-[10vw]"> <a href={data.posts[10].slug}>Learn more here</a></span>
            </div>
            <div>
                <div class="bg-black rounded-lg p-4 relative top-[10%]">
                    <video muted width="300" height="100" autoplay loop playsinline disablepictureinpicture>
                        <source src="/engine_mkvi_demo.mov" type="video/mp4"/>
                    </video>
                </div>
            </div>
        </div>
    </div>
</section>

<section class="h-[10vh] bg-gray-950">
    <div></div>
</section> 

<section id="astronomy" class=" text-gray-300 bg-gradient-to-tr from-teal-800 to-cyan-950 p-[10vh] pt-[5vh]">
    <div class="flex justify-center items-center ">
        <div class="flex justify-center items-center flex-col w-[75vw] mt-[10vh]">
            <div class=" flex flex-col justify-center text-center items-center gap-y-[5vh] ">
                <div>
                    <h1 class="text-[3rem] font-bold text-gray-200 ">Astronomy</h1>
                </div>
                <p class="text-[1.4rem] text-gray-300 text-center ">
                    Aside from computer programming, one of my primiary interests is <strong>astrophysics.</strong>
                    Many years ago,<br> I started writing down everything that I had learned from watching 
                    youtube videos and decided<br> it would be an ample opportunity to explore <strong>frontend 
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


