# References
## [How to Deploy an Angular Application to GitHub](https://dzone.com/articles/how-to-deploy-an-angular-application-to-github)
```cmd
npm install -g angular-cli-ghpages 
ng build --prod --base-href https://PublicWC.github.io/angular-demo/ 
ngh --no-silent --dir dist/demo
```

## [Can't bind to 'ngModel' since it isn't a known property of 'input'](https://stackoverflow.com/questions/38892771/cant-bind-to-ngmodel-since-it-isnt-a-known-property-of-input)
src/app/app.module.ts
```typescript
import { FormsModule } from '@angular/forms';

[...]

@NgModule({
  imports: [
    [...]
    FormsModule
  ],
  [...]
})
```
