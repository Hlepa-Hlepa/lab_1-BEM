# С помощью BEM описать человеческое тело

    голова
        голова__глаза--голубые
        голова__волосы--светлые
        голова__нос
    тело
        тело__спина
        тело__плечи
        тело__шея
    рука
        рука__локоть
        рука__запястье
        рука__пальцы--длинные

# Подготовить создание 4 различных блоков из макета в нотации Emmet

## a. Блок Header

![Image alt](Scren1.png)

Emmet нотация:

`
header.header>nav.header__nav>.header__logo>a^(.box>(.nav__box--menu>a.header__item--a*7+a.header__item--btn)+(.nav__box--JS>a.header__item--a*4))
`


Результат:
```html
<header class="header">
    <nav class="header__nav">
        <div class="header__logo"><a href=""></a></div>
        <div class="box">
            <div class="nav__box--menu"><a href="" class="header__item--a"></a><a href="" class="header__item--a"></a><a href="" class="header__item--a"></a><a href="" class="header__item--a"></a><a href="" class="header__item--a"></a><a href="" class="header__item--a"></a><a href="" class="header__item--a"></a><a href="" class="header__item--btn"></a></div>
            <div class="nav__box--JS"><a href="" class="header__item--a"></a><a href="" class="header__item--a"></a><a href="" class="header__item--a"></a><a href="" class="header__item--a"></a></div>
        </div>
    </nav>
</header>
```

## b. Блок Form

![Image alt](Scren3.png)

Emmet нотация:

`
form>input.field__message*2+.form__line>input.field__message*2^input.field__message--textarea+button.btn
`

Результат:
```html
<form action="">
    <input type="text" class="field__message">
    <input type="text" class="field__message">
    <div class="form__line">
        <input type="text" class="field__message">
        <input type="text" class="field__message">
    </div>
    <input type="text" class="field__message--textarea">
    <button class="btn"></button>
</form>
```

## c. Блок Card

![Image alt](Scren4.png)

Emmet нотация:

`
.card>img.card__photo.card__description+p.card__description--text*2
`

Результат:
```html
<div class="card">
    <img src="" alt="" class="card__photo card__description">
    <p class="card__description--text"></p>
    <p class="card__description--text"></p>
</div>
```

## d. Один на выбор студента

![Image alt](Scren2.png)

Emmet нотация:

`
.
.partners>.partners__block>img.partners__block--photo*4^.partners__block>img.partners__block--photo*4
`

Результат:
```html
<div class="partners">
    <div class="partners__block">
        <img src="" alt="" class="partners__block--photo">
        <img src="" alt="" class="partners__block--photo">
        <img src="" alt="" class="partners__block--photo">
        <img src="" alt="" class="partners__block--photo">
    </div>
    <div class="partners__block">
        <img src="" alt="" class="partners__block--photo">
        <img src="" alt="" class="partners__block--photo">
        <img src="" alt="" class="partners__block--photo">
        <img src="" alt="" class="partners__block--photo">
    </div>
</div>
```