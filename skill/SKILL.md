---
name: uppora-deck
description: Делать презентации и одностраничники в фирменном стиле Uppora (для блогеров, партнёров, амбассадоров): готовые цвета, шрифты, ассеты и шаблоны слайдов.
---

# Презентации в стиле Uppora

Uppora (uppora.org) — сервис разовых донатов для авторов. Пример готовой презентации лежит в папке `templates/`.

## Как делать

1. Создай презентацию из типа Slides (Artifact quickstart, intent slides; design_systems: false).
2. Ассеты: загрузи файлы из `assets/` в новую презентацию как ассеты (asset:true, можно все сразу через file_paths) и используй /_blob/ url из ответа.
3. deck.json + слайды по шаблону из `templates/example/` (адаптируй готовый слайд, а не верстай с нуля; картинки в шаблоне замени на свои /_blob/ url).

## Шрифты (faces в deck.json)

```json
"faces":{"montserrat":{"family":"Montserrat","href":"https://fonts.googleapis.com/css2?family=Montserrat:wght@500..800&display=swap"},"manrope":{"family":"Manrope","href":"https://fonts.googleapis.com/css2?family=Manrope:wght@400..700&display=swap"}}
```
Заголовки Montserrat 800, letter-spacing -1px. Текст Manrope. Шкала: 112–120 / 72 / 44 / 32 / 26–28 / 24.

## Цвета

- акцент #00A63E; на тёмном #22C55E; мелкий зелёный текст на светлом #00843A
- тёмный #121512, текст #4B524C, вторичный #6B726C, на тёмном #C9D1CA / #F6F8F4
- фоны: #F7F8F5 (основной), #E6F5EA (раздел), #00A63E (заявление), #121512 (большая цифра)
- на зелёном фоне текст тёмный #121512

## Фирменные приёмы

- Зелёная плашка-маркер: `<p style="font-family:'Montserrat', Arial, sans-serif;font-size:48px;font-weight:700;color:#121512;background:#00A63E;padding:4px 24px 10px;border-radius:20px">…</p>`
- Знак U с точкой (обложка, справа):
  `<svg aria-label="Знак Uppora" viewBox="0 0 520 640" width="520" height="640" style="position:absolute;left:1272px;top:240px;width:520px;height:640px"><path d="M90 0 V350 A170 170 0 0 0 430 350 V0" fill="none" stroke="#00A63E" stroke-width="120" stroke-linecap="round"/><circle cx="260" cy="350" r="78" fill="#121512"/></svg>`
- Белая арка на зелёном слайде (правый верхний угол):
  `<svg aria-label="" viewBox="0 0 440 440" width="440" height="440" style="position:absolute;right:0px;top:0px;width:440px;height:440px"><path d="M90 -20 V230 A130 130 0 0 0 350 230 V-20" fill="none" stroke="#F6F8F4" stroke-width="100"/><circle cx="220" cy="230" r="62" fill="#F6F8F4"/></svg>`
- Обложка: фон `radial-gradient(circle at 82% 62%, #C6EFD4 0%, #F7F8F5 52%)`, логотип 284×60 сверху слева.
- Карточка: `background:#FFFFFF;padding:36px 40px;border-radius:32px;box-shadow:0px 8px 32px rgba(18,21,18,0.06)`; акцентная — зелёная или тёмная.
- Эйбрау-пилюля раздела: Montserrat 24px 700 uppercase, letter-spacing 2px, фон #00A63E, border-radius 999px.
- Футер (padding слайда 128px 128px 160px): логотип `position:absolute;left:128px;bottom:64px;width:142px;height:30px` + номер справа 24px #6B726C.
- Финал: фон #F7F7F7, фото руки справа на всю высоту (object-fit:cover), слева заголовок и зелёная плашка с призывом.

## Тон

- Энергично, честно, без пафоса, канцелярита и интонации КП; не говорить о человеке в третьем лице на слайдах для него.
- «вы» или безличные формулировки; без «ребята» и «коллеги»; без длинных тире.
- Одна мысль на слайд, крупные цифры. Если просят сохранить текст — сохраняй формулировки, раскладывай на блоки.
- Не обещать за блогера то, что он делает сам (сценарии рилс, регистрация): предлагать текст и оформление страницы по его мыслям.
- Не выдумывать цифры; плейсхолдеры в [квадратных скобках].

## Факты Uppora

- «Uppora это новый формат контента, а не просто ссылка на перевод»
- «Я люблю этого блогера и хочу сделать с ним что-то крутое» — главное ощущение от страницы
- Разово, без подписки; лента поддержки с пожеланиями; QR для эфиров; договор дарения, без ИП
- Кейс: 400 000 ₽ за 10 дней; 306 000 ₽ от 592 человек по первому эфиру; средний донат 517 ₽; 12% зрителей (592 из 5 000)
