<script lang="ts">
  import { i18n } from "$lib/i18n"
  import { ParaglideJS } from "@inlang/paraglide-sveltekit"
  import "../app.css"
  import MainNavigation from "./MainNavigation.svelte"
  let { children } = $props()
</script>

<ParaglideJS {i18n}>
  <div class="mx-auto px-4 sm:px-8 md:max-w-6xl lg:max-w-7xl">
    <MainNavigation />
    {@render children()}
  </div>
</ParaglideJS>
