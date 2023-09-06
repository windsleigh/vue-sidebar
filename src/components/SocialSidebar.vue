<template>
  <div>
    <div :class="$style.sidebar">
      <a href="https://www.facebook.com/">
        <font-awesome-icon :icon="['fab', 'facebook']" :class="$style.icon" />
      </a>
      <a href="https://www.twitter.com/">
        <font-awesome-icon :icon="['fab', 'twitter']" :class="$style.icon" />
      </a>
      <a href="https://www.instagram.com/">
        <font-awesome-icon :icon="['fab', 'instagram']" :class="$style.icon" />
      </a>
    </div>
  </div>
</template>

<script setup>
import { library } from '@fortawesome/fontawesome-svg-core'
import { faFacebook, faTwitter, faInstagram } from '@fortawesome/free-brands-svg-icons'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'

library.add(faFacebook, faTwitter, faInstagram)
</script>

<style module>
.sidebar {
  position: fixed;
  top: 50%;
  left: 2rem;
  transform: translateY(-50%);
  display: flex;
  flex-direction: column;
  box-shadow:
    5px 0px 10px rgba(0, 0, 0, 0.5),
    0px 5px 10px rgba(0, 0, 0, 0.5);
  padding: 1rem;
  border-radius: 5px;
  background-color: rgb(255, 255, 255);
}

.icon {
  font-size: 24px;
  margin-top: 1rem;
  margin-bottom: 1rem;
  color: black;
}
</style>
