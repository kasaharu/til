## * は ng-template のシンタックスシュガー
```html
<div *ngIf="hero" class="name">{{hero.name}}</div>

<!-- 上と同義 -->
<ng-template [ngIf]="hero">
  <div class="name">{{hero.name}}</div>
</ng-template>
```



## Input プロパティへのバインド
- 以下のようにショートハンドで書ける (ref. [inputプロパティへのバインド](https://angular.jp/guide/attribute-directives#inputプロパティへのバインド))

```html
<p [appHighlight]="color">Highlight me!</p>
```

```ts
@Input() appHighlight: string;
```

## Unit Test
- directive を使用するテスト用のコンポーネントを用意
- テスト用のコンポーネントから fixture を生成し `debugElement.query` で DebugElement を取り出す
- DebugElement に対して `triggerEventHandler()` をすると期待する event を発火できる

```ts
// example
import { Component, DebugElement } from '@angular/core';
import { ComponentFixture, TestBed } from '@angular/core/testing';
import { By } from '@angular/platform-browser';
import { TestDirective } from './test.directive';

@Component({
  template: `<button testDir></button>`,
})
class TestComponent {}

describe('TestDirective', () => {
  let fixture: ComponentFixture<TestComponent>;
  let buttonEl: DebugElement;

  beforeEach(() => {
    TestBed.configureTestingModule({
      declarations: [TestComponent, TestDirective],
    });

    fixture = TestBed.createComponent(TestComponent);
    fixture.detectChanges();
    buttonEl = fixture.debugElement.query(By.directive(TestDirective));
  });

  it('sample', () => {
    buttonEl.triggerEventHandler('click', {});
    fixture.detectChanges();

    expect();
  });
});

```
