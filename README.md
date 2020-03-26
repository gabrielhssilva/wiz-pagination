# @wizsolucoes WizToggle
Modulo Angular 4+

## Configuração do módulo (app.module.ts)

Módulo simples de modal.

```ts
import { WizToggleModule } from '@wizsolucoes/wiz-toggle';

@NgModule({
  declarations: [],
  imports: [
    WizToggleModule,
  ]

```

## Chamando componente no HTML (.component.html)

Chamando o componente no html

```html
<wiz-toggle [disabled]=false (returnEvent)="teste($event)">
  Ativar
</wiz-toggle>

```

> **disabled:** *Desabilitar input*

```ts
  [disabled]=false
  [disabled]=true
```

> **(returnEvent)="teste($event)":** *Evento emitido*

app.component.ts
```ts
  teste(e) {
    console.log(e);
  }
```
