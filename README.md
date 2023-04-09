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
header.header>nav.header_nav>.header_logo>a^(.box>(.nav_box_menu>a.header__item_1*7+a.header__item_2)+(.nav_box_JS>a.header__1*4))
`


Результат:
```html
<header class="header">
    <nav class="header_nav">
        <div class="header_logo"><a href=""></a></div>
        <div class="box">
            <div class="nav_box_menu"><a href="" class="header__item_1"></a><a href="" class="header__item_1"></a><a href="" class="header__item_1"></a><a href="" class="header__item_1"></a><a href="" class="header__item_1"></a><a href="" class="header__item_1"></a><a href="" class="header__item_1"></a><a href="" class="header__item_2"></a></div>
            <div class="nav_box_JS"><a href="" class="header__1"></a><a href="" class="header__1"></a><a href="" class="header__1"></a><a href="" class="header__1"></a></div>
        </div>
    </nav>
</header>
```

## b. Блок Form

![Image alt](https://github.com/Hlepa-Hlepa/lab_1-BEM/blob/mybranch/Scren3.png)

Emmet нотация:

form.form>input.form_name+input.form_email+.form_company_position>input.form_company+input.form_position^input.comment+button.btn

Результат:
```html
<form action="" class="form">
    <input type="text" class="form_name"><input type="text" class="form_email">
    <div class="form_company_position"><input type="text" class="form_company"><input type="text" class="form_position"></div>
    <input type="text" class="comment"><button class="btn"></button></form>
```

## c. Блок Card

![Image alt](https://github.com/Hlepa-Hlepa/lab_1-BEM/blob/mybranch/Scren4.png)

Emmet нотация:

.Block_foto_text>.Block_img>img.Picture+.Loader^.Block_text>h5.Headline+p

Результат:
```html
<div class="Block_foto_text">
    <div class="Block_img">
        <img src="" alt="" class="Picture">
        <div class="Loader"></div>
    </div>
    <div class="Block_text">
        <h5 class="Headline"></h5>
        <p></p>
    </div>
</div>
```

## d. Один на выбор студента

![Image alt](https://github.com/Hlepa-Hlepa/lab_1-BEM/blob/mybranch/Scren2.png)

Emmet нотация:

.card>.box_card>img.card_prica*4^.box_card>img.card_prica*4

Результат:
```html
<div class="card">
    <div class="box_card"><img src="" alt="" class="card_prica"><img src="" alt="" class="card_prica"><img src="" alt="" class="card_prica"><img src="" alt="" class="card_prica"></div>
    <div class="box_card"><img src="" alt="" class="card_prica"><img src="" alt="" class="card_prica"><img src="" alt="" class="card_prica"><img src="" alt="" class="card_prica"></div>
</div>
```