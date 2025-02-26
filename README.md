# Flexbox: O que é e como usar

Flexbox (Flexible Box) é um modelo de layout do CSS que permite organizar elementos de forma eficiente dentro de um contêiner, distribuindo espaço e alinhando itens de maneira responsiva.

## Como usar

1. **Definir um contêiner flexível:**
   ```css
   .container {
       display: flex;
   }
   ```

2. **Propriedades do contêiner:**
   - `flex-direction`: Define a direção dos itens (`row`, `column`, `row-reverse`, `column-reverse`).
   - `justify-content`: Alinha os itens no eixo principal (`flex-start`, `center`, `space-between`, etc.).
   - `align-items`: Alinha os itens no eixo perpendicular (`flex-start`, `center`, `stretch`, etc.).
   - `flex-wrap`: Define se os itens devem quebrar linha (`nowrap`, `wrap`, `wrap-reverse`).

3. **Propriedades dos itens flexíveis:**
   - `flex-grow`: Define a capacidade do item de crescer dentro do contêiner.
   - `flex-shrink`: Define se o item pode diminuir caso necessário.
   - `flex-basis`: Define o tamanho inicial do item.
   - `align-self`: Alinha um item específico de forma diferente dos demais.

## Exemplo Completo

```css
.container {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
}

.item {
    flex: 1;
    padding: 10px;
    background-color: lightblue;
    margin: 5px;
}
```

```html
<div class="container">
    <div class="item">Item 1</div>
    <div class="item">Item 2</div>
    <div class="item">Item 3</div>
</div>
```

Flexbox facilita a criação de layouts responsivos e alinhamentos complexos de forma simples e eficiente!
