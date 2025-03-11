<script lang="ts">
  import FAQAccordionMenu from "./FAQAccordionMenu.svelte"
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
          alt="Clipboard X app icon"
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

      <FeatureSection
        videoSrc="/file_example_MP4_480_1_5MG.mp4"
        title="Scroll any app"
        mirrored
        description="Press [[⌘]][[⇧]][[J]]
        and start scrolling with&nbsp;[[J]]↓ and
        [[K]]↑.<br />Hold [[Shift]]
        to scroll faster.<br /><br />Switch to another scroll area by pressing
        [[Tab]] or the labeled Numbers."
      />

      <FeatureSection
        videoSrc="/file_example_MP4_480_1_5MG.mp4"
        title="Search and click"
        description="Press [[⌘]]
        [[⇧]]
        [[/]]
        and type what you want to click.<br /><br />Use the arrow keys to focus on another UI
        element. Alternatively, type the label of an element while holding
        [[Shift]].<br /><br />Press
        [[Return]] to click the focused element."
      />

      <FeatureSection
        videoSrc="/file_example_MP4_480_1_5MG.mp4"
        title="The Tutor 🤓"
        mirrored
        description="For some UI elements, it is not immediately obvious what the search query is. Press [[?]] to reveal the searchable properties of the focused element."
      />
    </div>
  </section>

  <section
    id="compatibility"
    class="mt-32 flex flex-col items-center gap-y-8 rounded-2xl bg-gradient-to-b from-sky-800 to-neutral-800 px-8 pt-12 pb-8 text-center md:flex-row md:gap-x-16 md:bg-gradient-to-r md:px-12 md:py-12 md:text-left"
  >
    <div class="md:basis-[calc(50%-2rem)]">
      <h2 class="text-3xl font-bold text-white sm:text-4xl">Works with your favourite apps</h2>
      <p class="mt-6 text-lg font-normal text-neutral-200">
        Homerow works with most native macOS apps and a growing set of non-native web-based apps.
      </p>
    </div>
    <div class="flex justify-center md:basis-[calc(50%-2rem)]">
      <div class="grid w-full grid-cols-5 gap-4">
        <div class="max-w-[80px]">
          <img
            alt="app icon of chrome"
            loading="lazy"
            width="1024"
            height="1024"
            decoding="async"
            data-nimg="1"
            style="color:transparent"
            src="/clipboardx.png"
          />
        </div>
        <div class="max-w-[80px]">
          <img
            alt="app icon of safari"
            loading="lazy"
            width="1024"
            height="1024"
            decoding="async"
            data-nimg="1"
            style="color:transparent"
            src="/clipboardx.png"
          />
        </div>
        <div class="max-w-[80px]">
          <img
            alt="app icon of firefox"
            loading="lazy"
            width="1024"
            height="1024"
            decoding="async"
            data-nimg="1"
            style="color:transparent"
            src="/clipboardx.png"
          />
        </div>
        <div class="max-w-[80px]">
          <img
            alt="app icon of arc"
            loading="lazy"
            width="1024"
            height="1024"
            decoding="async"
            data-nimg="1"
            style="color:transparent"
            src="/clipboardx.png"
          />
        </div>
        <div class="max-w-[80px]">
          <img
            alt="app icon of vscode"
            loading="lazy"
            width="1024"
            height="1024"
            decoding="async"
            data-nimg="1"
            style="color:transparent"
            src="/clipboardx.png"
          />
        </div>
        <div class="max-w-[80px]">
          <img
            alt="app icon of xcode"
            loading="lazy"
            width="1024"
            height="1024"
            decoding="async"
            data-nimg="1"
            style="color:transparent"
            src="/clipboardx.png"
          />
        </div>
        <div class="max-w-[80px]">
          <img
            alt="app icon of slack"
            loading="lazy"
            width="1024"
            height="1024"
            decoding="async"
            data-nimg="1"
            style="color:transparent"
            src="/clipboardx.png"
          />
        </div>
        <div class="max-w-[80px]">
          <img
            alt="app icon of discord"
            loading="lazy"
            width="1024"
            height="1024"
            decoding="async"
            data-nimg="1"
            style="color:transparent"
            src="/clipboardx.png"
          />
        </div>
        <div class="max-w-[80px]">
          <img
            alt="app icon of notion"
            loading="lazy"
            width="1024"
            height="1024"
            decoding="async"
            data-nimg="1"
            style="color:transparent"
            src="/clipboardx.png"
          />
        </div>
        <div class="max-w-[80px]">
          <img
            alt="app icon of obsidian"
            loading="lazy"
            width="1024"
            height="1024"
            decoding="async"
            data-nimg="1"
            style="color:transparent"
            src="/clipboardx.png"
          />
        </div>
        <div class="max-w-[80px]">
          <img
            alt="app icon of notes"
            loading="lazy"
            width="1024"
            height="1024"
            decoding="async"
            data-nimg="1"
            style="color:transparent"
            src="/clipboardx.png"
          />
        </div>
        <div class="max-w-[80px]">
          <img
            alt="app icon of mail"
            loading="lazy"
            width="1024"
            height="1024"
            decoding="async"
            data-nimg="1"
            style="color:transparent"
            src="/clipboardx.png"
          />
        </div>
        <div class="max-w-[80px]">
          <img
            alt="app icon of spotify"
            loading="lazy"
            width="1024"
            height="1024"
            decoding="async"
            data-nimg="1"
            style="color:transparent"
            src="/clipboardx.png"
          />
        </div>
        <div class="max-w-[80px]">
          <img
            alt="app icon of finder"
            loading="lazy"
            width="1024"
            height="1024"
            decoding="async"
            data-nimg="1"
            style="color:transparent"
            src="/clipboardx.png"
          />
        </div>
        <div class="max-w-[80px]">
          <img
            alt="app icon of system-preferences"
            loading="lazy"
            width="1024"
            height="1024"
            decoding="async"
            data-nimg="1"
            style="color:transparent"
            src="/clipboardx.png"
          />
        </div>
      </div>
    </div>
  </section>

  <section id="pricing" class="mt-32 flex flex-col">
    <h2 class="text-center text-3xl font-bold text-neutral-900 sm:text-4xl">
      Buy once, use forever
    </h2>
    <p class="mt-2 text-center text-xl font-normal text-neutral-500">
      Homerow is a one-time purchase.<br /> You own it completely, 'til the heat death of the universe.
    </p>
    <div class="mt-16 mb-16 flex flex-row flex-wrap items-center justify-center gap-8">
      <div
        class="flex max-w-[24rem] basis-full flex-col items-center rounded-2xl bg-white p-8 shadow-xl ring-1 ring-neutral-200 sm:p-12"
      >
        <div class="flex">
          <p class="mt-2 ml-1 text-3xl font-bold text-neutral-700">$</p>
          <p class="mt-2 text-6xl font-bold text-neutral-900">49</p>
          <p class="mt-2 ml-1 text-3xl font-bold text-neutral-900">99</p>
        </div>
        <h3 class="text-xl font-semibold text-neutral-700">Homerow Pro</h3>
        <ul class="mt-8">
          <li class="mt-2 flex flex-row items-center">
            <svg
              width="21"
              height="21"
              viewBox="0 0 15 15"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="inline rounded-full bg-green-500 text-white"
              ><path
                d="M7.49991 0.877045C3.84222 0.877045 0.877075 3.84219 0.877075 7.49988C0.877075 11.1575 3.84222 14.1227 7.49991 14.1227C11.1576 14.1227 14.1227 11.1575 14.1227 7.49988C14.1227 3.84219 11.1576 0.877045 7.49991 0.877045ZM1.82708 7.49988C1.82708 4.36686 4.36689 1.82704 7.49991 1.82704C10.6329 1.82704 13.1727 4.36686 13.1727 7.49988C13.1727 10.6329 10.6329 13.1727 7.49991 13.1727C4.36689 13.1727 1.82708 10.6329 1.82708 7.49988ZM10.1589 5.53774C10.3178 5.31191 10.2636 5.00001 10.0378 4.84109C9.81194 4.68217 9.50004 4.73642 9.34112 4.96225L6.51977 8.97154L5.35681 7.78706C5.16334 7.59002 4.84677 7.58711 4.64973 7.78058C4.45268 7.97404 4.44978 8.29061 4.64325 8.48765L6.22658 10.1003C6.33054 10.2062 6.47617 10.2604 6.62407 10.2483C6.77197 10.2363 6.90686 10.1591 6.99226 10.0377L10.1589 5.53774Z"
                fill="currentColor"
                fill-rule="evenodd"
                clip-rule="evenodd"
              ></path></svg
            ><span class="ml-2 text-base font-normal text-neutral-900">Use on all your devices</span
            >
          </li>
          <li class="mt-2 flex flex-row items-center">
            <svg
              width="21"
              height="21"
              viewBox="0 0 15 15"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="rounded-full bg-green-500 text-white"
              ><path
                d="M7.49991 0.877045C3.84222 0.877045 0.877075 3.84219 0.877075 7.49988C0.877075 11.1575 3.84222 14.1227 7.49991 14.1227C11.1576 14.1227 14.1227 11.1575 14.1227 7.49988C14.1227 3.84219 11.1576 0.877045 7.49991 0.877045ZM1.82708 7.49988C1.82708 4.36686 4.36689 1.82704 7.49991 1.82704C10.6329 1.82704 13.1727 4.36686 13.1727 7.49988C13.1727 10.6329 10.6329 13.1727 7.49991 13.1727C4.36689 13.1727 1.82708 10.6329 1.82708 7.49988ZM10.1589 5.53774C10.3178 5.31191 10.2636 5.00001 10.0378 4.84109C9.81194 4.68217 9.50004 4.73642 9.34112 4.96225L6.51977 8.97154L5.35681 7.78706C5.16334 7.59002 4.84677 7.58711 4.64973 7.78058C4.45268 7.97404 4.44978 8.29061 4.64325 8.48765L6.22658 10.1003C6.33054 10.2062 6.47617 10.2604 6.62407 10.2483C6.77197 10.2363 6.90686 10.1591 6.99226 10.0377L10.1589 5.53774Z"
                fill="currentColor"
                fill-rule="evenodd"
                clip-rule="evenodd"
              ></path></svg
            ><span class="ml-2 text-base font-normal text-neutral-900"
              >All future features &amp; releases</span
            >
          </li>
          <li class="mt-2 flex flex-row items-center">
            <svg
              width="21"
              height="21"
              viewBox="0 0 15 15"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="rounded-full bg-green-500 text-white"
              ><path
                d="M7.49991 0.877045C3.84222 0.877045 0.877075 3.84219 0.877075 7.49988C0.877075 11.1575 3.84222 14.1227 7.49991 14.1227C11.1576 14.1227 14.1227 11.1575 14.1227 7.49988C14.1227 3.84219 11.1576 0.877045 7.49991 0.877045ZM1.82708 7.49988C1.82708 4.36686 4.36689 1.82704 7.49991 1.82704C10.6329 1.82704 13.1727 4.36686 13.1727 7.49988C13.1727 10.6329 10.6329 13.1727 7.49991 13.1727C4.36689 13.1727 1.82708 10.6329 1.82708 7.49988ZM10.1589 5.53774C10.3178 5.31191 10.2636 5.00001 10.0378 4.84109C9.81194 4.68217 9.50004 4.73642 9.34112 4.96225L6.51977 8.97154L5.35681 7.78706C5.16334 7.59002 4.84677 7.58711 4.64973 7.78058C4.45268 7.97404 4.44978 8.29061 4.64325 8.48765L6.22658 10.1003C6.33054 10.2062 6.47617 10.2604 6.62407 10.2483C6.77197 10.2363 6.90686 10.1591 6.99226 10.0377L10.1589 5.53774Z"
                fill="currentColor"
                fill-rule="evenodd"
                clip-rule="evenodd"
              ></path></svg
            ><span class="ml-2 text-base font-normal text-neutral-900"
              >No annoying purchase pop-up</span
            >
          </li>
        </ul>
        <div class="mt-8"></div>
        <a href="https://buy.stripe.com/8wMeVP3FU33zeQ0bIP" target="_blank" class="w-full"
          ><button
            style="background:radial-gradient(at bottom, rgba(50,50,50,1) 0%, rgba(10,10,10,1) 100%)"
            class=" relative w-full rounded-xl border-b-[6px] border-b-black shadow-xl transition-all select-none hover:-translate-y-[1px] hover:shadow-2xl active:translate-y-[4px] active:border-b-2 active:shadow-md"
            ><div
              class="w-full rounded-xl border-t-1 border-b-[1px] border-t-white/30 border-b-white/20 px-6 py-4 text-center text-lg font-medium text-white shadow-inner active:border-b-0 active:border-t-black"
            >
              Buy now
            </div></button
          ></a
        >
      </div>
    </div>
  </section>

  <section id="faq" class="mt-32 flex flex-col items-center">
    <h2 class="text-center text-3xl font-bold text-neutral-900 sm:text-4xl">
      Questions &amp; Answers
    </h2>
    <p class="mt-2 text-center text-xl font-normal text-neutral-500">
      If you have any other questions - please get in touch
    </p>
    <div class="mt-16 mb-16 w-full">
      <FAQAccordionMenu
        items={[
          {
            question: "Is Homerow free?",
            answer:
              "Homerow is a paid application. However, you can use Homerow without a license. An annoying prompt to purchase will show every 50 activations. Sorry about that, but I have kids to feed.",
          },
          {
            question: "Which apps are supported by Homerow?",
            answer:
              "Homerow works with nearly all native macOS applications. Popular non-native apps such as Chrome, Firefox, Brave, Arc, Visual Studio Code, Spotify, Slack, Discord, and Obsidian are supported, among many others.",
          },
          {
            question: "Is there a student discount?",
            answer:
              "Yes! There is a 30% discount for students. Please drop me an email at hey@homerow.app from your student email and I'll get back to you with the discount code.",
          },
          {
            question: "Can I change the machine a license is linked to?",
            answer:
              "Yes. You must first unlink the license from the old machine in Preferences > Unlink License.",
          },
        ]}
      />
    </div>
  </section>

  <section id="footer" class="flex flex-col gap-y-8 pt-10 pb-10 sm:flex-row">
    <div class="flex-grow">
      <div class="flex flex-grow flex-row items-center gap-x-2">
        <img
          alt="Clipboard X app icon"
          loading="lazy"
          width="32"
          height="32"
          decoding="async"
          class="inline"
          style="color:transparent"
          src="/clipboardx.png"
        /><span class="text-base font-semibold text-neutral-900">Clipboard X</span>
      </div>
      <div class="mt-4">
        <p class="text-xs font-medium text-neutral-500">
          © 2025 Clipboard X, Inc. All rights reserved.
        </p>
      </div>
    </div>
    <div class="flex flex-grow items-center sm:justify-end">
      <ul class="flex flex-col gap-4 sm:flex-row">
        <li>
          <a
            target="_blank"
            class="text-sm font-medium text-neutral-500 hover:text-neutral-900"
            href="/changelog">Changelog</a
          >
        </li>
        <li>
          <a
            target="_blank"
            class="text-sm font-medium text-neutral-500 hover:text-neutral-900"
            href="/user-guide">User Guide</a
          >
        </li>
        <li>
          <a
            target="_blank"
            class="text-sm font-medium text-neutral-500 hover:text-neutral-900"
            href="https://twitter.com/clipboardx_app">Twitter</a
          >
        </li>
        <li>
          <a
            target="_blank"
            class="text-sm font-medium text-neutral-500 hover:text-neutral-900"
            href="mailto:hey@clipboardx.app">Get in touch</a
          >
        </li>
      </ul>
    </div>
  </section>
</main>
