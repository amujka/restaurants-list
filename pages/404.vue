<template>
  <div>
    <div class="container">
      <NuxtLayout name="page-not-found">
        <template #errorTitle>
          <h1>page not found</h1>
        </template>

        <template #redirectLink>
          <NuxtLink to="/">return to home</NuxtLink>
        </template>
      </NuxtLayout>
    </div>
  </div>
</template>
