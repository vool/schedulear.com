<script lang="ts" setup>
useSeoMeta({
  title: 'schedulear',
  ogTitle: 'schedulear',
  description: '...organising the world for the ear',
  ogDescription: '...organising the world for the ear',
  ogImage: 'https://schedulear.com/og_card.png',
  twitterCard: 'summary_large_image',
})

useHead({
  script: [
    {
      src: "https://tally.so/widgets/embed.js",
      defer: true,
    },
  ],
});

onMounted(() => {
  if (window.Tally) {
    window.Tally.loadEmbeds()
  }
})

const sections = [
  {
    label: 'We think',
    title: "Listening to great radio shouldn't be hard.",
    description:
        "The world is full of incredible radio, but discovering the right show at the right time is harder than it should be. With schedules scattered across websites and apps, confusing time zones, and no simple way to see what's live, too much great radio goes unheard."
  },
  {
    label: 'The problem',
    title: "Radio isn't broken because of the content, it's broken because of discovery.",
    description:
        "Radio has always had incredible content, we’re just building the discovery layer it's been missing. A platform connecting stations, presenters, DJs, and listeners to make live audio easier to find, follow, and experience."
  },
  {
    label: 'Built for',
    title: "Those who broadcast, and those who listen.",
    description:
        "A platform that helps stations, presenters, DJs, podcasters, and creators reach the right audience, while giving listeners a better way to discover, follow, and engage with the voices and shows they love."
  },
  {
    label: 'Join us',
    title: "Stay tuned.",
    description:
        "Join the waitlist and be the first to know when early access opens."
  }
]

</script>
<template>


  <div class="min-h-screen bg-white text-zinc-900">
    <div class="mx-auto grid max-w-7xl grid-cols-1 lg:grid-cols-[1fr_440px]">

      <!-- Scroll Content -->

      <main class="px-8 lg:px-20">

        <section class="flex min-h-screen items-center">
          <div class="max-w-3xl">

            <!-- Logo -->
            <div class="mb-12 flex items-center gap-3">
              <div
                  class="flex h-18 w-18 xitems-center xjustify-center xrounded-xl xbg-zinc-900 text-sm font-medium xtext-white text-zinc-900"
              >
                <ImgsLogo/>
              </div>
            </div>


            <h1
                class="text-4xl font-medium leading-[1.05] tracking-tight text-zinc-950 lg:text-6xl"
            >Still listening to radio like it's 1926?
            </h1>

            <p class="mt-8 max-w-xl text-xl leading-9 text-zinc-600">
              Keep missing your favourite shows? Stuck listening to the same two stations? Or worse, listening to
              algorithmic playlists while your favourite DJs are live?
            </p>

          </div>
        </section>
        <section
            v-for="section in sections"
            :key="section.label"
            class="flex min-h-screen items-center"
        >
          <div class="max-w-2xl">

            <span
                class="inline-flex rounded-full bg-zinc-100 px-3 py-1 text-sm text-zinc-600"
            >
              {{ section.label }}
            </span>

            <h2 class="mt-8 text-4xl font-medium tracking-tight lg:text-6xl">
              {{ section.title }}
            </h2>

            <p class="mt-8 text-xl leading-9 text-zinc-600">
              {{ section.description }}
            </p>

          </div>
        </section>


        <section class="flex min-h-[40vh] items-center">


          <div>

            <p class="my-28 text-xs xtext-zinc-400 text-zinc-900">
              <ImgsName/>
            </p>


            <div class="flex flex-wrap gap-4 text-sm">
              <a
                  class="text-zinc-500 transition hover:text-black"
                  href="mailto:listen@product.com"
              >
                listen@schedulear.com
              </a>

              <span class="text-zinc-300">/</span>

              <a
                  class="text-zinc-500 transition hover:text-black"
                  href="https://mastodon.social/@schedulear"
              >
                mastodon
              </a>

              <span class="text-zinc-300">/</span>

              <a
                  class="text-zinc-500 transition hover:text-black"
                  href="https://bsky.app/profile/schedulear.bsky.social"
              >
                bluesky
              </a>

              <span class="text-zinc-300">/</span>

              <a
                  class="text-zinc-500 transition hover:text-black"
                  href="https://www.instagram.com/schedulear_"
              >
                instagram
              </a>
            </div>
          </div>
        </section>
      </main>


      <!-- Right: Waitlist -->
      <aside>
        <div
            class="flex items-center border-t border-zinc-100 px-8 py-12 lg:sticky lg:top-0 lg:h-screen lg:border-l lg:border-t-0 lg:px-10"
        >
          <div
              class="w-full max-w-sm rounded-3xl border border-zinc-200 bg-white p-8 shadow-xl shadow-zinc-100"
          >

            <p class="mt-2 text-zinc-600">
              Join the waitlist...
            </p>

            <div class="mt-8">
              <iframe
                  data-tally-src="https://tally.so/embed/Zja6Py?alignLeft=1&hideTitle=1&transparentBackground=1&dynamicHeight=1"
                  frameborder="0"
                  height="540"
                  loading="lazy"
                  marginheight="0"
                  marginwidth="0"
                  title="join wait list"
                  width="100%"
              />
            </div>

          </div>
        </div>

      </aside>

    </div>
  </div>

</template>
