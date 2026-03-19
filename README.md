# projects in the field of RAG and voice interfaces
Pet-проекты
1. Нейро-консультант по техническому регламенту ТР ТС 001/2011
(RAG-система на базе LangChain, FAISS, VseGPT)
Разработала приложение для ответов на вопросы по техническому регламенту безопасности железнодорожного состава.
Реализовала загрузку документа из Google Docs, разбиение на чанки, создание эмбеддингов (text-embedding-3-small) и индексацию в FAISS.
Внедрила пороговый фильтр релевантности для повышения качества ответов.
Использовала API VseGPT (совместимое с OpenAI) для генерации ответов.
Стек: Python, LangChain, FAISS, OpenAIEmbeddings, VseGPT API.

2. Нейро-консультант по экологической экспертизе (GigaChat + HuggingFace)
Аналогичная RAG-система, но с использованием GigaChat и локальных эмбеддингов через HuggingFace (paraphrase-multilingual-mpnet-base-v2).
Настроила взаимодействие с GigaChat API, обработал особенности авторизации.
Провёла тестирование на наборе вопросов, обеспечил корректную обработку запросов вне темы.
Стек: Python, LangChain, FAISS, HuggingFaceEmbeddings, GigaChat API.

3. Голосовой переводчик Русский → Английский
Создала приложение для голосового перевода с использованием Salute Speech (STT/TTS) и GigaChat (перевод).
Реализовала полный цикл: распознавание речи (ru) → перевод текста (en) → синтез речи.
Интегрировала авторизацию и работу с API SberDevices.
Стек: Python, requests, Salute Speech API, GigaChat API, pydub.
