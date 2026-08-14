# The Pointer-Based Security Paradigm

---

**Архитектурный сдвиг от защиты данных к их несуществованию**

Фундаментальное переосмысление архитектуры цифровой безопасности, которое устраняет уязвимое существование данных вместо их защиты с помощью обычных механизмов шифрования и контроля доступа.

---

## Аннотация

В данной работе представлена Pointer-Based Security Paradigm, которая трансформирует цифровую безопасность от защиты данных при передаче и хранении к созданию систем, в которых конфиденциальные данные никогда не существуют как уязвимая сущность. Парадигма характеризуется тремя ключевыми трансформациями: (1) от передачи данных к синхронному обнаружению на основе указателей, (2) от хранения секретов к детерминированной регенерации и (3) от защиты поверхности атак к архитектурному устранению. Мы демонстрируем этот сдвиг на практических реализациях, включая системы обмена сообщениями, обменивающиеся только открытыми указателями, и системы аутентификации, не требующие хранения учетных данных. Данный подход обеспечивает неотъемлемую устойчивость к анализу метаданных, устранение баз данных учетных данных и математическую опровержимость за счет архитектурного проектирования, а не криптографической новизны.

> *Опубликовано: 26 сентября 2025 года*  
> *Статус: Теоретическое исследование*

---

[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.17204738-blue)](https://doi.org/10.5281/zenodo.17204738)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Research Paper](https://img.shields.io/badge/📄_Research_Paper-Zenodo-success)](https://zenodo.org/records/17204738)
[![Unique Views](https://img.shields.io/badge/dynamic/json?url=https://zenodo.org/api/records/17204738&query=$.stats.unique_views&label=👁️_Unique_Views&color=blue&logo=zenodo)](https://doi.org/10.5281/zenodo.17204738)
[![Unique Downloads](https://img.shields.io/badge/dynamic/json?url=https://zenodo.org/api/records/17204738&query=$.stats.unique_downloads&label=📥_Unique_Downloads&color=green&logo=zenodo)](https://doi.org/10.5281/zenodo.17204738)
[![Total Views](https://img.shields.io/badge/dynamic/json?url=https://zenodo.org/api/records/17204738&query=$.stats.views&label=👀_Total_Views&color=blue&logo=zenodo)](https://doi.org/10.5281/zenodo.17204738)
[![Total Downloads](https://img.shields.io/badge/dynamic/json?url=https://zenodo.org/api/records/17204738&query=$.stats.downloads&label=💾_Total_Downloads&color=green&logo=zenodo)](https://doi.org/10.5281/zenodo.17204738)
[![Paradigm Research](https://img.shields.io/badge/🔬_Paradigm_Research-Theoretical-orange)](https://github.com/smartlegionlab/pointer-based-security-paradigm)
[![Published](https://img.shields.io/badge/📅_Published-September_26,_2025-brightgreen)](https://doi.org/10.5281/zenodo.17204738)

---

## ⚠️ Правовое уведомление и статус исследования

**АКАДЕМИЧЕСКОЕ ИССЛЕДОВАНИЕ - НЕ ДЛЯ ПРАКТИЧЕСКОГО ИСПОЛЬЗОВАНИЯ**

**Это теоретическое исследование, а не производственное программное обеспечение.**

> **Предупреждение:** Данная работа предназначена только для академического обсуждения. Не используйте в производственных системах.

**Полное академическое уведомление:** См. [DISCLAIMER.md](DISCLAIMER.md)

---

## Детали публикации

| Деталь                      | Информация                                                         |
|-----------------------------|--------------------------------------------------------------------|
| **Название**                | The Pointer-Based Security Paradigm                                |
| **DOI**                     | [10.5281/zenodo.17204738](https://doi.org/10.5281/zenodo.17204738) |
| **Опубликовано**            | 26 сентября 2025 года                                              |
| **Лицензия**                | Creative Commons Attribution 4.0 International                     |
| **Автор**                   | Александр Суворов                                                  |
| **ORCID**                   | [0009-0006-3427-9611](https://orcid.org/0009-0006-3427-9611)       |
| **Тип**                     | Теоретическое исследование                                         |

## Загрузка и доступ

| Формат                     | Ссылка                                                                                                                                                          |
|----------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 📄 **Загрузка PDF**        | [Скачать с Zenodo](https://zenodo.org/records/17204738/files/suvorov-the-pointer-based-security-paradigm-v2.pdf?download=1)                                     |
| 📖 **Читать онлайн**       | [Запись Zenodo](https://doi.org/10.5281/zenodo.17204738)                                                                                                        |
| 💻 **Исходный код**        | [Репозиторий GitHub](https://github.com/smartlegionlab/pointer-based-security-paradigm)                                                                         |
| 📰 **Статья**              | [dev.to Технический разбор](https://dev.to/smartlegionlab/the-pointer-based-security-paradigm-a-practical-shift-from-data-protection-to-data-non-existence-h82) |

## Информация об авторе

| Контакт     | Информация                                                     |
|-------------|----------------------------------------------------------------|
| **Имя**     | Александр Суворов                                              |
| **Сайт**    | [smartlegionlab.ru](https://smartlegionlab.ru)                 |
| **GitHub**  | [smartlegionlab](https://github.com/smartlegionlab)            |
| **Email**   | smartlegionlab@gmail.com                                       |
| **ORCID**   | [0009-0006-3427-9611](https://orcid.org/0009-0006-3427-9611)   |

---

## Ключевые трансформации

| От                          | К                               |
|-----------------------------|---------------------------------|
| Передача данных             | Синхронное обнаружение          |
| Хранение секретов           | Детерминированная регенерация   |
| Защита поверхности атак     | Архитектурное устранение        |

### Детальные трансформации

1. **От передачи данных к синхронному обнаружению**  
   Информация возникает через координацию на основе указателей, а не передается и не хранится

2. **От хранения секретов к детерминированной регенерации**  
   Аутентификация через доказательство знания, а не через хранимые учетные данные

3. **От защиты поверхности атак к архитектурному устранению**  
   Безопасность через удаление уязвимого существования данных

---

## Связанные исследования

### Local Data Regeneration Paradigm  
**Онтологическая основа для синхронного обнаружения**

- **Статья:** [Zenodo](https://doi.org/10.5281/zenodo.17264327)
- **Код:** [Репозиторий GitHub](https://github.com/smartlegionlab/local-data-regeneration-paradigm)

### Position-Candidate-Hypothesis (PCH) Paradigm 
**Position-Candidate-Hypothesis (PCH) — это теоретическая парадигма для структурно-статистического анализа NP-полных задач.**

- **Статья:** [Zenodo](https://doi.org/10.5281/zenodo.17614888)
- **Код:** [Репозиторий GitHub](https://github.com/smartlegionlab/position-candidate-hypothesis-paradigm)

### Deterministic Game Engine  
**Практическая реализация и экспериментальная валидация**

- **Статья:** [Zenodo](https://doi.org/10.5281/zenodo.17383447)
- **Код:** [Репозиторий GitHub](https://github.com/smartlegionlab/deterministic-game-engine-report)

---

## Практическая реализация

Pointer-Based Security Paradigm реализована в экосистеме **Smart Password Ecosystem**:

| Компонент                                                                                   | Описание                     | Кроссплатформенность |
|---------------------------------------------------------------------------------------------|------------------------------|----------------------|
| [smartpasslib](https://github.com/smartlegionlab/smartpasslib)                              | Основная библиотека Python   | Python               |
| [smartpasslib-js](https://github.com/smartlegionlab/smartpasslib-js)                        | Реализация JavaScript        | JS                   |
| [smartpasslib-kotlin](https://github.com/smartlegionlab/smartpasslib-kotlin)                | Реализация Kotlin            | Kotlin               |
| [smartpasslib-go](https://github.com/smartlegionlab/smartpasslib-go)                        | Реализация Go                | Go                   |
| [smartpasslib-csharp](https://github.com/smartlegionlab/smartpasslib-csharp)                | Реализация C#                | C#                   |
| [Desktop Manager](https://github.com/smartlegionlab/smart-password-manager-desktop)         | Десктопное приложение        | Linux                |
| [Desktop Manager (C#)](https://github.com/smartlegionlab/SmartPasswordManagerCsharpDesktop) | Десктопное приложение        | Windows              |
| [CLI PassMan](https://github.com/smartlegionlab/clipassman)                                 | Консольный менеджер паролей  | Кроссплатформенный   |
| [CLI PassGen](https://github.com/smartlegionlab/clipassgen)                                 | Консольный генератор паролей | Кроссплатформенный   |
| [Web Manager](https://github.com/smartlegionlab/smart-password-manager-web)                 | Веб-интерфейс                | Любой браузер        |
| [Android Manager](https://github.com/smartlegionlab/smart-password-manager-android)         | Мобильное приложение         | Android              |

---

## Кроссплатформенная совместимость

Практическая реализация парадигмы генерирует **идентичные пароли** на всех платформах:

| Платформа  | Реализация                                                                                                                   |
|------------|------------------------------------------------------------------------------------------------------------------------------|
| Python     | [smartpasslib](https://github.com/smartlegionlab/smartpasslib)                                                               |
| JavaScript | [smartpasslib-js](https://github.com/smartlegionlab/smartpasslib-js)                                                         |
| Kotlin     | [smartpasslib-kotlin](https://github.com/smartlegionlab/smartpasslib-kotlin)                                                 |
| Go         | [smartpasslib-go](https://github.com/smartlegionlab/smartpasslib-go)                                                         |
| C#         | [smartpasslib-csharp](https://github.com/smartlegionlab/smartpasslib-csharp)                                                 |
| Web        | [Web Manager](https://github.com/smartlegionlab/smart-password-manager-web)                                                  |
| Android    | [Android Manager](https://github.com/smartlegionlab/smart-password-manager-android)                                          |
| Десктоп    | [Desktop Manager](https://github.com/smartlegionlab/smart-password-manager-desktop)                                          |
| CLI        | [CLI PassMan](https://github.com/smartlegionlab/clipassman) / [CLI PassGen](https://github.com/smartlegionlab/clipassgen)    |

---

## Цитирование

```bibtex
@misc{suvorov_2025_17204738,
  author       = {Suvorov, Alexander},
  title        = {The Pointer-Based Security Paradigm: Architectural
                   Shift from Data Protection to Data Non-Existence
                  },
  month        = sep,
  year         = 2025,
  publisher    = {Zenodo},
  doi          = {10.5281/zenodo.17204738},
  url          = {https://doi.org/10.5281/zenodo.17204738},
}
```

---

## Лицензия

Данное исследование и все сопроводительные документы лицензированы в соответствии с
[Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/).

## Авторские права

Copyright © 2025 Александр Суворов. Лицензировано в соответствии с Creative Commons Attribution 4.0 International.
