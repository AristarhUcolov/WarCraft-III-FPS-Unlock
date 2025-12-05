# WarCraft III FPS Unlock

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> Unlock the full potential of WarCraft III by removing the 30 FPS frame limiter

---

## 📖 Table of Contents

- [🇷🇺 Русская версия](#-русская-версия)
- [🇬🇧 English Version](#-english-version)

---

## 🇷🇺 Русская версия

### 📋 Описание

Простой RegFile, который отключает V-Sync (а точнее ограничитель кадров в 30 FPS) для WarCraft III. После применения вы получите максимальную производительность и плавность игры.

### ✨ Особенности

- 🚀 Снимает ограничение в 30 FPS
- ⚡ Повышает плавность игры
- 🎮 Улучшает отзывчивость управления
- 🔧 Простая установка через реестр Windows

### 💾 Требования

- Windows (любая версия)
- WarCraft III (любая версия: Reign of Chaos, The Frozen Throne, Reforged)

### 📦 Установка

1. Скачайте файл `WarCraft III.reg` из репозитория
2. Дважды щелкните на файле, чтобы запустить его
3. Подтвердите внесение изменений в реестр Windows
4. Запустите WarCraft III и наслаждайтесь!

### ⚙️ Как это работает

Файл реестра изменяет параметр `lockfb` в настройках видео WarCraft III:

```registry
[HKEY_CURRENT_USER\Software\Blizzard Entertainment\Warcraft III\Video]
"lockfb"=dword:00000000
```

Установка значения `lockfb` в `0` отключает принудительное ограничение частоты кадров, позволяя игре работать с максимальной частотой кадров, которую поддерживает ваше оборудование.

### ⚠️ Важно

- Убедитесь, что WarCraft III закрыт перед применением изменений
- Для отмены изменений установите значение `lockfb` обратно в `1`

### 🔄 Откат изменений

Чтобы вернуть ограничение в 30 FPS, создайте файл с расширением `.reg` и следующим содержимым:

```registry
Windows Registry Editor Version 5.00

[HKEY_CURRENT_USER\Software\Blizzard Entertainment\Warcraft III\Video]
"lockfb"=dword:00000001
```

![image](https://github.com/user-attachments/assets/9ce0b912-71c1-4ca8-a628-33e44670f848)

---

## 🇬🇧 English Version

### 📋 Description

A simple RegFile that disables V-Sync (or rather the 30 FPS frame limiter) for WarCraft III. After applying, you will experience maximum performance and smooth gameplay.

### ✨ Features

- 🚀 Removes the 30 FPS limitation
- ⚡ Increases game smoothness
- 🎮 Improves control responsiveness
- 🔧 Easy installation via Windows Registry

### 💾 Requirements

- Windows (any version)
- WarCraft III (any version: Reign of Chaos, The Frozen Throne, Reforged)

### 📦 Installation

1. Download the `WarCraft III.reg` file from the repository
2. Double-click the file to run it
3. Confirm the changes to the Windows Registry
4. Launch WarCraft III and enjoy!

### ⚙️ How It Works

The registry file modifies the `lockfb` parameter in WarCraft III's video settings:

```registry
[HKEY_CURRENT_USER\Software\Blizzard Entertainment\Warcraft III\Video]
"lockfb"=dword:00000000
```

Setting `lockfb` to `0` disables the forced frame rate limiter, allowing the game to run at the maximum frame rate your hardware can support.

### ⚠️ Important

- Make sure WarCraft III is closed before applying the changes
- To revert the changes, set `lockfb` back to `1`

### 🔄 Reverting Changes

To restore the 30 FPS limitation, create a file with `.reg` extension and the following content:

```registry
Windows Registry Editor Version 5.00

[HKEY_CURRENT_USER\Software\Blizzard Entertainment\Warcraft III\Video]
"lockfb"=dword:00000001
```

![image](https://github.com/user-attachments/assets/f547557d-a86a-4a58-a768-801d6758b2af)

---

## 👤 Author

**Aristarh Ucolov (Аристарх Уколов)**

## 📄 License

This project is open source and available under the MIT License.

---

⭐ If this helped you enjoy WarCraft III at higher frame rates, please consider giving this repository a star!
