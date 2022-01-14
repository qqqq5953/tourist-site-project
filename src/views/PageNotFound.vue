<template>
  <HeaderSectionTest></HeaderSectionTest>
  <h1>404</h1>
  <p>Oops! Page not found!</p>
  <div class="back-to-home">
    <router-link :to="{ name: 'HomeTest' }"> Back to home page </router-link>
  </div>
</template>

<style lang="scss" scoped>
h1 {
  font-size: 80px;
  text-align: center;
  color: $color-primary;
  font-weight: bold;
  margin-bottom: 20px;
  margin-top: 50px;

  @include pad {
    font-size: 50px;
  }

  @include mobile {
    font-size: $font-size-xxl;
  }
}

p {
  font-size: $font-size-xxl;
  text-align: center;
  color: $color-primary;

  @include pad {
    font-size: $font-size-lg;
  }

  @include mobile {
    font-size: 16px;
  }
}

.back-to-home {
  text-align: center;
  margin-top: 50px;

  a {
    @include btn-hover;
    display: inline-block;
    color: $color-primary;
    font-size: $font-size-xxl;
    background-color: $color-primary;
    border-radius: 100px;
    color: white;
    padding: 20px 40px;

    @include pad {
      font-size: $font-size-lg;
      margin-bottom: 50px;
    }

    @include mobile {
      font-size: 16px;
    }
  }
}
</style>
