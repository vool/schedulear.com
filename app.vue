<template>
<div class="min-h-screen grid grid-flow-row md:grid-flow-col bg-lusta">

  <div class="flex p-2 relative bg-shaft text-lusta">
    <div class="p-8  ">
      <ImgsLogo />
    </div>
    <div class="p-8 float-right absolute bottom-0 right-0 ">
      <ImgsName />
    </div>
  </div>
  <div class="flex relative">

    <div class="p-8 hidden md:block absolute top-0 right-0  ">
      ...organising the world for the ear
    </div>


    <div class="p-8 bottom-0 absolute right-0  ">

      <ul class="flex justify-center mt-5 space-x-5">
        <li>
          <a href="https://mastodon.social/@schedulear" target="_blank" class="text-shaft hover:text-black">
            <ImgsIconsMastodon />
          </a>
        </li>
        <li>
          <a href="https://bsky.app/profile/schedulear.bsky.social" target="_blank" class="text-shaft hover:text-black">
            <ImgsIconsBluesky />
          </a>
        </li>
        <li>
          <a href="https://www.instagram.com/schedulear_" target="_blank" class="text-shaft hover:text-black">
            <ImgsIconsInstagram />
          </a>
        </li>
        <li>
          <a href="mailto:hello@schedulear.com" target="_blank" class="text-shaft hover:text-black">
            <ImgsIconsEmail />
          </a>
        </li>
      </ul>

    </div>
  </div>
</div>
</template>
