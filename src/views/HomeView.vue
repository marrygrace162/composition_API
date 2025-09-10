<script setup>
import { ref } from 'vue';
import MyWrapper from '@/components/MyWrapper.vue'
import PostItem from '@/components/PostItem.vue'

const posts = [
  {
    id: 65,
    author: "Rina Doydora",
    created_at: "2025-05-01",
    title: "consequatur id enim sunt et et",
    body: "voluptatibus ex esse\nsint explicabo est aliquid cumque adipisci fuga repellat labore…",
    is_saved: false
  },
  {
    id: 66,
    author: "Marry Grace Capesos",
    created_at: "2025-05-01",
    title: "repudiandae ea animi iusto",
    body: "officia veritatis tenetur vero qui itaque…",
    is_saved: false
  },
  {
    id: 67,
    author: "Angeline Magan",
    created_at: "2025-05-04",
    title: "aliquid eos sed fuga est maxime repellendus",
    body: "reprehenderit id nostrum voluptas doloremque pariatur…",
    is_saved: false
  },
  {
    id: 68,
    author: "Zhaira Jane Martinez",
    created_at: "2025-05-01",
    title: "odio quis facere architecto reiciendis optio",
    body: "magnam molestiae perferendis quisquam qui cum reiciendis…",
    is_saved: false
  },
]
</script>

<template>
  <div v-for="post in posts" :key="post.id">
    <MyWrapper>
      <PostItem :post="post" />
    </MyWrapper>
  </div>
</template>

<style>
body {
  margin: 0;
  padding: 0;
  background: linear-gradient(135deg, #ffe0b2, #e1bee7);
  font-family: "Segoe UI", Arial, sans-serif;
}

.wrapper {
  max-width: 700px;
  margin: 40px auto;
  padding: 24px;
  background: #fff;
  border-radius: 16px;
  box-shadow: 0 6px 16px rgba(0,0,0,0.12);
}
</style>
