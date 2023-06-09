### index.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Grid Layout</title>
</head>
<body>
    <div class="grid-container">
        <div class="grid__header"></div>

        <div class="grid__item card__1"></div>
        <div class="grid__item card__2"></div>
        <div class="grid__item card__3"></div>

        <div class="grid__item card__4"></div>
        <div class="grid__item card__5"></div>
        <div class="grid__item card__6"></div>

        <div class="grid__item card__7"></div>
        <div class="grid__item card__8"></div>
        <div class="grid__item card__9"></div>

        <div class="grid__item card__10"></div>
        <div class="grid__item card__11"></div>
        <div class="grid__item card__12"></div>

    </div>
</body>
</html>
```

### style.css
```css
body {
    margin: 0;
    padding: 0;
}

.grid-container {
    display: grid;
    gap: 4px;
}

.grid__header {
    height: 60px;
    background-color: antiquewhite;
}

.grid__item {
    height: 240px;
    background-color: antiquewhite;
}

/* tablet */
@media only screen and (min-width: 640px) {

    .grid-container {
        grid-template-columns: repeat(2, 1fr);
    }
    
    .grid__header {
        grid-row-start: 1;
        grid-row-end: 2;
        grid-column: 1/3;
        height: 40px;
    }

    .card__1 {
        grid-row-start: 2;
        grid-row-end: 3;
    }

    .card__2 {
        grid-row-start: 2;
        grid-row-end: 3;
    }

    .card__3 {
        grid-row-start: 3;
        grid-row-end: 4;
    }

    .card__4 {
        grid-row-start: 3;
        grid-row-end: 4;
    }

    .card__5 {
        grid-row-start: 4;
        grid-row-end: 5;
    }

    .card__6 {
        grid-row-start: 4;
        grid-row-end: 5;
    }

    .card__7 {
        grid-row-start: 5;
        grid-row-end: 6;
    }

    .card__8 {
        grid-row-start: 5;
        grid-row-end: 6;
    }

    .card__9 {
        grid-row-start: 6;
        grid-row-end: 7;
    }

    .card__10 {
        grid-row-start: 6;
        grid-row-end: 7;
    }

    .card__11 {
        grid-row-start: 7;
        grid-row-end: 8;
    }

    .card__12 {
        grid-row-start: 7;
        grid-row-end: 8;
    }

}

@media only screen and (min-width: 768px) {
    .grid-container {
        grid-template-columns: repeat(3, 1fr);
    }
    
    .grid__header {
        grid-row-start: 1;
        grid-row-end: 2;
        grid-column: 1/4;
        height: 40px;
    }

    .card__1 {
        grid-row-start: 2;
        grid-row-end: 3;
    }

    .card__2 {
        grid-row-start: 2;
        grid-row-end: 3;
    }

    .card__3 {
        grid-row-start: 2;
        grid-row-end: 3;
    }

    .card__4 {
        grid-row-start: 3;
        grid-row-end: 4;
    }

    .card__5 {
        grid-row-start: 3;
        grid-row-end: 4;
    }

    .card__6 {
        grid-row-start: 3;
        grid-row-end: 4;
    }

    .card__7 {
        grid-row-start: 4;
        grid-row-end: 5;
    }

    .card__8 {
        grid-row-start: 4;
        grid-row-end: 5;
    }

    .card__9 {
        grid-row-start: 4;
        grid-row-end: 5;
    }

    .card__10 {
        grid-row-start: 5;
        grid-row-end: 6;
    }

    .card__11 {
        grid-row-start: 5;
        grid-row-end: 6;
    }

    .card__12 {
        grid-row-start: 5;
        grid-row-end: 6;
    }
}

/* laptop */
@media only screen and (min-width: 1024px) {
    .grid-container {
        grid-template-columns: repeat(4, 1fr);
    }
    
    .grid__header {
        grid-row-start: 1;
        grid-row-end: 2;
        grid-column: 1/5;
        height: 40px;
    }

    .card__1 {
        grid-row-start: 2;
        grid-row-end: 3;
    }

    .card__2 {
        grid-row-start: 2;
        grid-row-end: 3;
    }

    .card__3 {
        grid-row-start: 2;
        grid-row-end: 3;
    }

    .card__4 {
        grid-row-start: 2;
        grid-row-end: 3;
    }

    .card__5 {
        grid-row-start: 3;
        grid-row-end: 4;
    }

    .card__6 {
        grid-row-start: 3;
        grid-row-end: 4;
    }

    .card__7 {
        grid-row-start: 3;
        grid-row-end: 4;
    }

    .card__8 {
        grid-row-start: 3;
        grid-row-end: 4;
    }

    .card__9 {
        grid-row-start: 4;
        grid-row-end: 5;
    }

    .card__10 {
        grid-row-start: 4;
        grid-row-end: 5;
    }

    .card__11 {
        grid-row-start: 4;
        grid-row-end: 5;
    }

    .card__12 {
        grid-row-start: 4;
        grid-row-end: 5;
    }
}

/* desktop */
@media only screen and (min-width: 1280px) {

    .grid-container {
        gap: 4px;
    }

    .grid__header {
        height: 48px;
    }
}
```
