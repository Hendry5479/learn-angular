# learn-angular
take some notes about learning of angular

``` JavaScript
app.module.ts
  @NgModule({
      imports: [CoreModule]
  })
  exports class AppMoudle {}
app.html
  <header>
    <app-header></app-header>
  </header>
  <main></main>
  <footer>
    <app-footer></app-footer>
  </footer>

core
  header
  footer
  sidebar
  core.module.ts
    @NgModule({
      imports:
      declarations:
      exports:
    })

    exports class CoreModule {
      consturctor(@optional @skipself parent: CoreModule) {
        ...
      }
    }

    
        
```