# 🚀 Оптимизация VS Code для веб-разработки (HTML/CSS/JS)  

Краткий гайд по настройке Visual Studio Code для комфортной и продуктивной работы с HTML, CSS и JavaScript.
 
## 📦 Рекомендуемые расширения (Extensions) 

### Обязательные 
*   **Live Server** (Ritwick Dey) - Запускает локальный сервер с горячей перезагрузкой.
*   **Prettier - Code formatter** - Автоматическое форматирование кода по единому стандарту.
*   **Auto Rename Tag** - Автоматически переименовывает парный HTML/XML тег. 
*   **CSS Peek** - Позволяет "заглянуть" в CSS правила из HTML и наоборот.
*   **IntelliSense for CSS class names in HTML** - Автодополнение классов CSS в HTML. 

### Для улучшения работы
*   **ES7+ React/Redux/... Snippets** (dsznajder) - Сниппеты для JS, React (полезно даже без React).
*   **JavaScript (ES6) code snippets** - Полезные сниппеты для нативного JS.
*   **Bracket Pair Colorizer 2** (или встроенная функция) - Разноцветные скобки для лучшей читаемости.
*   **Path Intellisense** - Автодополнение путей к файлам.
*   **Error Lens** - Показывает ошибки и предупреждения прямо в строке кода.
*   **Material Icon Theme** - Красивые иконки для файлов в дереве проекта.

## ⚙️ Настройки (`settings.json`)

Добавьте эти настройки в файл `File -> Preferences -> Settings` (в правом верхнем углу нажмите на иконку `{}`):

```json
{
  // Редактор
  "editor.formatOnSave": true,
  "editor.wordWrap": "on",
  "editor.minimap.enabled": false, // Убрать мини-карту для экономии места
  "editor.tabSize": 2,
  "editor.insertSpaces": true,
  
  // Форматирование
  "prettier.singleQuote": true,
  "prettier.semi": false,
  "[html]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[css]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },

  // Файлы и исключения
  "files.autoSave": "onFocusChange",
  "files.exclude": {
    "**/.git": true,
    "**/.DS_Store": true,
    "**/node_modules": true
  },

  // Эммет для ускорения вёрстки
  "emmet.includeLanguages": {
    "javascript": "html"
  },
  "emmet.triggerExpansionOnTab": true
}
