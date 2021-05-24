# ngx-numeric-textbox

An Angular numeric textbox component

## Dependencies

- [Angular](https://angular.io)
- [Lodash](https://lodash.com)
- [Numeral](http://numeraljs.com)
- [Bootstrap 4 alpha 6](https://v4-alpha.getbootstrap.com)

You can customize CSS yourself to break down dependencies to Bootstrap.

## Demo

[https://github.com/GStoynev/ngx-numeric-textbox/](https://github.com/GStoynev/ngx-numeric-textbox/)

## Installation

After install the above dependencies, install `ngx-numeric-textbox-upd` via:

```shell
npm install ngx-numeric-textbox-upd --save
```

Once installed you need to import our main module in your application module:

```js
import { NumericTextboxModule } from 'ngx-numeric-textbox-upd';

@NgModule({
  declarations: [
    AppComponent,
    ...
  ],
  imports: [
    FormsModule,
    NumericTextboxModule,
    ...
  ],
  bootstrap: [
    AppComponent
  ]
})
export class AppModule {
}
```

## Usage

```html
<ngx-numeric-textbox
  [min]="min"
  [max]="max"
  [disabled]="disabled"
  [decimals]="decimals"
  [format]="format"
  [placeholder]="placeholder"
  [rangeValidation]="rangeValidation"
  [(ngModel)]="value"
  (focus)="onFocus()"
  (blur)="onBlur()"
  (enter)="onEnter()"
  (escape)="onEscape()"
  (ngModelChange)="ngModelChange($event)"
>
</ngx-numeric-textbox>
```

- format string: http://numeraljs.com/#format

## Contributing

I am very appreciate for your ideas, proposals and found bugs which you can leave in github issues. Thanks in advance!
