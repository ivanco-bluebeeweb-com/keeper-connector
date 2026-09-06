# Keeper Security Connector — Connector Discovery

**Official Documentation:** https://keepersecurity.com  
**Base URL:** https://keepersecurity.com/api/rest  
**Auth Model:** Keeper Secrets Manager (KSM) Client Token  

## Основные сущности вендора
- записи хранилища (/vault/records), общие папки (/vault/shared_folders), роли, аудитные события

## Лимиты и особенности API
- Соблюдение Rate Limits вендора, обработка HTTP 429 с экспоненциальным backoff.
- Валидация входных данных по Pydantic-схемам вендора до отправки запроса.
- Тестовая точка проверки подключения: `POST /api/rest/vault/get_records`.
