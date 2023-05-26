# goit-markup-hw-07

<!-- Слова, часто используемые в CSS-классах -->

    https://github.com/yoksel/common-words

<!-- Tottal (мнемоніки) -->

    https://www.toptal.com/designers/htmlarrows/symbols/

<!-- HTML validator -->

    https://validator.w3.org/

<!-- CSS validator -->

    https://jigsaw.w3.org/css-validator/#validate_by_input

<!-- FIGMA -->

    Shift+0 (Show outlines)

<!-- Figma plugins -->

    CSSGen (CSS, RGBA, kebab)
    Font Fascia (Fonts analisys)

<!--  -->

    outline (рамка контейнеру)
    text-align: justify (рівномірне розподіленя тексту в блоці)
    Font family: WendyOne (BANANA c00l fonts)

    display: inline-block (inline to block box)
    vartical-align: middle (to center inline blocks in box)

    margin-left: auto
    margin-right: auto (to center BOX on page)

    2n+1 (even - парні)
         (odd - непарні)
    nth child calculator

<!-- Position -->

    position: absolute (по центру)
    top: 50%;
    left: 50%;
    transform: translate (-50%, -50%);

    is-hidden (щоб клацати за межі модалки)
    opacity: 0;
    pointer-events: none;

<!-- Animation -->

    Бібліотека Animate.css https://animate.style/
    Бібліотека AOS (Анімациї на скрол): https://michalsnik.github.io/aos/
    Приклад анімації shake іконок: https://codepen.io/mpadalko/pen/GRWEWMZ?editors=1100
    Приклад анімації heartbeat: https://codepen.io/mpadalko/pen/JjbErPB?editors=1100
    Модальне вікно ****https://codepen.io/mpadalko/pen/eYreJEL

<!-- FORM -->

    &nbsp - (замість символа " ")
    icon-background - yoksel.github.io/url-encoder/

<!-- Interesting webs -->

    codepen.io (приклади по Grid)

    Бібліотека для накладання маски на елементи форми - https://robinherbots.github.io/Inputmask/

    Генерація фігур - https://bennettfeely.com/clippy/
    Генерація анімацій -https://animista.net/play/basic/swing/swing-left-bck
                        https://animate.style/
    Генерація градієнтів - https://cssgradient.io/
    Генерація фільтрів для фотки - http://www.cssfiltergenerator.com/
    Генерація тіней - https://cssbud.com/css-generator/
    Генерація хвиль для фону - https://getwaves.io/
    Генерація загрузок - https://uiverse.io/
                        https://cssloaders.github.io/ https://whirl.netlify.app/
    Красиві фотки для сайтів - https://www.pexels.com/uk-ua/
    СВГ ілюстрації - https://designstripe.com/ https://undraw.co/illustrations
    Набір іконків свг - https://www.svgrepo.com/
    3д іконки свг - https://3dicons.co/
    Опис термінів "Аккордіон" https://getbootstrap.com/docs/5.3/components/accordion/
    Приклади текстової анімації - animista.net/play/text
    Анімація при скролінгу - AOS (бібліотека JS) - https://michalsnik.github.io/aos/

// Адаптація контентних зображень під ретіна екрани (розмір фіксований)
<img class="team-avatar"
  srcset="./images/team/x/img1_lg-@1x.jpg 1x, ./images/team/x/img1_lg-@2x.jpg 2x"
  src="./images/team/x/img1_lg-@1x.jpg"
  alt="John Smith"
  width="370"
  height="346"
  loading="lazy"
/> Адаптація контентних зображень під ретіна екрани (розмір залежить від типу
пристрою) <img
  class="team-avatar"
  srcset="
    ./images/team/img1-370.jpg 370w,
    ./images/team/img1-418.jpg 418w,
    ./images/team/img1-450.jpg 450w,
    ./images/team/img1-740.jpg 740w,
    ./images/team/img1-836.jpg 836w,
    ./images/team/img1-900.jpg 900w
  "
  sizes="(min-width: 1200px) 370px, (min-width: 768px) 450px, (min-width: 480px) 418px, 100vw"
  src="./images/team/img1-418.jpg"
  alt="John Smith"
  loading="lazy"
/> Адаптація контентних зображень під ретіна екрани (залежно від формату і
кадрування зображення) <picture>

  <!-- Desktop screen -->
  <source
    media="(min-width: 1200px)"
    srcset="./images/gallery/img-1_lg.webp 1x, ./images/gallery/img-1_lg@2x.webp 2x"
    type="image/webp"
  />
  <source
    media="(min-width: 1200px)"
    srcset="./images/gallery/img-1_lg.jpg 1x, ./images/gallery/img-1_lg@2x.jpg 2x"
    type="image/jpg"
  />
  <!-- Tablet screen -->
  <source
    media="(min-width: 768px)"
    srcset="./images/gallery/img-1_md.webp 1x, ./images/gallery/img-1_md@2x.webp 2x"
    type="image/webp"
  />
  <source
    media="(min-width: 768px)"
    srcset="./images/gallery/img-1_md.jpg 1x, ./images/gallery/img-1_md@2x.jpg 2x"
    type="image/jpg"
  />
  <!-- Mobile screen -->
  <source
    media="(max-width: 767px)"
    srcset="./images/gallery/img-1_sm.webp 1x, ./images/gallery/img-1_sm@2x.webp 2x"
    type="image/webp"
  />
  <source
    media="(max-width: 767px)"
    srcset="./images/gallery/img-1_sm.jpg 1x, ./images/gallery/img-1_sm@2x.jpg 2x"
    type="image/jpg"
  />
  <img
    class="card-img"
    src="./images/gallery/img-1_sm.jpg"
    alt="Ноутбук"
    width="450"
    height="294"
    loading="lazy"
  />
</picture>
Адаптація фонових зображень під ретіна екрани
background-repeat: no-repeat;
background-position: center;
background-size: cover;

// Mobile screen background-image: linear-gradient(to right, rgba(47, 48, 58,
0.4), rgba(47, 48, 58, 0.4)), url(../images/price/bg-img_sm-@1x.jpg); // retina
mobile screen @media (min-device-pixel-ratio: 2), (min-resolution: 192dpi),
(min-resolution: 2dppx) { background-image: linear-gradient(to right, rgba(47,
48, 58, 0.4), rgba(47, 48, 58, 0.4)), url(../images/price/bg-img_sm-@2x.jpg); }

// Tablet screen @media screen and (min-width: 481px) { background-image:
linear-gradient(to right, rgba(47, 48, 58, 0.4), rgba(47, 48, 58, 0.4)),
url(../images/price/bg-img_md-@1x.jpg); // retina tablet screen @media
(min-device-pixel-ratio: 2), (min-resolution: 192dpi), (min-resolution: 2dppx) {
background-image: linear-gradient(to right, rgba(47, 48, 58, 0.4), rgba(47, 48,
58, 0.4)), url(../images/price/bg-img_md-@2x.jpg); } }

// Desktop screen @media screen and (min-width: 769px) { background-image:
linear-gradient(to right, rgba(47, 48, 58, 0.4), rgba(47, 48, 58, 0.4)),
url(../images/price/bg-img_lg-@1x.jpg); // retina desktop screen @media
(min-device-pixel-ratio: 2), (min-resolution: 192dpi), (min-resolution: 2dppx) {
background-image: linear-gradient(to right, rgba(47, 48, 58, 0.4), rgba(47, 48,
58, 0.4)), url(../images/price/bg-img_lg-@2x.jpg); } }
