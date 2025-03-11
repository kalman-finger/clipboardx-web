<script lang="ts">
  let {
    href,
    text,
  }: {
    href: string
    text: string
  } = $props()
</script>

<a {href} class="text-sm font-medium text-neutral-500 hover:text-neutral-900">{text}</a>
