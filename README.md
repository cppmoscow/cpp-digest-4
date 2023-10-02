# cpp-digest-4

Название: C++ Дайджест №4 (18 сентября – 1 октября 2023)

## Аннотация

Привет, Хабр! Сегодня я хочу вам представить подборку интересных новостей и материалов из мира C++ за последние две недели.

Приятного чтения!

## ⚡️️ Новости и релизы

1. [LLVM 17.0.1](https://github.com/llvm/llvm-project/releases/tag/llvmorg-17.0.1) — Новый мажорный релиз, принесший множество изменений во все проекты LLVM: полная поддержка [корутин](https://en.cppreference.com/w/cpp/language/coroutines), начало работы над реализацией [нововведений C++26](https://en.cppreference.com/w/cpp/compiler_support/26) и другое.
2. [Qt 6.5.3](https://www.qt.io/blog/qt-6.5.3-released) — Багфиксы и исправление уязвимостей.
3. [Conan 2.0.11](https://github.com/conan-io/conan/releases/tag/2.0.11), [2.0.12](https://github.com/conan-io/conan/releases/tag/2.0.12), [2.0.13](https://github.com/conan-io/conan/releases/tag/2.0.13) — Добавление поддержки clang-17, улучшение поддержки clang-cl и другое.
4. [cppfront: Autumn update](https://herbsutter.com/2023/09/28/cppfront-autumn-update/) — Очередные новости с полей разработки [cppfront](https://github.com/hsutter/cppfront): теперь он написан на самом себе; поддерживает `requires` и еще три стандартные «метафункции» (см. [P0707R4](https://www.open-std.org/jtc1/sc22/wg21/docs/papers/2019/p0707r4.pdf)): безопасные альтернативы `enum` и `union`.
5. 🇷🇺 Habr: [userver 1.0 — релиз фреймворка для IO-bound программ](https://habr.com/ru/companies/yandex/articles/760244/) — Первый мажорный релиз, привнесший целую кучу нововведений: WebSockets и TLS/HTTPS сервер, драйвер MySQL и RabbitMQ и многое другое.

## 📝 Статьи

1. 🇷🇺 Habr: [Основы C++: Указатели и Итераторы](https://habr.com/ru/companies/otus/articles/762548/) — Перевод статьи из серии «Back to Basics»: Что такое указатели, что такое итераторы, и чем они отличаются.
2. 🇷🇺 Habr: [Визуализация алгоритмов стандартной библиотеки C++](https://habr.com/ru/articles/762554/) ([продолжение](https://habr.com/ru/articles/763024/)) — Визуализация работы стандартных алгоритмов `std::reduce`, `std::shuffle`, `std::lower_bound`, `std::sort` и других.
3. 🇷🇺 Habr: Промышленные контроллеры, Linux и только C++ ([Часть 1](https://habr.com/ru/articles/762576/), [Часть 2](https://habr.com/ru/articles/764116/)) — Сборник наработок по работе с протоколами Modbus и MQTT на C++.
4. 🇷🇺 Habr: [Когда private, но очень хочется public](https://habr.com/ru/articles/762250/) — Практическое пособие, как можно сломать механизм инкапсуляции в C++.
5. 🇷🇺 Habr: [Форматирование текста на C++ старым и новым способом](https://habr.com/ru/companies/ruvds/articles/761910/) — Обзор различных способов форматирования текста в C++: с помощью потоков, `printf`-подобных функций, библиотеки форматирования C++20 и сторонней библиотеки [libfmt](https://github.com/fmtlib/fmt).
6. 🇷🇺 Habr: [Fibers в C++: основы](https://habr.com/ru/articles/763074/) — Теоретические основы fibers, легковесной альтернативы потоков.
7. 🇷🇺 Habr: [Блеск и нищета std::format](https://habr.com/ru/articles/763784/) — О подводных камнях работы с `std::format`.
8. 🇷🇺 Habr: [Как мы анализируем потребление памяти нативными приложениями (C++, Windows, Linux)](https://habr.com/ru/companies/1c/articles/761012/)
9. 🇷🇺 Habr: [Шпаргалка по модели памяти С++11](https://habr.com/ru/companies/otus/articles/763810/) — Обзор модели памяти C++11, впервые позволившей писать на плюсах кроссплатформенные многопоточные программы.
10. 🇷🇺 Habr: [Федя, дичь](https://habr.com/ru/articles/764514/) — Подборка интересных багов в плюсовом коде: попробуйте найти их все!
11. Bartłomiej Filipek: [2 Lines Of Code and 3 C++17 Features - The overload Pattern](https://www.cppstories.com/2019/02/2lines3featuresoverload.html/) — Обзор одного интересного и полезного паттерна, в двух строчках (который благодаря C++20 могут превратиться в одну) своей реализации демонстрирующего сразу три нововведения C++17.
12. KDAB Team (осторожно, для чтения требуется VPN): [GitHub Actions for C++ and Qt](https://www.kdab.com/github-actions-for-cpp-and-qt/) — Введение в Github Actions с примером настройки workflow для плюсовой программы, использующей Qt.
13. Daniel Lemire: [Parsing integers quickly with AVX-512](https://lemire.me/blog/2023/09/22/parsing-integers-quickly-with-avx-512/) — Ускорение `std::from_chars` в несколько раз с помощью инструкций AVX-512.
14. Raymond Chen: [The dangers of releasing the last strong reference from within its own callback](https://devblogs.microsoft.com/oldnewthing/20230927-00/?p=108831) — Об одной из опасностей, которую таит в себе работа с колбэками.

## 📺 Видео и доклады

1. Jason Turner: [C++ Weekly — Ep 394 — C++11's Most Overlooked Feature: Delegating Constructors](https://www.youtube.com/watch?v=G5ewfxJ0KMU) — Обзор одного из нововведений C++11: [делегирующих конструкторов](https://learn.microsoft.com/en-us/cpp/cpp/delegating-constructors?view=msvc-170).

### CppCon

1. [Interview with Kristen Shaker (How to Build Your First C++ Automated Refactoring Tool)](https://www.youtube.com/watch?v=7UCeltE3gF4) — Интервью с Кристин Шейкер, инженером Google’s C++ Core Libraries Team: Об автоматизации рефакторинга с помощью clang.

### Meeting C++

1. [Meeting C++ live with Kevlin Henney](https://www.youtube.com/watch?v=O0BghVOugXc) — Интервью с Кевином Хинли, независимым консультантом и автором множества статей и докладов про C++: О [cppfront](https://learn.microsoft.com/en-us/cpp/cpp/delegating-constructors?view=msvc-170), юнит-, мок- тестировании и параллелизме в C++.

## Послесловие

> Дайджест составлен и опубликован при поддержке московского сообщества программистов [C++ Moscow](https://t.me/cppmoscow_info)

Заметили ошибку или опечатку? Сообщите в личку ([telegram](https://t.me/eoanermine), [habr](https://habr.com/ru/conversations/eoanermine/))

Прислать ссылку можно [через форму](https://forms.yandex.ru/cloud/64f48043e010db921819c447/) или просто написав мне в личные сообщения ([telegram](https://t.me/eoanermine), [habr](https://habr.com/ru/conversations/eoanermine/))

← Предыдущий выпуск: [C++ Дайджест №3](https://habr.com/ru/articles/761786/)
