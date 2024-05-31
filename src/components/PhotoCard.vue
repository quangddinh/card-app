<script setup lang="ts">
import { ref } from 'vue';

interface ICard {
  img: string;
  label: string;
}

const data = ref<ICard[]>([
  {
    img: 'https://i.imgur.com/2MM9Jqo.png',
    label: 'This is a long paragraph that will be truncated when it exceeds the width of its container',
  },
  {
    img: 'https://i.imgur.com/2MM9Jqo.png',
    label: 'This is a long paragraph that will be truncated when it exceeds the width of its container',
  },
  {
    img: 'https://i.imgur.com/unmma82.jpeg',
    label: 'This is a long paragraph that will be truncated when it exceeds the width of its container',
  },
  {
    img: 'https://i.imgur.com/2MM9Jqo.png',
    label: 'This is a long paragraph that will be truncated when it exceeds the width of its container',
  },
  {
    img: 'https://i.imgur.com/2MM9Jqo.png',
    label: 'This is a long paragraph that will be truncated when it exceeds the width of its container',
  },
  {
    img: 'https://i.imgur.com/2MM9Jqo.png',
    label: 'This is a long paragraph that will be truncated when it exceeds the width of its container',
  },
  {
    img: 'https://i.imgur.com/2MM9Jqo.png',
    label: 'This is a long paragraph that will be truncated when it exceeds the width of its container',
  },
  {
    img: 'https://i.imgur.com/unmma82.jpeg',
    label: 'This is a long paragraph that will be truncated when it exceeds the width of its container',
  },
  {
    img: 'https://i.imgur.com/unmma82.jpeg',
    label: 'This is a long paragraph that will be truncated when it exceeds the width of its container',
  },
  {
    img: 'https://i.imgur.com/unmma82.jpeg',
    label: 'This is a long paragraph that will be truncated when it exceeds the width of its container',
  },
  {
    img: 'https://i.imgur.com/2MM9Jqo.png',
    label: 'This is a long paragraph that will be truncated when it exceeds the width of its container',
  },
  {
    img: 'https://i.imgur.com/2MM9Jqo.png',
    label: 'This is a long paragraph that will be truncated when it exceeds the width of its container',
  },
]);
</script>

<template>
  <section class="card-display">
    <h2>Photo Cards</h2>
    <div class="card-list">
      <div v-for="(item, index) in data" :key="index" class="card-item">
        <div class="card-image-container">
          <img class="card-image" :src="item.img" alt="No image" />
        </div>
        <p>{{ item.label }}</p>
      </div>
    </div>
  </section>
</template>
