<!--laravelvuejs_Home_M.png-->
<template>
  <section>
    <app-header/>
    <div class="container">
      <adsbygoogle  class="adsbygoogle"/>
    </div>
    <app-featured/>
    <div class="container">
      <adsbygoogle  class="adsbygoogle"/>
    </div>
    <div class="main-posts">
      <div class="container">
        <div class="posts-wrapper">
          <app-feed/>
          <app-aside/>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    name: 'index',
    components: {
      AppHeader: () => import('@/components/web/partials/app-header'),
      AppFeatured: () => import('@/components/web/partials/app-featured'),
      AppFeed: () => import('@/components/web/partials/app-feed'),
      AppAside: () => import('@/components/web/partials/app-aside'),
    },
    data() {
      return {}
    }
  }

</script>

<style lang="stylus" scoped>
  .main-posts
    padding 60px 0 80px

  .posts-wrapper
    display flex
    justify-content space-between
</style>
