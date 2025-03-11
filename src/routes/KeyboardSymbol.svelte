<script lang="ts">
  let { symbol }: { symbol: string } = $props()
</script>

<span
  class="shadow-inset-skeuo inline-block cursor-pointer rounded bg-amber-400/40 px-3 pt-0.5 pb-1 font-mono text-sm font-semibold tracking-tight text-neutral-900 transition-all duration-75 select-none hover:-translate-y-[1px] active:translate-y-1"
>
  {symbol}
</span>
