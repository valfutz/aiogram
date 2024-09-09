===============
Handling events
===============

*aiogram* включає в себе механізм Dispatcher. 
Dispatcher потрібен для обробки вхідних оновлень з Telegram.

За допомогою Dispatcher ви можете:

- Обробляти вхідні оновлення;
- Фільтрувати вхідні події перед тим, як вони будуть оброблені певним обробником;
- Змінювати події та пов'язані з ними дані в проміжних модулях;
- Розділяти функціонал бота між різними обробниками, модулями та пакетами.

Dispatcher також розділений на дві сутності - Router та Dispatcher.
Dispatcher є підкласом маршрутизатора і завжди повинен бути кореневим маршрутизатором.

Telegram підтримує два способи отримання оновлень:
- :ref:`Webhook <webhook>` - ви повинні налаштувати свій веб-сервер на отримання оновлень від Telegram;
- :ref:`Long polling <long-polling>` - ви повинні запитувати оновлення від Telegram.
Отже, ви можете використовувати обидва способи з *aiogram*.

.. toctree::

    router
    dispatcher
    dependency_injection
    filters/index
    long_polling
    finite_state_machine/index
    middlewares
    errors
    flags
    webhook
    class_based_handlers/index
