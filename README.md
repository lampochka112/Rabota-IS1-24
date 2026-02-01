# 🚀 Репозиторий колледжных заданий 🎓
 
🧑‍🎓 **Студент:** Голосов Даниил Алексеевич  
📝 **Проверяющая:** Матишевская София Юрьевна   
📝 **Группа:** ИС1-24 
 
---

## 📂 Описание проекта
Этот репозиторий содержит выполненные задания и проекты, которые я изучаю в рамках колледжа. 🎯

---

## 📝 Задания и темы
- 💻 Основы программирования
- 🌐 Работа с системами контроля версий (Git)
- 🖥️ Операционные системы и командная строка
- 🌐 Основы сетевых технологий
- 🧩 Объектно-ориентированное программирование
- 🛠️ Разработка небольших проектов и практических заданий

---

## 📞 Контакты
| **Информация** | **Данные** |
|----------------|------------|
| Студент | Голосов Даниил Алексеевич |
| Группа | ИС1-24 |
| Проверяющая | Матишевская София Юрьевна |


# 🚀 Полный гайд по настройке VS Code для веб-разработки (HTML/CSS/JS)

Пошаговое руководство для начинающих по установке и настройке Visual Studio Code для комфортной работы с HTML, CSS и JavaScript.

## 📥 Часть 1: Установка VS Code

### Шаг 1: Скачивание
1. Перейдите на официальный сайт: [https://code.visualstudio.com/](https://code.visualstudio.com/)
2. Нажмите большую синюю кнопку **"Download for Windows"** (или для вашей ОС)
3. Дождитесь завершения загрузки

### Шаг 2: Установка (для Windows)
1. Запустите скачанный установщик (файл `.exe`)
2. Следуйте инструкциям мастера установки
3. **Важно:** Отметьте галочки:
   - ✅ "Add to PATH" (добавить в путь)
   - ✅ "Register as editor for supported file types"
   - ✅ "Add to context menu" (добавить в меню правой кнопки)
4. Нажмите "Install" и дождитесь завершения

## 🔧 Часть 2: Установка расширений (Extensions)

### Как установить расширение:
1. Откройте VS Code
2. На панели слева нажмите на иконку **"Extensions"** (или `Ctrl+Shift+X`)
   ![Иконка Extensions](dimg_7pp_aYSnBrr-p84PvfWRyQI_107)
3. В поисковой строке введите название расширения
4. Нажмите "Install" на нужном расширении

### 🎯 Обязательные расширения для старта:

| Расширение | Зачем нужно | Как найти |
|------------|-------------|-----------|
| **Live Server** by Ritwick Dey | Запускает сайт на локальном сервере с автообновлением | В поиске: `Live Server` |
| **Prettier - Code formatter** | Автоматически форматирует код | В поиске: `Prettier` |
| **Auto Rename Tag** | Автопереименование парных тегов | В поиске: `Auto Rename Tag` |
| **CSS Peek** | Показывает CSS-стили прямо в HTML | В поиске: `CSS Peek` |

### 📦 Дополнительные полезные расширения:
- **Material Icon Theme** - красивые иконки для файлов
- **Bracket Pair Colorizer 2** - цветные парные скобки
- **Path Intellisense** - подсказки путей к файлам
- **Error Lens** - ошибки прямо в коде

## ⚙️ Часть 3: Настройка параметров (Settings)

### Способ 1: Через графический интерфейс (рекомендуется новичкам)
1. Нажмите `Ctrl+,` (Windows/Linux) или `Cmd+,` (Mac)
2. Откроется окно настроек
3. В правом верхнем углу нажмите на иконку `{}`
   ![Open settings.json](https://i.imgur.com/W3axkQe.png)
4. Вставьте настройки из блока ниже

### Способ 2: Прямое редактирование файла
1. Нажмите `Ctrl+Shift+P` → введите "settings"
2. Выберите "Preferences: Open Settings (JSON)"
3. Вставьте настройки ниже

### 📝 Настройки для вставки:

```json
{
  // ========== РЕДАКТОР ==========
  "editor.fontSize": 14,
  "editor.wordWrap": "on",
  "editor.tabSize": 2,
  "editor.insertSpaces": true,
  "editor.minimap.enabled": false,
  
  // ========== ФОРМАТИРОВАНИЕ ==========
  "editor.formatOnSave": true,
  "editor.formatOnPaste": true,
  
  // Настройки Prettier
  "prettier.singleQuote": true,
  "prettier.semi": false,
  
  // Указываем Prettier как форматтер по умолчанию
  "[html]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[css]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  
  // ========== ФАЙЛЫ ==========
  "files.autoSave": "afterDelay",
  "files.autoSaveDelay": 1000,
  
  // ========== ЭММЕТ ==========
  "emmet.triggerExpansionOnTab": true,
  "emmet.includeLanguages": {
    "javascript": "html"
  },
  
  // ========== ТЕРМИНАЛ ==========
  "terminal.integrated.fontSize": 13,
  "terminal.integrated.defaultProfile.windows": "Command Prompt",
  
  // ========== ВНЕШНИЙ ВИД ==========
  "workbench.iconTheme": "material-icon-theme",
  "workbench.colorTheme": "Default Dark Modern"
}
