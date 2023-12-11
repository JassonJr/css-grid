# CSS - Grid

Na aula de hoje aprendemos sobre estilização de páginas e elementos utilizando o Grid do CSS. 

Aprendemos como criar o template de um sistema de linhas e colunas para um elemento da página com:
```css
.conteiner {
    height: 100%;
    display: grid;
    grid-template-rows: repeat(3, 1fr);
    grid-template-columns: repeat(7, 1fr);
}
```

Tembém aprendemos a utilizar `grid-row-start`, `grid-row-end`,`grid-column-start`,`grid-column-end`, para podermos definir quais partes do nosso container grid o elemento filho irá ocupar.

```css
.elemento1 {
    grid-row-start: 1;
    grid-row-end: -1;
    grid-column-start: 1;
    grid-column-end: span 3;
}
```

Aprendemos a reduzir estas quatro linhas de código para apenas duas linhas, utilizando `grid-row` e `grid-column`.

```css
.elemento2 {
    grid-row: 1 / 3;
    grid-column: 4 / -1;
}
```

Em seguida reduzimos estas duas linhas para apenas uma utilizando `grid-area`.

```css
.elemento3 {
    grid-area: 3 / 4 / 3 / span 2;
}

.elemento4 {
    grid-area: 3 / 6/ -1 / span 2;
}
```


