# Keeper Security Connector — Auth & Credentials Standard

**Compliance:** AUTH_AND_CREDENTIALS_STANDARD.md (B1–B10)

## Схема аутентификации
- **Метод:** Keeper Secrets Manager (KSM) Client Token
- **Хранение:** Секреты сохраняются изолированно в хранилище секретов платформы Imperal.
- **Валидация:** При сохранении ключа выполняется тестовый запрос `POST /api/rest/vault/get_records`.
- **Отключение:** Удаление локальных ключей без воздействия на аккаунт вендора.
