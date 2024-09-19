# Шаг 7. Проверка качества
## Требования
- Установить расширение `Lighthouse` для браузера.
	- Добиться показателей >= 90 для Prefomance, Acessibility, Best Practices и SEO.
- Настроить и запустить `eslint` и `prettier` для проекта.
	- Необходимые зависимости: `eslint`, `prettier`, `eslint-config-prettier`.
	- Вынести запуск команд в npm scripts.
	- В приложении не должно быть ошибок и предупреждений.

Конфиг для `.eslintrc.json`:
```json
{  
    "env": {  
        "es2021": true  
    },  
    "extends": [  
        "eslint:recommended",
        "prettier"  
    ],  
    "parserOptions": {  
        "ecmaVersion": "latest",  
        "sourceType": "module"  
    }
}
```
Конфиг для `.prettierrc.json`:
```json
{  
  "trailingComma": "all",  
  "tabWidth": 2,  
  "semi": true,  
  "singleQuote": true,  
  "printWidth": 100  
}
```