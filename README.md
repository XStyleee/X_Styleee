# CoinScan

CoinScan — это веб-приложение, похожее на CoinMarketCap, разработанное на Java с использованием Spring Boot и базы данных PostgreSQL.

## Основные технологии
- **Язык программирования**: Java
- **Фреймворк**: Spring Boot
- **База данных**: PostgreSQL
- **Сборщик проектов**: Maven
- **Среда разработки**: IntelliJ IDEA

## Функционал
- **Регистрация и авторизация пользователей**
- **Просмотр информации о криптовалютах**
- **Поиск криптовалют**
- **Управление портфелем** (добавление, удаление активов)
- **История транзакций**
- **Обсуждения в сообществе**

## Установка и запуск

### 1. Клонирование репозитория
```sh
git clone https://github.com/your-repository/coinscan.git
cd coinscan
```

### 2. Настройка базы данных PostgreSQL
1. Установите PostgreSQL и pgAdmin4
2. Создайте базу данных `coinscan`
3. Настройте `application.properties`:
```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/coinscan
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
```

### 3. Запуск приложения
```sh
mvn spring-boot:run
```

Приложение будет доступно по адресу: [http://localhost:8080](http://localhost:8080)

## API Эндпоинты
| Метод | URL | Описание |
|--------|----------------------|--------------------------------|
| `POST` | `/auth/register` | Регистрация нового пользователя |
| `POST` | `/auth/login` | Авторизация пользователя |
| `GET` | `/market` | Получение списка криптовалют |
| `GET` | `/portfolio` | Просмотр портфеля пользователя |
| `POST` | `/portfolio/add` | Добавление актива в портфель |
| `GET` | `/community` | Просмотр обсуждений |

## Контрибьюция
1. Форкните репозиторий
2. Создайте новую ветку (`git checkout -b feature-branch`)
3. Внесите изменения и закоммитьте (`git commit -m 'Добавлено: новая функция'`)
4. Запушьте изменения (`git push origin feature-branch`)
5. Откройте Pull Request

## GoogleDoc
https://docs.google.com/document/d/1BT9k7-wNWz9m-jd7rH9BkCqTRGnQiY675RgcYCimlV0/edit?tab=t.0
