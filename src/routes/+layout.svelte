<script lang="ts">
	import "../app.css";
	import * as Sidebar from "$lib/components/ui/sidebar/index.js";
	import AppSidebar from "$lib/components/app-sidebar.svelte";
    import { ModeWatcher } from "mode-watcher";

	let { children } = $props();
</script>

<ModeWatcher/>
<Sidebar.Provider>
<AppSidebar />
<Sidebar.Inset>
<div class="flex h-screen flex-col">
	{@render children?.()}
</div>
</Sidebar.Inset>
</Sidebar.Provider>
