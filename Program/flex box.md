https://tpverstak.ru/flex-cheatsheet/

позволяет выстраивать элементы в один ряд по горизонтали и вертикали 

```css
.row {
  display : flex;
}
```


- align-items - выравнивает элементы по вертикали
- justify-content - выравнивает элементы по горизонтали   
- gap - задает отступы между flex элементами, прописывается во flex контейнере 
```css
.parent{
gap : 10px;
}
```
- flex-direction: column - меняет направление flex контейнера 