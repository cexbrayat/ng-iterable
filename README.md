# NgIterable

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 9.0.0-rc.0.

## Template

```html
<div *ngFor="let user of users | slice: 0:2 as total">
  {{ total.length }}: {{ user.name }}
</div>
```

## Error

With `fullTemplateTypeCheck: true` throws:

```
ERROR in src/app/app.component.html:2:6 - error TS2339: Property 'length' does not exist on type 'NgIterable<any>'.
  Property 'length' does not exist on type 'Iterable<any>'.

2   {{ total.length }}: {{ user.name }}
       ~~~~~~~~~~~~~

  src/app/app.component.ts:5:16
    5   templateUrl: './app.component.html',
                     ~~~~~~~~~~~~~~~~~~~~~~
    Error occurs in the template of component AppComponent.
```
