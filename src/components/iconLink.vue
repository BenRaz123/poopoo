<script setup>
    
    import { defineProps } from 'vue';

    defineProps({
        text: {type:String, required:true},
        icon: {type:String, required:false},
        url:  {type:String, required:false}
    })
</script>

<template>
    <a v-if="url" target="_blank" :href="url">
        <div class="navbar-item">
            <i v-if="icon" :class="icon"></i>
            <span class="icon-text">{{ text }}</span>
        </div>
    </a>
</template>