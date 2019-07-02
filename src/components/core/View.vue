<template>
  <div>
    <welcome />
    <about-me />
    <recent-projects />
    <services />
    <get-in-touch />
  </div>
</template>

<script>
export default {
  components: {
    AboutMe: () => import('@/components/AboutMe'),
    GetInTouch: () => import('@/components/GetInTouch'),
    RecentProjects: () => import('@/components/RecentProjects'),
    Services: () => import('@/components/Services'),
    Welcome: () => import('@/components/Welcome')
  }
}
</script>
