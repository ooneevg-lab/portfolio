# Сурнов Евгений — портфолио Python-разработчика

Backend: Django / DRF / Flask · ML: PyTorch / fastai · Desktop: Electron / pywebview
Продакшн-опыт: развёртывание и сопровождение систем на VPS (nginx + systemd + PostgreSQL + Redis)

## Проекты

### 1. [Clinic Queue](https://github.com/ooneevg-lab/clinic-queue) — электронная очередь клиники (продакшн)
Django + DRF + Channels (Redis) + PostgreSQL. Регистратура, кабинеты врачей, табло, TTS-озвучка (конкатенация wav-кусков + Silero), WebSocket, аудит, печать талонов с QR. Мультифилиальность, интеграционные и стресс-тесты. Развёрнута на VPS (nginx, systemd, daphne), живая эксплуатация.
**Стек:** Python, Django, DRF, Django Channels, Redis, Daphne, PostgreSQL, Electron, Silero TTS.

### 2. [ECG Analysis](https://github.com/ooneevg-lab/ecg-analysis) — настольное приложение анализа ЭКГ (ВКР)
Настольное приложение-«watcher» для автоматизации анализа ЭКГ: отслеживает папку с XML-выгрузками электрокардиографа, прогоняет сигнал через нейросети DenseNet121 (PyTorch + fastai, отдельный классификатор ритма), оболочка pywebview, PDF-отчёты (ReportLab), сборка в exe (PyInstaller).
**Стек:** Python, Flask, PyTorch, fastai, Plotly, pywebview, PyInstaller.

### 3. [Clinic Schedule](https://github.com/ooneevg-lab/clinic-schedule) — расписание врачей с push-уведомлениями
Django + Celery + Redis: загрузка Excel-графика и его парсинг в структуру, REST API с токенами, push через Firebase Cloud Messaging, Android-клиент (Kotlin, WebView + FCM-сервис).
**Стек:** Python, Django, DRF, Celery, Redis, firebase-admin, Kotlin.

## Документы

- 📄 **ВКР** — выпускная квалификационная работа Сурнова Е. С. — [docs/ВКР_СУРНОВ_Е_С.pdf](docs/ВКР_СУРНОВ_Е_С.pdf)
- 📄 **Презентация к ВКР** (анализ ЭКГ с тематическими плашками) — [docs/prezentaciya_analiz_ekg.pdf](docs/prezentaciya_analiz_ekg.pdf)

## Прочее

- Мои репозитории: [github.com/ooneevg-lab](https://github.com/ooneevg-lab?tab=repositories)
- README каждого проекта содержит описание, инструкции запуска и состав.
