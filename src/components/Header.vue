<template>
  <header>
    <img class="logo" src="../assets/IMG_0674.gif" @click="$router.push('/')">
    <div class="header-nav">
      <p @click="$router.push('/menu')">メニュー</p>
      <p @click="$router.push('/store')">店舗情報</p>
      <p @click="$router.push('/news')">お知らせ</p>
      <p @click="$router.push('/contact')">お問い合わせ</p>
    </div>
  </header>
</template>

<style scoped>
header{
  padding: 20px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
header img:hover{
  opacity: 0.5;
}
.header-nav{
  display: flex;
}
.header-nav p{
  margin: 0 40px 0;
  cursor: pointer;
}
.header-nav p:hover{
  color: rgb(131, 131, 131);
}
</style>