<script setup>
import { useEventListener } from '@vueuse/core'
import { useRouter } from 'vue-router/auto'

const router = useRouter()

useEventListener(window, 'keyup', ({ code, defaultPrevented }) => {
  if (defaultPrevented) {
    return // Do nothing if event already handled
  }

  const directionMap = {
    ArrowLeft: -1,
    ArrowRight: 1,
  }

  const direction = directionMap[code]

  if (!direction) {
    return
  }

  const routes = router.getRoutes()
  const currentRoute = router.currentRoute.value

  const currentRouteIndex = routes.findIndex(
    (route) => route.path === currentRoute.path,
  )

  const targetRoute = routes[currentRouteIndex + direction]

  if (!targetRoute || targetRoute.path === '/') {
    // Ignore index route
    return
  }

  router.push(targetRoute)
})
</script>
