# Eastrica Ultimate Windows Optimizer 🚀

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Windows](https://img.shields.io/badge/OS-Windows%2010%20%7C%2011-blue?logo=windows)](#)
[![PowerShell](https://img.shields.io/badge/Script-PowerShell-1f425f.svg?logo=powershell)](#)
[![Version](https://img.shields.io/badge/Version-1.0.0-success.svg)](#)

[🇷🇺 Русский](#ru-русский) | [🇬🇧 English](#en-english)

---

## [RU] Русский

**Eastrica Ultimate Windows Optimizer** — это ультимативный PowerShell-скрипт с интерактивным графическим интерфейсом (GUI) для глубокой, но безопасной настройки Windows 10 и 11. Создан специально для киберспортсменов, энтузиастов, геймеров и разработчиков в сфере ИИ, которым важна каждая миллисекунда и максимальная производительность железа.

### 📑 Оглавление
1. [Почему именно Eastrica?](#-почему-именно-eastrica)
2. [Что внутри (Ключевые функции)](#-что-внутри-ключевые-функции)
3. [Инструкция по установке и запуску](#-инструкция-по-установке-и-запуску)
4. [Безопасность и Удаление](#-безопасность-и-удаление)
5. [FAQ (Частые вопросы)](#-faq)

### 🏆 Почему именно Eastrica?
В отличие от многих «оптимизаторов», которые вслепую удаляют системные файлы и ломают Windows, этот скрипт работает прозрачно, имеет встроенную систему защиты и гибко адаптируется под вашу среду (например, определяет установленные античиты). Абсолютно весь код открыт.

### 🛠 Что внутри (Ключевые функции)

*   **Интерактивный GUI:** Удобный интерфейс с темной темой для выбора нужных опций без необходимости копаться в коде.
*   **Умная работа с Anti-Cheat:** Автоматическое обнаружение *Riot Vanguard, FACEIT AC, Easy Anti-Cheat, BattlEye*. Скрипт не отключает службы, критически важные для античитов, исключая риск бана или ошибок при запуске игр.
*   **Глубокая настройка ядра и DPC:** 
    *   Тонкая настройка таймеров ядра (Kernel Timers) и MMCSS (Multimedia Class Scheduler Service).
    *   Активация MSI Mode (Message Signaled Interrupts) для видеокарт, сетевых и USB-контроллеров для снижения инпут-лага.
    *   Включение/Отключение HAGS (Hardware-Accelerated GPU Scheduling) в зависимости от ваших нужд.
*   **Оптимизация CPU и Планировщика:** Правильная парковка ядер, адаптация Thread Director для процессоров с P-Cores и E-Cores (Intel 12th+ Gen), настройка квантов времени (Win32PrioritySeparation).
*   **Режим ИИ (AI Mode):** Подготовка ОС для работы с *PyTorch, Docker, WSL2 и Ollama*. Оптимизация выделения VRAM и предотвращение конфликтов с игровыми твиками.
*   **Отключение телеметрии:** Мягкое отключение сбора данных Microsoft без поломки Windows Update и Microsoft Store.
*   **Builder Mode:** Генерация файла `autounattend.xml` для создания собственного «чистого» образа Windows с заранее вшитыми настройками.

### 🚀 Инструкция по установке и запуску

1. Перейдите в раздел [Releases](../../releases) и скачайте последнюю версию `EastricaUltimateWindowsOptimizer.ps1`.
2. Кликните по скачанному файлу **правой кнопкой мыши** и выберите **«Выполнить с помощью PowerShell»** (Run with PowerShell).
3. При появлении запроса UAC нажмите «Да» (скрипту требуются права Администратора).

*Альтернативный запуск через консоль:*
Откройте PowerShell от имени Администратора и введите:
```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force
.\EastricaUltimateWindowsOptimizer.ps1
```

### 🛡 Безопасность и Удаление (Откат изменений)
Ваша безопасность — приоритет. При первом запуске скрипт автоматически:
1. Создает точку восстановления Windows.
2. Генерирует файл `Eastrica_Complete_Rollback.cmd` для экстренного восстановления.

**Как удалить оптимизатор и вернуть все как было?**
1. Запустите скрипт снова.
2. В правом верхнем углу GUI нажмите на **красный значок корзины (🗑)**.
3. Подтвердите действие. Скрипт восстановит реестр из бэкапа, удалит свои службы, задачи и полностью сотрет себя с ПК.

### ❓ FAQ
* **Сломает ли это мой Windows Update?** Нет, скрипт настроен так, чтобы телеметрия отключалась без влияния на базовые службы обновления ОС.
* **Подходит ли для ноутбуков?** Да. Скрипт умеет переключать схемы питания и автоматически отключает *Hardware Bus Sleep (ASPM/D3)* на мобильных CPU, чтобы избежать перегрева.

---
---

## [EN] English

**Eastrica Ultimate Windows Optimizer** is an ultimate PowerShell script with an interactive Graphical User Interface (GUI) for deep, yet safe optimization of Windows 10 and 11. Built specifically for eSports athletes, enthusiasts, gamers, and AI developers who care about every single millisecond and maximum hardware performance.

### 📑 Table of Contents
1. [Why choose Eastrica?](#-why-choose-eastrica)
2. [Under the Hood (Features)](#-under-the-hood-features)
3. [Installation & Usage](#-installation--usage)
4. [Safety & Uninstallation](#-safety--uninstallation)
5. [FAQ](#-faq-1)

### 🏆 Why choose Eastrica?
Unlike many "optimizers" that blindly delete system files and break Windows, this script is fully transparent, features a built-in safety net, and dynamically adapts to your environment (e.g., detecting installed anti-cheats). The code is 100% open-source.

### 🛠 Under the Hood (Features)

*   **Interactive GUI:** A user-friendly dark-themed menu to select tweaks without diving into the code.
*   **Smart Anti-Cheat Compatibility:** Automatically detects *Riot Vanguard, FACEIT AC, Easy Anti-Cheat, and BattlEye*. The script prevents disabling critical services required by these anti-cheats, ensuring zero ban risks or game crashes.
*   **Deep Kernel & DPC Tuning:** 
    *   Fine-tuning of Kernel Timers and MMCSS (Multimedia Class Scheduler Service).
    *   Enables MSI Mode (Message Signaled Interrupts) for GPUs, Network, and USB controllers for the lowest possible input lag.
    *   Configures HAGS (Hardware-Accelerated GPU Scheduling) based on your workload.
*   **CPU & Scheduler Optimization:** Proper core parking, Thread Director adaptation for hybrid architectures (P-Cores & E-Cores on Intel 12th+ Gen), and monolithic scheduler quantums (Win32PrioritySeparation).
*   **AI Mode:** Preps the OS for *PyTorch, Docker, WSL2, and Ollama*. Optimizes VRAM allocation and prevents conflicts with gaming tweaks.
*   **Telemetry Debloat:** Safely disables Microsoft data collection without breaking Windows Update or the Microsoft Store.
*   **Builder Mode:** Generates an `autounattend.xml` file to help you create your own debloated Windows ISO with baked-in tweaks.

### 🚀 Installation & Usage

1. Go to the [Releases](../../releases) page and download the latest `EastricaUltimateWindowsOptimizer.ps1`.
2. **Right-click** the downloaded file and select **"Run with PowerShell"**.
3. Click "Yes" on the UAC prompt (the script requires Administrator privileges).

*Alternative Console Method:*
Open PowerShell as Administrator and run:
```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force
.\EastricaUltimateWindowsOptimizer.ps1
```

### 🛡 Safety & Uninstallation (Rollback)
Your system's stability is our priority. On the first run, the script automatically:
1. Creates a Windows System Restore Point.
2. Generates an `Eastrica_Complete_Rollback.cmd` master script for emergency recovery.

**How to uninstall and revert all changes?**
1. Run the optimizer again.
2. Click the **red trash can icon (🗑)** in the top right corner of the GUI.
3. Confirm the action. The script will restore the registry from its backup, delete custom services/tasks, and completely remove itself from your PC.

### ❓ FAQ
* **Will this break Windows Update?** No. The script safely disables telemetry without affecting core OS update services.
* **Is it safe for laptops?** Yes. It includes smart power management and automatically disables *Hardware Bus Sleep (ASPM/D3)* on mobile CPUs to prevent thermal throttling.

---
### 📄 License / Лицензия
This project is licensed under the **[MIT License](LICENSE)**. 
*Use at your own risk. The author is not responsible for any system damage.*

Этот проект распространяется под лицензией **MIT License**. 
*Используйте на свой страх и риск. Автор не несет ответственности за возможные неполадки в работе ОС.*