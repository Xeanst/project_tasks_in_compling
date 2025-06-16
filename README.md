<!DOCTYPE html>
<html>
    <table>
        <tr>
            <td colspan="3" >А. Теоретическая часть</td>
        </tr>
        <tr>
            <td>1. Введение в обработку текстовых данных</td>
            <td>Предобработка текста: токенизация, приведение к нижнему регистру, удаление стоп-слов, нормализация (стемминг и лемматизация). Методы векторизации текстов: мешок слов, TF-IDF. Алгоритмы классификации: наивный байесовский классификатор, логистическая регрессия, дерево решений, наивный байесовский классификатор, случайный лес. Меры качества классификации. Пример классификации новостных текстов по тематикам.</td>
            <td><a href="https://colab.research.google.com/drive/1iWF2hisv50MZ7AKi585tPldjEYmeAxay?usp=sharing">Ссылка</a></td>
        </tr>
        
        <tr>
            <td>2. Векторные представления слов</td>
            <td>Модель word2vec: алгоритмы skip-gram и CBOW. Оптимизация negative sampling. FastText: векторы для символьных n-грамм. Самостоятельная реализация в pytorch. Использование предобученных моделей.</td>
            <td class="link-column"><a href="https://colab.research.google.com/drive/1fx7U398lcwIoPGp1vn2e5_vjLnu5lQjf?usp=sharing">Ссылка</a></td>
        </tr>
        
        <tr>
            <td>3. Языковое моделирование</td>
            <td>Вероятность слов и предложений на основе корпуса. N-граммные модели. Сглаживание Лапласа. Генерация текста. Перплексия. Генерация текста статьи с помощью n-граммных моделей. Нейросетевые языковые модели. Архитектура рекуррентных нейронных сетей. Типы задач: один к одному, один ко многим, многие к одному, многие ко многим. Сеть долгой краткосрочной памяти. Применение LSTM для посимвольной генерации.</td>
            <td class="link-column"><a href="https://colab.research.google.com/drive/10XFszxpbWVREx1vAVleixIddZ_R0NlqR?usp=sharing">Ссылка</a></td>
        </tr>
        
        <tr>
            <td>4. Механизм внимания</td>
            <td>Постановка задачи sequence2sequence (seq2seq) на примере машинного перевода. Архитектура энкодер-декодер. Недостатки стандартной модели. Пример реализации машинного перевода. Визуализация весов внимания. Оценка качества машинного перевода.</td>
            <td class="link-column"><a href="https://colab.research.google.com/drive/1-hg_qXMwZXcPiks5mPuSXsPdNccbyZZN?usp=sharing">Ссылка</a></td>
        </tr>
        
        <tr>
            <td>5. Архитектура Трансформер</td>
            <td>Механизм внутреннего внимания. Множественное внимание. Кодирование позиции. Нормализация слоя. Сквозная связь. Оптимизация и регуляризация. Примеры на искусственных и на реальных данных. Развитие архитектуры Трансформер. Модели BART, T5.</td>
            <td class="link-column"><a href="https://colab.research.google.com/drive/1KUSuJkKaww5QXhNUMoN3MYZqdKhxqILE?usp=sharing">Ссылка</a></td>
        </tr>
        
        <tr>
            <td>6. Модели на основе энкодера Трансформера</td>
            <td>Использование предобученных векторов ELMo. Модель BERT на основе энкодера трансформера. Маскированное языковое моделирование. Предсказание следующего предложения. Библиотека Transformers. Токенизация на подслова. Тонкая настройка для определения логического следования.</td>
            <td class="link-column"><a href="https://colab.research.google.com/drive/1sGSHCxC3H_plgpRalfRiHI9x7qrRBV65?usp=sharing">Ссылка</a></td>
        </tr>
        
        <tr>
            <td>7. Модели на основе декодера Трансформера</td>
            <td>Модель GPT и открытые модели. Методы генерации текста: жадный поиск, поиск по лучу, сэмплирование с температурой. Затравочное программирование. Обучение с подкреплением с обратной связью от человека. Проблемы дообучения больших моделей. Методы PEFT. Пример тонкой настройки с помощью LoRA.</td>
            <td class="link-column"><a href="https://colab.research.google.com/drive/1ceGd9wwzhJf9srL50NSr-SV0Ys-DWmC0?usp=sharing">Ссылка</a></td>
        </tr>
        
        <tr>
            <th colspan="3" class="section-header">Б. Проектная часть</th>
        </tr>
        
        <tr>
            <td>8. Анализ тональности к именованным сущностям в новостных текстах</td>
            <td>Особенности новостных текстов с точки зрения анализа тональности. Соревнование RuSentNE-2023: постановка задачи, анализ датасета, метрики. Воспроизведение бейзлайна: тонкая настройка модели RuBERT base conversational для классификации пары предложений: 1) Вопрос «Как относятся к X?» где Х — сущность в дательном падеже; 2) Текст предложения.</td>
            <td class="link-column">
                <a href="https://drive.google.com/file/d/125-u2a68TYi2LBqoT6X0iw2Jflwa-kpO/view?usp=sharing">Ссылка 1</a><br>
                <a href="https://colab.research.google.com/drive/1X5pew_-CNX63eP8ueNnnURRngzVSpY6K?usp=sharing">Ссылка 2</a>
            </td>
        </tr>
        
        <tr>
            <td>9. Извлечение мнений из новостных текстов</td>
            <td>Предшествующие исследования: графовый подход, разметка последовательности. Соревнование RuOpinionNE-2024: постановка задачи, анализ датасета, метрики. Воспроизведение бейзлайна: применение модели Qwen2.5 72B instruct в режиме few-shot.</td>
            <td class="link-column">
                <a href="https://drive.google.com/file/d/1RuSHU472CwvWeDoZ9cqVluVS5Vfl-DUS/view?usp=sharing">Ссылка 1</a><br>
                <a href="https://colab.research.google.com/drive/13LIYbe95t-fKL7QMvuU71k8LRVNLXY5q?usp=sharing">Ссылка 2</a>
            </td>
        </tr>
        
        <tr>
            <td>10. Анализ аргументации</td>
            <td>Аргумент как утверждение, содержащее позицию и довод. Соревнование RuArg-2022: постановка задачи, анализ датасета, метрики. Воспроизведение бейзлайна: тонкая настройка отдельной модели Sentence RuBERT по каждой теме: «маски», «карантин», «вакцины».</td>
            <td class="link-column">
                <a href="https://drive.google.com/file/d/1tG6GeZ-hE09CDgYuvNY5cQ0-_uPe_lQp/view?usp=sharing">Ссылка 1</a><br>
                <a href="https://colab.research.google.com/drive/1J4-LHvIhoXXSRoy8z_A7pRv9AyZDy2Jp?usp=sharing">Ссылка 2</a>
            </td>
        </tr>
        
        <tr>
            <td>11. Представление тем проектных работ</td>
            <td>Выступления студентов. Постановка цели и задач проектной работы. Обзор существующих методов и подходов. Определение репрезентативности данных, их дисбаланс, выбросы и пропуски в данных. Выбор и обоснование целевых метрик. Выбор моделей для планируемых экспериментов. Обсуждение с преподавателем и другими студентами.</td>
            <td class="link-column"><a href="https://drive.google.com/drive/folders/1Yl-eMVuxB1YgnelhMWXAkCHzJt57XR2j?usp=sharing">Ссылка</a></td>
        </tr>
        
        <tr>
            <td>12. Методы подбора инструкций для больших языковых моделей</td>
            <td>Платформы для доступа к LLM по API: Yandex Cloud, Sber, Mistral AI, Together AI, Hugging Face, GroqCloud. Преимущества и недостатки: скорость работы, стоимость, ограничения. Методы подбора инструкций (prompt engineering) для работы с LLM. Генерация ответа в режиме zero-shot и few-shot. Наиболее продвинутые техники: цепочка размышлений (Chain-of-Thoughts), самосогласованность (self-consistency), установка роли (role prompting).</td>
            <td class="link-column"><a href="https://colab.research.google.com/drive/12twkTbImoJrwDDAVL18_JjNqRiLbt0oK?usp=sharing">Ссылка</a></td>
        </tr>
        
        <tr>
            <td>13. Объяснимость моделей машинного обучения</td>
            <td>Важность понимания решений моделей. Деление моделей на прозрачные и непрозрачные с точки зрения интерпретируемости. Объяснимость моделей классического ML: линейных моделей, деревьев решений. Методы объяснения, независимые от модели (model-agnostic): ICE, LIME, SHAP. Практическая реализация для различных задач.</td>
            <td class="link-column"><a href="https://colab.research.google.com/drive/1d-td9O3yvNz360y4cLUIiXIaNK0KSuDq?usp=sharing">Ссылка</a></td>
        </tr>
        
        <tr>
            <td>14. Итоговая защита проектов</td>
            <td>Представление результатов выполненных проектов. Описание опробованных гиперпараметров модели и проведенных экспериментов по улучшению качества. Сопоставление итогов проекта с предыдущими работами в этой области. Практическая применимость результатов. Рецензирование работ друг друга. Ответы на вопросы.</td>
            <td class="link-column"><a href="https://drive.google.com/drive/folders/1vzof0gS5E98sag30Z_23e4wIPGaNKJUY?usp=sharing">Ссылка</a></td>
        </tr>
    </table>
</html>
