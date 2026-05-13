# tvOS Sideload Apps

Коллекция IPA-файлов для установки на Apple TV (tvOS) через сайдлоад.

## Приложения

| Приложение | Скачать | Размер | Описание |
|---|---|---|---|
| 🎮 CloudNow | [CloudNow.ipa](https://github.com/akorshun/tvos-sideload-apps/raw/master/CloudNow.ipa) | 6.7 MB | Неофициальный клиент [GeForce NOW](https://www.nvidia.com/en-us/geforce-now/) для tvOS — стриминг игр с облачных серверов NVIDIA прямо на Apple TV |
| 🎬 Infuse Pro 8 | [InfusePro8.ipa](https://github.com/akorshun/tvos-sideload-apps/raw/master/InfusePro8_tvOS_sideload_patched.ipa) | 112 MB | [Infuse Pro 8](https://firecore.com/infuse) — мощный медиаплеер с поддержкой MKV, Dolby Vision, HDR и сетевых хранилищ. Файл патчен для установки через сайдлоад без подписки. ⚠️ После установки обязательно отключи синхронизацию iCloud в настройках приложения |
| 📺 MuTube | [mutube_4.54.01.ipa](https://github.com/akorshun/tvos-sideload-apps/raw/master/mutube_4.54.01.ipa) | 41 MB | YouTube-клиент v4.54.01 для tvOS, основанный на [TizenTube](https://github.com/reisxd/TizenTube) — оптимизированная альтернатива официальному приложению с поддержкой 4K, SponsorBlock и без рекламы |
| 🌐 tvOS Browser | [tvOSBrowser.ipa](https://github.com/akorshun/tvos-sideload-apps/raw/master/tvOSBrowser.ipa) | 205 KB | Веб-браузер для tvOS |

## Как установить

### ATVLoadly (рекомендуется для Apple TV)

[ATVLoadly](https://github.com/bitxeno/atvloadly) — самохостящийся Docker-контейнер с веб-интерфейсом для сайдлоада напрямую на Apple TV без компьютера рядом.

1. Подними контейнер на любом сервере или домашнем NAS:
   ```bash
   docker run -d -p 8080:8080 ghcr.io/atvloadly/atvloadly:latest
   ```
2. На Apple TV открой браузер и перейди на адрес твоего сервера
3. Загрузи `.ipa` и следуй инструкциям на экране

> Требуется Apple TV с tvOS 16+ и учётная запись разработчика (бесплатная)

### Sideloadly (через компьютер)

[Sideloadly](https://sideloadly.io/) — установка с компьютера через USB или Wi-Fi.

1. Скачай и установи [Sideloadly](https://sideloadly.io/)
2. Подключи Apple TV к той же сети Wi-Fi, что и компьютер
3. Перетащи `.ipa` файл в окно Sideloadly
4. Введи Apple ID и нажми **Start**

### AltStore

[AltStore](https://altstore.io/) — альтернативный магазин приложений через AltServer на компьютере.

1. Установи [AltServer](https://altstore.io/) на компьютер
2. Подключи Apple TV по сети
3. Установи AltStore на Apple TV через AltServer
4. Открой AltStore → **My Apps** → **+** → выбери `.ipa`

## Примечания

- Бесплатный Apple ID позволяет устанавливать до **3 приложений** одновременно, сертификат действует **7 дней**
- С платным аккаунтом разработчика ($99/год) — до **10 приложений**, сертификат **1 год**
- Большие файлы (Infuse, MuTube) хранятся через [Git LFS](https://git-lfs.com/)
