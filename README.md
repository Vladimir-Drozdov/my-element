# My Element - Masonry Container Card

[![hacs_badge](https://img.shields.io/badge/HACS-Default-41BDF5.svg)](https://github.com/hacs/default)
![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)

Адаптивная карточка-контейнер для Home Assistant, которая располагает вложенные карточки в виде динамических masonry-колонок (как Pinterest). Карточка автоматически подстраивает количество колонок под ширину экрана.

## 📱 Демонстрация

<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/6f513411-6fce-4bfb-8383-de902993efec" />


## ✨ Возможности

- 📱 **Адаптивный дизайн** — автоматически меняет количество колонок (1/2/3) в зависимости от ширины экрана
- 🎨 **Визуальный редактор** — полная поддержка UI-редактора для настройки вложенных карточек
- 📦 **Drag & Drop** — удобное управление порядком карточек через интерфейс
- 🔧 **Поддержка любых карточек** — работает как со стандартными карточками HA, так и с пользовательскими (custom cards)
- 🖱️ **Стилизация** — каждая вложенная карточка имеет скруглённые углы 24px и единый стиль

## 📦 Установка

### Через HACS (рекомендуется)

1. Откройте HACS в вашем Home Assistant
2. Нажмите на три точки в правом верхнем углу и выберите "Custom repositories"
3. Добавьте репозиторий: `https://github.com/ВАШ_АККАУНТ/my-element` с типом "Lovelace"
4. Нажмите "ADD"
5. Найдите карточку "My Element" в HACS и установите её
6. Очистите кеш браузера (Ctrl+F5)

### Вручную

1. Скачайте файл `my-element.js` из [релизов](https://github.com/Vladimir-Drozdov/my-element/releases)
2. Поместите файл в папку `/config/www/` вашего Home Assistant
3. Добавьте ресурс в **Настройки → Панели → Ресурсы**:

```yaml
url: /local/my-element.js
type: JavaScript Module
