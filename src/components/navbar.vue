<script setup>
  import iconLink from './iconLink.vue';
</script>

<template>
  <div id="navbar" class="navbar">
      <div class="navbar-item" id="nav-title">Ben Raz</div>
      <div class="nav-links-container">
        
        <iconLink
          text="Stack Overflow"
          icon="fa-brands fa-stack-overflow"
          url="https://stackoverflow.com/users/15595062/ben-raz"
        />

        <iconLink 
          text="Github"
          icon="fa-brands fa-github"
          url="github.com/benraz123/"
        />

        <iconLink 
          text="Youtube"
          icon="fa-brands fa-youtube"
          url="https://youtube.com/channel/UCVH5pH8Yua6D42eRaAXoZYQ"
        />

        <iconLink
          text="Twitter"
          icon="fa-brands fa-twitter"
          url="https://www.twitter.com/hhhhh31352962"
        />

        <iconLink
          text="Email"
          icon="fa-solid fa-at"
          url="mailto:ben.raz2008@gmail.com"  
        />
      
      </div>
    </div>
</template>
