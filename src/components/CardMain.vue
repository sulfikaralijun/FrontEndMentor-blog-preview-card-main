
<script setup>
import banner from '../assets/images/illustration-article.svg'
import avatar from '../assets/images/image-avatar.webp'
</script>

<template>
  <div class="card">
    <div class="card-header">
      <img :src="banner" alt="illustration-article">
      <div class="tag">
        <strong>Learning</strong>
      </div>
      <div class="date-publish">
        <span>Published 21 Dec 2023</span>
      </div>
    </div>

    <div class="card-body">
      <h1 class="title">HTML & CSS foundations</h1>
      <div class="description">
        <p>These languages are the backbone of every website, defining structure, content, and presentation.</p>
      </div>
    </div>

    <div class="card-footer">
      <img :src="avatar" alt="image-avatar">
      <h3>Greg Hooper</h3>
    </div>
  </div>
</template>

<style scoped>
.card {
  width: 370px;
  padding: 20px;
  background-color: hsl(0, 0%, 100%);
  border-radius: 20px;
  position: relative;
  display: flex;
  flex-direction: column;
  border: 1px solid hsl(0, 0%, 7%);
  box-shadow: 8px 8px hsl(0, 0%, 7%);
}
/* Card header Style */
.card .card-header {
  display: flex;
  flex-direction: column;
}
.card-header img {
  width: 100%;
  height: 100%;
  border-radius: 10px;
  object-fit: cover;
}
.card-header .tag {
  margin-top: 20px;
}
.card-header .tag strong {
  background-color: hsl(47, 88%, 63%);
  padding: 6px 10px;
  border-radius: 5px;
}
.card-header .date-publish {
  margin-top: 15px;
}
.date-publish span {
  font-weight: 500;
  font-size: 14px;
}

/* Card Body Style */
.card .card-body {
  margin-top: 18px;
}
.card-body .title {
  font-size: 24px;
}
.card-body .description {
  margin-top: 15px;
}
.description p {
  font-size: 16px;
  color: hsl(0, 0%, 50%);
  line-height: 20px;
}
/* Card Footer Style */
.card .card-footer {
  display: flex;
  align-items: center;
  margin-top: 20px;
  gap: 15px;
}
.card-footer img{
  width: 30px;
}
.card-footer h3 {
  font-size: 16px;
}
</style>