<template>
<div class="min-h-screen flex space-y-1 w-full fixed bg-lusta-50 ">
  <div class="flex-1 p-2  relative bg-shaft-950 text-lusta-50">


    <div class="p-8  ">
      <ImgsLogo />
    </div>


    <div class="p-8 bottom-0 float-right absolute bottom-0 right-0 ">
      <ImgsName />
    </div>

  </div>

  <div class="flex-1 relative">

    <div class="p-8  float-right ">
      ...organise the world for the ear.
    </div>


    <div class="p-8 bottom-0 float-right absolute bottom-0 right-0  ">

      <ul class="flex justify-center mt-5 space-x-5">
        <li>
          <a href="https://mastodon.social/@schedulear" target="_blank" class="hover:text-white">
            <ImgsIconsMastodon />
          </a>
        </li>
        <li>
          <a href="https://bsky.app/profile/schedulear.bsky.social" target="_blank" class="text-gray-500 hover:text-gray-900 dark:hover:text-white dark:text-gray-400">
            <ImgsIconsBluesky />
          </a>
        </li>
        <li>
          <a href="https://www.instagram.com/schedulear_" target="_blank" class="text-gray-500 hover:text-gray-900 dark:hover:text-white dark:text-gray-400">
            <ImgsIconsInstagram />
          </a>
        </li>
        <li>
          <a href="mailto:hello@schedulear.com" target="_blank" class="text-gray-500 hover:text-gray-900 dark:hover:text-white dark:text-gray-400">
            <ImgsIconsEmail />
          </a>
        </li>
      </ul>

    </div>
  </div>

</div>
</template>
