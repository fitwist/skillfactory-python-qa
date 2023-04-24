REST (Representational State Transfer) — популярный архитектурный стиль для создания веб-сервисов. RESTful API — это способ создания веб-сервисов, к которым можно получить доступ через Интернет, используя стандартные методы HTTP.

Преимущества:
- Простой и легкий
- Поддерживает несколько форматов данных, таких как XML, JSON и обычный текст.
- Кэширование: REST API может использовать кэширование, что повышает производительность.
- Независимый от платформы: REST API не зависит от платформы и доступен с любого устройства.
- Безопасный благодаря протоколу HTTPS.

Пример GET-запроса на Python, который предстоит "перегнать" в Postman:

```
import requests

headers = {"Content-Type": "application/json"}
payload = {"size": 10}

r = requests.get('https://jsonplaceholder.typicode.com/posts', json=payload)
print(r.text)
```
