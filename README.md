# JobFinderBot

Локальный асинхронный Telegram-бот на базе Java (Spring Boot) и TDLib (it.tdlight), который мониторит входящие сообщения из профильных каналов, фильтрует их с помощью локального ИИ-агента (FreeQwenApi) под конкретный Java-стек и пересылает релевантные вакансии/заказы в целевой чат-приемник.

## Стек технологий
* Backend: Java 21, Spring Boot 3.5.7, Spring Data JPA

* Telegram Client: TDLib (it.tdlight-java)

* AI Integration: Spring AI (OpenAI-compatible starter)

* LLM Proxy: FreeQwenApi (модель qwen3.7-plus)

* Database: PostgreSQL

## Архитектура потока данных

<img width="759" height="432" alt="image" src="https://github.com/user-attachments/assets/0a8199b2-c124-408d-af58-423493faec99" />

**Важное замечание:** бот выполняет свой функционал, а именно сканирует все каналы пользователя с вакансиями, фриланс биржами и тд, и отправляет в одно место. Но это не весь задуманный функционал, и пока бот находится на стадии разработки.
