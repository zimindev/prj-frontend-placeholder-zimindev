# Placeholder | Zimin.Dev

Сторінка-заглушка з лого Zimin.Dev для субдоменів, на яких згодом з'являються презентації проєктів для клієнтів (site1–site9.zimin.dev). Статичний HTML без залежностей і без запитів до сторонніх сервісів.

![Desktop](screenshots/desktop.png)

<p><img src="screenshots/mobile.png" width="300" alt="Mobile"> <img src="screenshots/desktop-uk.png" width="520" alt="Українською"></p>

- Темний дизайн у кольорах zimin.dev (#111111, #7d3ed0), лого з легкою анімацією, кнопка **zimin.dev**.
- У плашці під лого автоматично показується адреса, на якій відкрита сторінка (`site3.zimin.dev` тощо), тому один файл підходить для всіх субдоменів.
- Текст англійською. За мовою браузера він сам перемикається на українську, німецьку, польську, французьку чи російську.
- Шрифти Manrope і Plus Jakarta Sans лежать разом зі сторінкою.
- Сторінку закрито від індексації: `robots.txt`, `<meta name="robots">`, заголовок `X-Robots-Tag` у `.htaccess`.
- `.htaccess` має `RewriteEngine On`, щоб правила WordPress із батьківської теки (`/home/<user>/.htaccess`) не успадковувались і не давали помилку 500. Також вимикає перелік файлів і задає `index.html`.

## Встановлення

Скопіюйте `index.html`, `robots.txt`, `.htaccess` і теку `assets/` у корінь сайту (або розпакуйте zip із Release).

```sh
scp -r index.html robots.txt .htaccess assets user@server:/home/user/subdomains/site1.example.com/
```

## Версії

- **1.0.1** — на кнопці текст «zimin.dev» (усіма мовами), підпис у футері прибрано.
- **1.0.0** — перша версія.

---

Sasha Zimin · [zimin.dev](https://zimin.dev)
