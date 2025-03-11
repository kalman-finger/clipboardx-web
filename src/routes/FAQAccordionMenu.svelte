<script lang="ts">
  type AccordionMenuItem = {
    question: string
    answer: string
  }

  let {
    items,
  }: {
    items: AccordionMenuItem[]
  } = $props()

  let itemStates = $state(items.map((item) => ({ open: false })))

  const toggleAccordionItem = (index: number) => () => {
    itemStates = itemStates.map((item, i) => (i === index ? { open: !item.open } : { open: false }))
  }
</script>

<ul class="mx-auto flex max-w-3xl flex-col gap-y-8">
  {#each items as item, i (item.question)}
    <li>
      <div>
        <button
          type="button"
          class="w-full cursor-pointer appearance-none"
          aria-controls={`accordion${i}`}
          aria-expanded={itemStates[i].open}
          onclick={toggleAccordionItem(i)}
        >
          <div class="flex flex-row items-center justify-between gap-x-4">
            <span class="text-lg font-semibold text-neutral-900">{item.question}</span>
            <div>
              <svg
                width="24"
                height="24"
                viewBox="0 0 15 15"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="inline stroke-none text-neutral-900"
                class:-rotate-180={itemStates[i].open}
                ><path
                  d="M3.13523 6.15803C3.3241 5.95657 3.64052 5.94637 3.84197 6.13523L7.5 9.56464L11.158 6.13523C11.3595 5.94637 11.6759 5.95657 11.8648 6.15803C12.0536 6.35949 12.0434 6.67591 11.842 6.86477L7.84197 10.6148C7.64964 10.7951 7.35036 10.7951 7.15803 10.6148L3.15803 6.86477C2.95657 6.67591 2.94637 6.35949 3.13523 6.15803Z"
                  fill="currentColor"
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                ></path></svg
              >
            </div>
          </div>
        </button>
        <!-- TODO If multiple Accordions are present the ids won't be unique -->
        <div id={`accordion${i}`} class:hidden={!itemStates[i].open}>
          {#if itemStates[i].open}
            <div class="mt-6 flex flex-col gap-y-3">
              <p class="text-base text-neutral-600">{item.answer}</p>
            </div>
          {/if}
        </div>
      </div>
    </li>
  {/each}
</ul>
