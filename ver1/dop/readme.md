### replace (mermaid)
- modifiedContent = content.replace(regexQuotes, '');      // шаг 1: удаляем кавычки
- modifiedContent = modifiedContent.replace(regexBrackets, '_'); // шаг 2: заменяем скобки
### symbol
- Кавычки (", «, », „, ‟) — удалены.
- Скобки ((), [], {}, <>) — заменены на _.
