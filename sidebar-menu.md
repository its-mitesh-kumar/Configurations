```
dynamicPlugins:
  frontend:
    default.main-menu-items:
      menuItems:
        default.home:
          title: Home
          icon: home
          enabled: false
        default.list:
          title: References
          icon: bookmarks
        default.my-group:
          parent: default.list
        default.learning-path:
          parent: default.list
          title: ''
        default.homepage:
          title: HomePage 123
          icon: home
          enabled: false
        default.create:
          title: Create
          icon: add
          parent: default.homepage
```
```
app:
  sidebar:
    search: false # hides sidebar search
    logo: false # hides sidebar logo
    settings: false # hides settings item
    administration: false # hides administration item
```
