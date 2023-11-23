<script lang="ts">
	import { browser } from "$app/environment";
    import {darkmode} from "$lib/stores/darkmode";
    import Header from "./header.svelte";
    import Footer from "./footer.svelte";
    import "../app.css";
</script>
<div>
    <Header />
    
    <main> 
        <slot />
    </main>

    <Footer />
</div>