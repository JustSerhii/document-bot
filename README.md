## Опис
Цей бот для Telegram використовує Google Document AI для аналізу документів. Він дозволяє користувачам завантажувати PDF або зображення, розпізнавати текст, генерувати короткий опис змісту.

## Функціональність
- **Розпізнавання тексту** в PDF та зображеннях за допомогою Document AI.
- **Генерація стислого резюме** документа.
- **Збереження результатів** у форматах: повідомлення, TXT, DOCX.

## Як працює
1. Надіслати у чат **фото** або **PDF**.
2. Бот обробить документ за допомогою Google Document AI.
3. Отримати результати у вигляді повідомлення, TXT або DOCX-файлу (на вибір).
4. За бажанням можна **узагальнити текст**.

## Налаштування
1. **Створити `.env` файл**:
   ```env
   BOT_TOKEN=your_telegram_bot_token
   PROJECT_ID=your_google_cloud_project_id
   LOCATION=your_processor_location
   PROCESSOR_ID=your_document_ai_processor_id
   SUMMARIZER_PROCESSOR_ID=your_summarizer_processor_id
   GOOGLE_CREDENTIALS=your_google_credentials.json
   ```

2. **Встановити залежності**:
   ```sh
   pip install -r requirements.txt
   ```

3. **Запусти бота**:
   ```sh
   python bot.py
   ```
   
## Бот у роботі
Користувач надсилає документ → Бот аналізує його через Google Document AI → Відправляє результат у зручному форматі.

Код можна розширювати, додаючи підтримку нових процесорів Google Document AI.
