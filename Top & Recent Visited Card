```
dynamicPlugins:
  rootDirectory: dynamic-plugins-root
  frontend:
    red-hat-developer-hub.backstage-plugin-dynamic-home-page:
      dynamicRoutes:
        - path: /
          importName: DynamicHomePage
      mountPoints:
        - mountPoint: application/listener
          importName: VisitListener
        - mountPoint: home.page/cards
          importName: RecentlyVisitedCard
          config:
            layouts:
              xl: { w: 6, h: 4, x: 6 }
              lg: { w: 6, h: 4, x: 6 }
              md: { w: 6, h: 4, x: 6 }
              sm: { w: 6, h: 4, x: 6 }
              xs: { w: 6, h: 4, x: 6 }
              xxs: { w: 6, h: 4, x: 6 }
        - mountPoint: home.page/cards
          importName: TopVisitedCard
          config:
            layouts:
              xl: { w: 6, h: 4 }
              lg: { w: 6, h: 4 }
              md: { w: 6, h: 4 }
              sm: { w: 6, h: 4 }
              xs: { w: 6, h: 4 }
              xxs: { w: 6, h: 4 }
```
