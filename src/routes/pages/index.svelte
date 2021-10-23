<script context="module" lang="ts">
  export const prerender = true;
</script>

<script lang="ts">
  import { page } from "$app/stores";
</script>

<li class:active={$page.path === "/pages/firefox"}>
  <a sveltekit:prefetch href="/pages/firefox">Firefox</a>
</li>
