<script lang="ts">
    import * as config from "$lib/config";
</script>

<header class="flex justify-center z-10 top-0 inset-x-0 border-b">
    <nav class="flex items-center justify-between max-w-5xl mx-auto px-4 h-24 gap-20">
        <h1 class="text-red-500"> 
            <a href="/">{config.title}</a>
        </h1>
        <div class="flex space-x-1 items-center">
            <a 
            class="p-2 rounded-lg text-gray-700 hover:bg-gray-100" 
            target="_blank"
            href="https://github.com/KenM4sters">
            Github
            </a>
        </div>
    </nav>
</header>