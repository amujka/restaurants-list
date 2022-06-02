<template>
<div>
    <Header/>
  <div class="container">
      <h1>Welcome to Restaurantly</h1>
      <NuxtLink to="/restaurants">Go to restaurants</NuxtLink>
  </div>

</div>
</template>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  text-decoration: none;
}
.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 100%;
  max-width: 1440px;
  margin: 0 auto;
  border: 1px solid #eee;
}

</style>
