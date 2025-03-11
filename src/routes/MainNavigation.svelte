<script lang="ts">
  import LanguageSwitcher from "./LanguageSwitcher.svelte"
  import MainNavigationLink from "./MainNavigationLink.svelte"
</script>

<nav class="flex h-[70px] flex-row items-center">
  <div class="flex flex-grow flex-row items-center gap-x-2">
    <a class="flex flex-row items-center gap-x-2" href="/" aria-label="Clipboard X home">
      <img
        src="/clipboardx.png"
        fetchpriority="high"
        decoding="async"
        class="inline"
        alt="Clipboard X app icon"
        height="32"
        width="32"
      />
      <span class="text-base font-semibold text-neutral-900">Clipboard X</span>
    </a>
  </div>
  <div class="flex flex-row items-center gap-x-8 pr-4 sm:pr-0">
    <!-- <LanguageSwitcher /> -->
    <ul class="flex flex-row items-center gap-x-8">
      <li>
        <MainNavigationLink href="/" text="Home" />
      </li>
      <li>
        <MainNavigationLink href="/about" text="About" />
      </li>
      <li>
        <MainNavigationLink href="/contact" text="Contact" />
      </li>
    </ul>
  </div>
</nav>
