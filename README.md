# Student Material Design

**Приложение «Список студентов» с Material Design**

---

## Цель работы

Изучить принципы Material Design в Android-приложениях с использованием Jetpack Compose. Научиться создавать кастомные цветовые схемы, подключать пользовательские шрифты, настраивать формы компонентов и добавлять анимации.

---

## Функциональность приложения

- **Список студентов** — отображение 10 студентов с аватарками, именем и возрастом
- **Кастомная цветовая схема** — зеленая палитра для светлой и тёмной темы
- **Пользовательские шрифты** — Abril Fatface для заголовков, Montserrat для текста
- **Формы (Shapes)** — круглые аватарки, скошенные углы карточек
- **Поддержка тёмной темы** — автоматическое переключение по настройкам системы
- **Анимация раскрытия** — плавное появление описания студента при клике
- **Material Design 3 компоненты** — Card, Scaffold, TopAppBar, IconButton

---

## Технологии

- **Язык:** Kotlin
- **UI Toolkit:** Jetpack Compose
- **Дизайн-система:** Material Design 3
- **Шрифты:** Google Fonts (Abril Fatface, Montserrat)
- **Иконки:** Material Icons Extended
- **Система сборки:** Gradle (KTS)

---

## Структура проекта

```
app/
├── src/main/
│ ├── java/com.example.student_material_design/
│ │ ├── data/
│ │ │ ├── Student.kt
│ │ │ └── DataSource.kt
│ │ ├── ui/
│ │ │ ├── theme/
│ │ │ │ ├── Color.kt
│ │ │ │ ├── Theme.kt
│ │ │ │ ├── Type.kt
│ │ │ │ └── Shape.kt
│ │ │ └── MainActivity.kt
│ │ └── MainActivity.kt
│ ├── res/
│ │ ├── drawable/
│ │ │ ├── student1.jpg ... student10.jpg
│ │ │ └── ic_student_logo.png
│ │ ├── font/
│ │ │ ├── abril_fatface_regular.ttf
│ │ │ ├── montserrat_regular.ttf
│ │ │ └── montserrat_bold.ttf
│ │ ├── values/
│ │ │ ├── strings.xml
│ │ │ ├── colors.xml
│ │ │ └── dimens.xml
│ │ └── values-night/
│ └── img/ (скриншоты)
└── build.gradle.kts
```

---

## Реализованные элементы Material Design

### 1. Цвет (Color)
- Кастомная цветовая схема с основным зеленым цветом `#006C4C`
- Поддержка светлой и тёмной темы
- Автоматическая адаптация цветов для разных состояний

### 2. Типографика (Typography)
- **displayLarge** — Abril Fatface 36sp (заголовок приложения)
- **displayMedium** — Montserrat Bold 20sp (имена студентов)
- **bodyLarge** — Montserrat Regular 14sp (возраст, описание)
- **labelSmall** — Montserrat Bold 14sp (метка "О студенте")

### 3. Формы (Shape)
- **small** — круглое скругление 50dp (аватарки студентов)
- **medium** — диагональное скругление карточек (topEnd = 16dp, bottomStart = 16dp)

### 4. Компоненты
- **Card** — контейнер для каждого студента
- **Scaffold** — базовая структура экрана
- **TopAppBar** — верхняя панель с логотипом
- **IconButton** — кнопка раскрытия описания
- **LazyColumn** — эффективный список

### 5. Анимация
- **animateContentSize()** — плавное раскрытие карточки
- **Spring Animation** — физическая анимация с настраиваемыми параметрами

---

## Команды Git для публикации

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/yourusername/Student_Material_Design_FIO.git
git push -u origin main
```

---

## Автор
### ФИО: Грошев Никита Андреевич
### Группа: ИСП-232
### Дата: 11.03.2026
