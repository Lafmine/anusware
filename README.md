# ANUSWARE

<p align="center">
  <img src="https://img.shields.io/badge/Статус-Release%201.0-c0392b?style=for-the-badge" alt="Release 1.0" />
  <img src="https://img.shields.io/badge/Release-1f1f1f?style=for-the-badge" alt="Release" />
  <img src="https://img.shields.io/badge/Язык-Lua-e67e22?style=for-the-badge" alt="Lua" />
  <img src="https://img.shields.io/badge/UI-Anusware%20Style-2c3e50?style=for-the-badge" alt="Anusware Style UI" />
</p>

<p align="center">
  Автономный Roblox Lua-скрипт с интерфейсом в стиле Anuswaremware, собранный в один release-файл.
</p>

<p align="center">
  <a href="./README.md">English Version</a>
</p>

## Описание

В этом репозитории хранится готовая к использованию обфусцированная release-сборка `anusware.lua`.

Читаемый исходник для разработки хранится отдельно и в этот репозиторий не входит. Репозиторий используется как чистая точка выдачи финального билда.

## Что В Репозитории

| Файл | Описание |
| --- | --- |
| `anusware.lua` | Обфусцированная release-сборка |

## Возможности

### Combat

- Aimbot с настраиваемым режимом активации
- Trigger Bot с минимальной задержкой
- Dynamic FOV и регулируемое сглаживание
- Выбор части тела с body fallback
- Wall check, лимит дистанции, team check и friend check
- Приоритеты: screen distance, world distance, lowest health
- Предикт по скорости с настраиваемым prediction time

### Anti-Aim

- Режимы yaw: `None`, `Static`, `Spin`, `Jitter`, `Sway`, `Random`
- Настройка base yaw, range, speed и random interval
- Режимы pitch, включая `Skeet Up` и `Down`

### Movement

- AirStrafe
- Auto Peek
- Infinite Jump
- Jump bypass
- WalkSpeed override
- Noclip
- Fly
- Quick Stop

### Visuals

- Упрощенный ESP
- Chams
- FOV circle
- Bullet tracers только по подтвержденному попаданию
- Hitmarker
- Custom crosshair
- Watermark и HUD активных функций
- Third person camera offset

### World

- Модуляция цвета мира
- Управление яркостью и временем
- Удаление тумана
- Поддержка custom skybox

### MM2

- Role ESP
- Gun ESP
- Coin ESP
- Auto gun pickup

### Sounds и QoL

- Trigger sound
- Hit sound
- Настройка громкости для обоих каналов
- Сохранение настроек в JSON при наличии filesystem API
- Безопасный `Unload` и восстановление состояний

## Стандартные Клавиши

| Действие | Клавиша |
| --- | --- |
| Меню | `Insert` |
| Aim | `MouseButton2` |
| Auto Peek | `X` |
| Third Person | `V` |

## Примечания По Запуску

- Все игровые функции по умолчанию выключены
- Доступность функций зависит от API, которые предоставляет текущий executor/runtime
- Если какая-то возможность не поддерживается средой, скрипт должен отключить только ее, а не ломаться целиком

## Конфигурация

Если доступны filesystem API, скрипт сохраняет настройки в версионированный JSON-конфиг и загружает их при следующем запуске.

Если конфиг поврежден, устарел или заполнен частично, он мигрируется либо заменяется безопасными значениями по умолчанию.

## Маркировка Релиза

Текущая внутренняя маркировка сборки:

```text
ANUSWARE | RELEASE 1.0
```

## Важно

Этот репозиторий предназначен для распространения release-сборки, а не открытого исходного кода без обфускации.

## Дисклеймер

Использование на ваш риск. Совместимость, поведение и стабильность зависят от конкретной игры и среды, в которой выполняется скрипт.
