<script setup>
const post = [
  {
    "userId": 7,
    "id": 65,
    "name": "Rina Doydora",
    "date": "2025-05-01",
    "title": "consequatur id enim sunt et et",
    "body": "voluptatibus ex esse\nsint explicabo est aliquid cumque adipisci fuga repellat labore\nmolestiae corrupti ex saepe at asperiores et perferendis\nnatus id esse incidunt pariatur"
  },
  {
    "userId": 7,
    "id": 66,
    "name": "Marry Grace Capesos",
    "date": "2025-05-01",
    "title": "repudiandae ea animi iusto",
    "body": "officia veritatis tenetur vero qui itaque\nsint non ratione\nsed et ut asperiores iusto eos molestiae nostrum\nveritatis quibusdam et nemo iusto saepe"
  },
  {
    "userId": 7,
    "id": 67,
    "name": "Angeline Magan",
    "date": "2025-05-04",
    "title": "aliquid eos sed fuga est maxime repellendus",
    "body": "reprehenderit id nostrum\nvoluptas doloremque pariatur sint et accusantium quia quod aspernatur\net fugiat amet\nnon sapiente et consequatur necessitatibus molestiae"
  },
  {
    "userId": 7,
    "id": 68,
    "name": "Zhaira Jane Martinez",
    "date": "2025-05-01",
    "title": "odio quis facere architecto reiciendis optio",
    "body": "magnam molestiae perferendis quisquam\nqui cum reiciendis\nquaerat animi amet hic inventore\nea quia deleniti quidem saepe porro velit"
  },
]
</script>

<template>
  <main>
    <div v-for="post in post" :key="post.id">
      <div class="wrapper">
        <div class="header">
          <span>Written by {{ post.name }} on {{ post.date }}</span>
          <div>
            <button class="del materials-icon">delete</button>
            <button class="save materials-icon">bookmark_border</button>
          </div>
        </div>
        <h2 class="title-box">{{ post.title }}</h2>
        <p class="body-box">{{ post.body }}</p>
      </div>
    </div>
  </main>
</template>

<style>
/* 🌈 Page background */
body {
  margin: 0;
  padding: 0;
  background: linear-gradient(135deg, #ffe0b2, #e1bee7); /* peach to lavender */
  font-family: "Segoe UI", Arial, sans-serif;
}

/* 📦 Card container */
.wrapper {
  max-width: 700px;
  margin: 40px auto;
  padding: 24px;
  background: #fff;
  border-radius: 16px;
  box-shadow: 0 6px 16px rgba(0,0,0,0.12);
}

/* 📌 Header bar */
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: -24px -24px 16px -24px;
  padding: 12px 24px;
  background: #9575cd;   /* lavender */
  border-bottom: 1px solid #d0e3ff;
  color: #fff;           /* white text */
  font-size: 14px;
  border-radius: 16px 16px 0 0;
}

/* 🔘 Buttons */
.materials-icon {
  font-family: "Material Icons";
  font-size: 24px;
  border: none;
  background: transparent;
  cursor: pointer;
  padding: 6px;
  border-radius: 50%;
  transition: background 0.2s, transform 0.2s;
}
.materials-icon:hover {
  background: rgba(0, 0, 0, 0.08);
  transform: scale(1.1);
}
.del {
  color: #f0625d;  /* coral red */
}
.save {
  color: #26a69a;  /* teal green */
}

/* 📝 Title and Body styles */
.title-box {
  background: #ffcc80; /* peach orange */
  color: #4e342e;     /* dark brown text */
  padding: 12px 16px;
  border-radius: 8px;
  font-size: 24px;
  margin-bottom: 16px;
}

.body-box {
  background: #fffde7; /* light cream */
  color: #424242;      /* dark gray text */
  padding: 16px;
  border-radius: 8px;
  line-height: 1.8;
  font-size: 16px;
}
</style>
