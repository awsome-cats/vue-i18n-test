<template>
  <header class="Header">
    <div class="links">
      <NuxtLink :to="$i18n.path('')">
        {{ $t('links.home') }}
      </NuxtLink>
      <NuxtLink :to="$i18n.path('about')">
        {{ $t('links.about') }}
      </NuxtLink>
      <NuxtLink v-if="$i18n.locale === 'ja'" class="translate" :to="`/en` + $route.fullPath">
        {{ $t('links.en') }}
      </NuxtLink>
      <NuxtLink v-else class="translate" :to="$route.fullPath.replace(/^\/[^\/]+/, '')">
        {{ $t('links.ja') }}
      </NuxtLink>
    </div>
  </header>
</template>
<script>
export default {

}
</script>

<style>

.links {
  display: flex;
  justify-content: center;
  width:100%;
  height:100px;
  background: #ccc;
  margin: 0 auto;
  padding-top: 25px;

}
a {
  color: black;
  padding: 10px 20px;
  margin:10px;

}
.translate {
  margin-left: 300px;
}

</style>
