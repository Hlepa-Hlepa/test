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

![Image alt](https://github.com/Hlepa-Hlepa/lab_1-BEM/blob/mybranch/Scren1.png)

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

![Image alt](https://github.com/Hlepa-Hlepa/lab_1-BEM/blob/mybranch/Scren3.png)

Emmet нотация:

`
form.form>input.form__name+input.form__email+.form__company--position>input.form__company+input.form__position^input.comment+button.btn
`

Результат:
```html
<form action="" class="form">
    <input type="text" class="form__name"><input type="text" class="form__email">
    <div class="form__company--position"><input type="text" class="form__company"><input type="text" class="form__position"></div>
    <input type="text" class="comment"><button class="btn"></button>
</form>
```

## c. Блок Card

![Image alt](https://github.com/Hlepa-Hlepa/lab_1-BEM/blob/mybranch/Scren4.png)

Emmet нотация:

`
.Block__foto--text>.Block__img>img.Picture+.Loader^.Block__text>h5.Headline+p
`

Результат:
```html
<div class="Block__foto--text">
    <div class="Block__img">
        <img src="" alt="" class="Picture">
        <div class="Loader"></div>
    </div>
    <div class="Block__text">
        <h5 class="Headline"></h5>
        <p></p>
    </div>
</div>
```

## d. Один на выбор студента

![Image alt](https://github.com/Hlepa-Hlepa/lab_1-BEM/blob/mybranch/Scren2.png)

Emmet нотация:

`
.card>.box__card>img.card__prica*4^.box__card>img.card__prica*4
`

Результат:
```html
<div class="card">
    <div class="box__card"><img src="" alt="" class="card__prica"><img src="" alt="" class="card__prica"><img src="" alt="" class="card__prica"><img src="" alt="" class="card__prica"></div>
    <div class="box__card"><img src="" alt="" class="card__prica"><img src="" alt="" class="card__prica"><img src="" alt="" class="card__prica"><img src="" alt="" class="card__prica"></div>
</div>
```