---
title: Nuxt Helpers
description: Using the $nuxt helpers with $nuxt.isOnline, renderedOn, refresh(), onNuxtReady
position: 8
category: miscellaneous
csb_link: https://codesandbox.io/embed/github/nuxtlabs/examples/tree/master/miscellaneous/nuxt-helpers?fontsize=14&hidenavigation=1&theme=dark&view=editor
---

<example-intro></example-intro>
<p>In this example:</p>

`pages/index.vue` shows:

- `$nuxt.isOnline` and `$nuxt.isOffline` - tells the user if they are online or offline.
- `renderedOn` - prints a message telling us if the page is rendered on the server or client.
- `$nuxt.refresh()` - refreshes data without refreshing the page.

`plugins/nuxt-ready.client.js` shows:

- `window.onNuxtReady` - logs a message to the console when Nuxt is ready.

<base-alert type="next">

<div class ="Learncontainor">
    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 9l3 3m0 0l-3 3m3-3H8m13 0a9 9 0 11-18 0 9 9 0 0118 0z" />
    </svg>
    <p>Learn more in the Concepts book in the <a href="#"> Context and Helpers </a> chapter.</p>
</div>


</base-alert>

<code-sandbox :src="csb_link"></code-sandbox>
