```
- package: ./dynamic-plugins/dist/red-hat-developer-hub-backstage-plugin-global-header
  disabled: false
  pluginConfig:
    app:
      sidebar:
        search: false
        settings: false
    dynamicPlugins:
      frontend:
        red-hat-developer-hub.backstage-plugin-global-header: # the default enabled dynamic header plugin
          mountPoints:
            - mountPoint: application/header
              importName: GlobalHeader
              config:
                position: above-main-content 
            - mountPoint: global.header/component
              importName: SearchComponent
              config:
                priority: 100
            - mountPoint: global.header/component
              importName: Spacer
              config:
                priority: 99
                props:
                  growFactor: 0
            - mountPoint: global.header/component
              importName: HeaderIconButton
              config:
                priority: 90
                props:
                  title: Create...
                  icon: add
                  to: create
            - mountPoint: global.header/component
              importName: SupportButton
              config:
                priority: 80
            - mountPoint: global.header/component
              importName: NotificationButton
              config:
                priority: 70
            - mountPoint: global.header/component
              importName: Divider
              config:
                priority: 50
            - mountPoint: global.header/component
              importName: ProfileDropdown
              config:
                priority: 10
            - mountPoint: global.header/profile
              importName: MenuItemLink
              config:
                priority: 100
                props:
                  title: Settings
                  link: /settings
                  icon: manageAccounts
            - mountPoint: global.header/profile
              importName: LogoutButton
              config:
                priority: 10 #The "Create..." button returns to the sidebar, but the RHDH global header no longer renders at al
```
