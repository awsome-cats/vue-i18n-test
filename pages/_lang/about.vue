<template>
  <div class="container">
    <h3 class="title">
      {{ $t('about.title') }}
    </h3>
    <p class="subtitle">
      {{ $t('about.introduction') }}
    </p>
  </div>
</template>

<script>

export default {
}
</script>

<style scoped>
.container {
  min-height: 100vh;
  display:flex;
  flex-direction: column;
}
.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  margin-bottom:30px;
  font-weight: 300;
  font-size: 30px;
  color: #35495e;
  letter-spacing: 1px;
  text-align:center;
  margin-top:50px;

}

.subtitle {
  margin:0 auto;
  width: 100%;
  max-width:500px;
  font-weight: 500;

  color: #304e8a;

  word-spacing: 5px;
  padding-bottom: 15px;

}

</style>
