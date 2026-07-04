# Suricata Study Labs

Учебный репозиторий с лабораторными стендами по Suricata и сетевой безопасности в контейнеризированной среде.

## Назначение

Проект показывает практику настройки и проверки IDS/IPS-подходов в локальных Docker Compose стендах. Репозиторий полезен как портфолио-проект для направлений Infrastructure Security, DevSecOps и Linux/containers.

## Что внутри

- `suricata-lab1/` - базовый Docker Compose стенд для запуска лабораторной среды.
- `suricata-lab2/` - отдельный Docker Compose стенд для следующего этапа практики.
- `suricata-lab3/` - расширенный стенд с `Dockerfile`, `docker-compose.yaml`, конфигурацией `smb.conf` и материалами лабораторной работы.

## Используемые технологии

- Suricata
- Docker
- Docker Compose
- Linux networking basics
- SMB/Samba lab configuration
- YAML configuration

## Практическая ценность

В рамках проекта отрабатываются:

- запуск security-инструментов в контейнерах;
- описание лабораторных окружений через Docker Compose;
- работа с сетевыми сервисами в изолированной среде;
- подготовка конфигураций для анализа сетевой активности;
- базовый troubleshooting контейнеров и сетевого взаимодействия.

## Быстрый старт

Пример запуска для третьей лабораторной работы:

```bash
cd suricata-lab3
docker compose up -d
```

Проверка состояния контейнеров:

```bash
docker compose ps
docker compose logs -f
```

Остановка стенда:

```bash
docker compose down
```

## Статус

Учебный проект. Перед использованием как production-конфигурации требуется ревизия настроек безопасности, сетевой модели и секретов.
