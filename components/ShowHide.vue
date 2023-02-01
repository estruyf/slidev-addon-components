<!-- 
Example:

---
clicks: 4
---

# Common capabilities of extensions

- Registering commands, configurations, keybindings, or menus
- Storing workspace or global state
- Displaying notifications
- Collect user input
- Open files, folders, or URLs
- Theming
- Language features

<ShowHide show="1" hide="2">
  Show on click 1, hide on 2, {{ $slidev.nav.clicks }}
</ShowHide>
<ShowHide show="2" hide="3">
  Show on click 1, hide on 2, {{ $slidev.nav.clicks }}
</ShowHide>

-->


<script setup lang="ts">
import { ref, resolveDirective } from 'vue'

const props = defineProps({
  show: {
    type: String,
    default: 0
  },
  hide: {
    type: String,
    default: 0
  },
})

const showNr = parseInt(props.show)
const hideNr = parseInt(props.hide)
</script>

<template>
  <slot v-if="$slidev.nav.clicks >= showNr && $slidev.nav.clicks < hideNr" />
</template>
