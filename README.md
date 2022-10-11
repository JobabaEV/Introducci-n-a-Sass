# Introduccion a Sass
Introducción a Sass


## Ejercicios

1. Instalar Sass en la máquina del pool TWFE

```
$ sudo apt-get install ruby

$ sudo gem install sass

$ sass -v
```
2. Escribir el código Sass que simplifique las reglas CSS:
```css
header {
    background-color: #531946;
  }
  .header a {
    color: #fff;
  }
  .header a:hover {
    color: #095169;
  }
  
  .footer {
    background-color: #30162B;
    color: #fff;
  }
  .footer a {
    color: #095169;
  }
  .footer a:hover {
    color: #fff;
  }
  
  .feature a {
    background-color: #30162B;
    color: #fff;
  }
  
  .feature a:hover {
    color: #531946;
  }
  
  .content {
    background-color: #fff;
    color: #222;
  }
```
**Solucion:**
```sass
header
  background-color: #531946

.header a
  color: #fff

  &:hover
    color: #095169

.footer
  background-color: #30162B
  color: #fff

  a
    color: #095169

    &:hover
      color: #fff

.feature a
  background-color: #30162B
  color: #fff

  &:hover
    color: #531946

.content
  background-color: #fff
  color: #222
 ``` 

3. Escribir el código Sass más simplificado posible que genere:

```css
.header {
    background-color: #531946;
    border-radius: 5px;
    padding: 5px 20px;
  }
  .header a {
    color: #fff;
  }
  .header a:hover {
    color: #095169;
  }
  
  .footer {
    background-color: #30162B;
    color: #fff;
    border-radius: 5px;
    padding: 5px 20px;
  }
  .footer a {
    color: #095169;
  }
  .footer a:hover {
    color: #fff;
  }
  
  .feature a {
    background-color: #30162B;
    color: #fff;
    border-radius: 5px;
    padding: 5px 20px;
  }
  .feature a:hover {
    color: #531946;
  }
  
  .content {
    background-color: #fff;
    color: #222;
    border-radius: 5px;
    padding: 5px 20px;
  }
```

**Solucion:**
```sass
.header
  background-color: #531946
  border-radius: 5px
  padding: 5px 20px

  a
    color: #fff

    &:hover
      color: #095169

.footer
  background-color: #30162B
  color: #fff
  border-radius: 5px
  padding: 5px 20px

  a
    color: #095169

    &:hover
      color: #fff

.feature a
  background-color: #30162B
  color: #fff
  border-radius: 5px
  padding: 5px 20px

  &:hover
    color: #531946

.content
  background-color: #fff
  color: #222
  border-radius: 5px
  padding: 5px 20px
  ```


4. Dado el código HTML a continuación, escribir el código Sass para los estilos css que se incluyen:
```html
<nav class="navigation">
  <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#about">About</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>
```

Código CSS esperado:

```css

.navigation {
  float: right;
}
.navigation li {
  display: inline-block;
  list-style-type: none;
  margin-left: 1.5em;
}
.navigation a {
  display: block;
  text-decoration: none;
}
```

**Solucion:**
```sass
.navigation
  float: right

  li
    display: inline-block
    list-style-type: none
    margin-left: 1.5em

  a
    display: block
    text-decoration: none
 ```


5. Crear el código Sass adecuado para obtener el CSS a continución:
```ruby
 a {
    color: #beedee;
  }
  
  a:hover {
    color: #cbbebb;
  }
  
  a.btn {
    background: #deede6;
  }
  
  a .btn {
    display: block;
  }
```

**Solucion:**
```sass
a
  color: #beedee

  &:hover
    color: #cbbebb

  &.btn
    background: #deede6

  .btn
    display: block
    ```

6. Crear el código Sass más estructurado posible que genere el código CSS:

```css
header {
    border-radius: 5px;
    padding: 5px 20px;
  }
  
  .footer {
    border-radius: 5px;
    padding: 5px 20px;
  }
  
  .feature a {
    border-radius: 5px;
    padding: 5px 20px;
  }
  
  .content {
    border-radius: 5px;
    padding: 5px 20px;

  }
  ```
  
  **Solucion:**
  ```sass
  header, .footer, .feature a, .content
  border-radius: 5px
  padding: 5px 20px
  ```
  
  
  
 7. Crear el código Sass más estructurado posible que genere el código CSS:

```css
  .header {
    -webkit-border-radius: 5px;
       -moz-border-radius: 5px;
            border-radius: 5px;
    /* ... */
  }
  
  .footer {
    -webkit-border-radius: 10px;
       -moz-border-radius: 10px;
            border-radius: 10px;
    /* ... */
  }
 ```
 
 **Solucion:**
 ```sass
 .header
  -webkit-border-radius: 5px
  -moz-border-radius: 5px
  border-radius: 5px

  /* ...

.footer
  -webkit-border-radius: 10px
  -moz-border-radius: 10px
  border-radius: 10px

  /* ...
  ```
 
