<script lang="ts">
	import { browser } from "$app/environment";
    import {darkmode} from "$lib/stores/darkmode";
    import Footer from "./footer.svelte";
    import "../app.css";
</script>
<div>

    <main> 
        <slot />
    </main>

    <Footer />
</div>