<script lang="ts">
  import { renderSymbols } from "$lib/symbols"
  import FeatureSection from "./FeatureSection.svelte"
</script>

<svelte:head>
  <title>Clipboard X - Paste like a Pro</title>
</svelte:head>

<main>
  <section
    id="hero"
    class="hero flex flex-col items-center justify-center pt-12 text-center sm:pt-28"
  >
    <div class="flex justify-center">
      <div class="w-32 sm:w-48">
        <img
          src="/clipboardx.png"
          fetchpriority="high"
          decoding="async"
          alt="ClipboardX app icon"
          height="1200"
          width="1200"
        />
      </div>
    </div>

    <h1 class="mt-8 text-4xl font-bold text-neutral-900 sm:text-5xl lg:text-6xl">Clipboard X</h1>
    <p class="mt-6 text-lg font-normal text-neutral-500 sm:text-2xl">
      Copy and paste like never before
    </p>
    <div class="mt-8 max-w-sm">
      <button
        style="background:radial-gradient(at bottom, rgba(50,50,50,1) 0%, rgba(10,10,10,1) 100%)"
        class="relative w-full rounded-xl border-b-[6px] border-b-black shadow-xl transition-all select-none hover:-translate-y-[1px] hover:shadow-2xl active:translate-y-[4px] active:border-b-2 active:shadow-md"
      >
        <div
          class="w-full rounded-xl border-t-1 border-b-[1px] border-t-white/30 border-b-white/20 px-6 py-4 text-center text-lg font-medium text-white shadow-inner active:border-b-0 active:border-t-black"
        >
          Download for Mac
        </div>
      </button>
    </div>
    <p class="mt-6 text-sm font-light text-neutral-500">macOS 12.3+</p>
    <div class="mt-16 w-full max-w-6xl">
      <video
        autoplay
        muted
        loop
        playsinline
        class="aspect-[1.539503386] w-full rounded-2xl object-cover shadow-lg shadow-neutral-500/50"
      >
        <source src="/file_example_MP4_480_1_5MG.mp4" type="video/mp4" />
      </video>
    </div>
  </section>

  <section id="features" class="features mt-48">
    <div class="flex flex-col gap-y-32">
      <FeatureSection
        videoSrc="/file_example_MP4_480_1_5MG.mp4"
        title="Click anywhere, without a mouse"
        description="Press [[⌘]][[⇧]][[Space]] and type the label of a UI element (e.g. [[F]][[D]]) to perform a click."
      />

      <!-- <FeatureSection videoSrc="/file_example_MP4_480_1_5MG.mp4" title="Scroll any app" mirrored>
        Press <KeyboardSymbol symbol="⌘" />
        <KeyboardSymbol symbol="⇧" />
        <KeyboardSymbol symbol="J" />
        and start scrolling with&nbsp;<KeyboardSymbol symbol="J" />↓ and
        <KeyboardSymbol symbol="K" />↑.<br />Hold
        <KeyboardSymbol symbol="Shift" />
        to scroll faster.<br /><br />Switch to another scroll area by pressing
        <KeyboardSymbol symbol="Tab" /> or the labeled Numbers.
      </FeatureSection>

      <FeatureSection videoSrc="/file_example_MP4_480_1_5MG.mp4" title="Search and click">
        Press <KeyboardSymbol symbol="⌘" />
        <KeyboardSymbol symbol="⇧" />
        <KeyboardSymbol symbol="/" />
        and type what you want to click.<br /><br />Use the arrow keys to focus on another UI
        element. Alternatively, type the label of an element while holding
        <KeyboardSymbol symbol="Shift" />.<br /><br />Press
        <KeyboardSymbol symbol="Return" /> to click the focused element.
      </FeatureSection>

      <FeatureSection videoSrc="/file_example_MP4_480_1_5MG.mp4" title="The Tutor 🤓" mirrored>
        For some UI elements, it is not immediately obvious what the search query is. Press <KeyboardSymbol
          symbol="?"
        /> to reveal the searchable properties of the focused element.
      </FeatureSection> -->
    </div>
  </section>

  <section id="compatibility"></section>
</main>
