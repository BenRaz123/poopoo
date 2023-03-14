<template>
<div class="title-section">
    <div class="title-section-text">
      <h1>{{headerText}}</h1>
      <p>
        {{paragraphText}}
      </p>
    </div>
    <img v-if="imgPath && imgAlt" :src="require(`@/assets/img/${imgPath}`)" :alt=imgAlt />
  </div>
</template>

<script>
    export default {
        name: 'TitleSection',
        props: {
            'headerText': String,
            'paragraphText': String,
            'imgPath': String,
            'imgAlt': String
        }
    }
</script>