# Image Archive

Публичный репозиторий для хранения изображений, используемых в проектах.

## Как формировать ссылку на изображение

Для использования изображения напрямую на сайте необходимо использовать адрес:

```text
https://raw.githubusercontent.com/MegaRostBLR1/Image_Archive/main/ПУТЬ_К_ФАЙЛУ
```

### Пример

Если изображение находится здесь:

```text
LightStudio/hero-img.webp
```

прямая ссылка будет:

```text
https://raw.githubusercontent.com/MegaRostBLR1/Image_Archive/main/LightStudio/hero-img.webp
```

Если изображение находится в папке товара:

```text
LightStudio/babylon/image.webp
```

ссылка:

```text
https://raw.githubusercontent.com/MegaRostBLR1/Image_Archive/main/LightStudio/babylon/image.webp
```

## Использование в HTML

```html
<img
    src="https://raw.githubusercontent.com/MegaRostBLR1/Image_Archive/main/LightStudio/hero-img.webp"
    alt="Описание изображения"
>
```

## Использование в Google Sheets

В таблице каталога можно хранить прямые ссылки на изображения.

**Поле `img`:**

```text
https://raw.githubusercontent.com/MegaRostBLR1/Image_Archive/main/LightStudio/babylon/image.webp
```

**Поле `gallery`:**

Несколько изображений указываются через символ `|`:

```text
https://raw.githubusercontent.com/MegaRostBLR1/Image_Archive/main/LightStudio/babylon/image-1.webp|https://raw.githubusercontent.com/MegaRostBLR1/Image_Archive/main/LightStudio/babylon/image-2.webp|https://raw.githubusercontent.com/MegaRostBLR1/Image_Archive/main/LightStudio/babylon/image-3.webp
```

## Важно

- Используйте `raw.githubusercontent.com`, а не URL страницы файла на GitHub.
- Репозиторий должен оставаться публичным, если изображения должны загружаться без авторизации.
- При переносе файла в другую папку путь в прямой ссылке необходимо изменить.
- Имена файлов и папок должны точно совпадать с путём в репозитории.
- Для изображений в проектах предпочтительно использовать формат WebP.

## Структура

Например:

```text
Image_Archive/
└── LightStudio/
    ├── babylon/
    │   ├── image-1.webp
    │   └── image-2.webp
    ├── bastion/
    ├── cascade/
    ├── ...
    ├── certificate.webp
    └── hero-img.webp
```

Формула ссылки:

```text
https://raw.githubusercontent.com/MegaRostBLR1/Image_Archive/main/ + путь к файлу
```
