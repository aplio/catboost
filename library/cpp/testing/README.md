В этой директории лежат библиотеки для удобного написания тестов на C++, а именно:

* `benchmark` — библиотека для реализации простых бенчмарков.
* `boost_test` — реализация тестирования средствами библиотеки _boost_. **Не используйте этот фреймворк в новом коде.**
* `boost_test_main` — реализация (средствами библиотеки _boost_) функции `int main(argc, argv)` для модуля `BOOSTTEST`. **Не используйте этот фреймворк в новом коде.**
* `gtest` — реализация модуля `GTEST_BETA` — средства для интеграции фреймворка _googletest_ в Аркадию
* `gtest_extensions` — реализация `PrintTo` (отладочной печати) для некоторых общеаркадийных типов: TString, TStringBuf, TMaybe, TVariant (список может быть неполон). Включена в модуле `GTEST_BETA` по умолчанию. Поддержка матчеров gmock для строковых типов.
* `gtest_main` — реализация `int main(argc, argv)` для модуля `GTEST_BETA` (вынесена в отдельную библиотеку, чтобы в перспективе была возможна реализация `GTEST_WITH_CUSTOM_ENTRY_POINT`)
* `mock_server` — реализация http-сервера для тестов.

По недосмотру отсутствуют в данной директории:

* `library/unittest` — реализация модуля UNITTEST — основного средства для тестирования тестов на С++ в Аркадии.
* `library/unittest/main` — реализация `int main(argc, argv)` для модуля UNITTEST (она вынесена в отдельную библиотеку, чтобы оставить возможность для реализации `UNITTEST_WITH_CUSTOM_ENTRY_POINT` и `YT_UNITTEST`.
* Содержимое директории `library/testing` — будет перемещено в рамках тикетов из очереди SUBBOTNIK.
