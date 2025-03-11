<script lang="ts">
  import { renderSymbols } from "$lib/symbols"

  let {
    videoSrc,
    mirrored = false,
    title,
    description = "",
  }: {
    videoSrc: string
    mirrored?: boolean
    title: string
    description?: string
  } = $props()
</script>

<div class="flex flex-col items-center gap-y-8 md:flex-row md:gap-x-16">
  <div class="md:basis-[calc(60%-2rem)]">
    <video
      autoplay
      muted
      loop
      playsinline
      class="aspect-[1.539503386] w-full rounded-xl object-cover shadow-md shadow-neutral-500/50"
    >
      <source src={videoSrc} type="video/mp4" /></video
    >
  </div>
  <div class="w-full {mirrored ? 'md:order-first' : 'md:order-last'} md:basis-[calc(40%-2rem)]">
    <h3 class="text-2xl font-semibold text-neutral-900 sm:text-3xl">
      {title}
    </h3>
    <p class="mt-4 text-lg font-normal text-neutral-600">
      {@html renderSymbols(description)}
    </p>
  </div>
</div>
