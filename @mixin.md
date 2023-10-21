это позволяет писать модульные решения в SCSS
в @mixin вношу повторяющейся код.
в @mixin вносятся глобальные решения используемые по всему проекту 
миксин для адабтива :
```scss
@mixin breakpoint($point) {
  @if $point == xl {
    @media(max-width: 1200px) { @content; }
  }
  @else if $point == lg {
    @media(max-width: 1024px) { @content; }
  }
  @else if $point == md {
    @media(max-width: 768px) { @content; }
  }
  @else if $point == sm {
    @media(max-width: 576px) { @content; }
  }
  @else if $point == xs {
    @media(max-width: 360px) { @content; }
  }
}

```
вызов и иммпорт миксина:
```scss
@import "@/styles/config/mixin"

@include breakpoint(lg) {
  justify-content: flex-start;
  padding-right: 30px;
}

@include breakpoint(md) {
  margin: auto;
}

@include breakpoint(sm) {
  padding: 8px;
  gap: 11px;
}

```
