## Проектные задачи компьютерной лингвистики

Цель курса – обеспечить системное представление о современных методах обработки текстовых данных с использованием машинного обучения и нейронных сетей, а также сформировать практические навыки их применения. Программа разделена на теоретическую и проектную части, что позволяет студентам не только освоить ключевые концепции, но и применить их в процессе научно-исследовательской работы.

Курс является обязательным для студентов 4 курса бакалавриата кафедры теоретической и прикладной лингвистики МГУ им. М. В. Ломоносова.

Материалы курса выложены в данном репозитории. Запущенные блокноты можно найти на гугл-диске по <a href="https://drive.google.com/drive/folders/1N5D--B3mBZqXExfDNgvvqxrXDSzb3bZV?usp=sharing">ссылке</a>.

<!DOCTYPE html>
<html>
    <table>
        <tr>
    <th>Тема</th>
    <th>Содержание</th>
    <th>Материалы</th>
  </tr>
        <tr>
            <td colspan="3" ><a href="https://github.com/Xeanst/project_tasks_in_compling/tree/main/1_theoretical_part">I. Теоретическая часть</a></td>
        </tr>
        <tr>
            <td>1. Введение в обработку текстовых данных</td>
            <td>
                <li>Предобработка текста: токенизация, приведение к нижнему регистру, удаление стоп-слов, нормализация (стемминг и лемматизация).</li>
                <li>Методы векторизации текстов: мешок слов, TF-IDF.</li>
                <li>Алгоритмы классификации: наивный байесовский классификатор, логистическая регрессия, дерево решений, наивный байесовский классификатор, случайный лес.</li>
                <li>Меры качества классификации.</li>
                <li>Пример классификации новостных текстов по тематикам.</li>
            </td>
            <td><a href="https://github.com/Xeanst/project_tasks_in_compling/blob/main/1_theoretical_part/01_Intro_to_NLP.ipynb">Colab-блокнот</a></td>
        </tr>
        <tr>
            <td>2. Векторные представления слов</td>
            <td>
                <li>Модель word2vec: алгоритмы skip-gram и CBOW.</li>
                <li>Оптимизация negative sampling.</li>
                <li>FastText: векторы для символьных n-грамм.</li>
                <li>Самостоятельная реализация в pytorch.</li>
                <li>Использование предобученных моделей.</li>
            </td>
            <td><a href="https://github.com/Xeanst/project_tasks_in_compling/blob/main/1_theoretical_part/02_Word_embeddings.ipynb">Colab-блокнот</a></td>
        </tr>
        <tr>
            <td>3. Языковое моделирование</td>
            <td>
                <li>Вероятность слов и предложений на основе корпуса.</li>
                <li>N-граммные модели. Сглаживание Лапласа.</li>
                <li>Генерация текста. Перплексия.</li>
                <li>Генерация текста статьи с помощью n-граммных моделей.</li>
                <li>Нейросетевые языковые модели.</li>
                <li>Архитектура рекуррентных нейронных сетей.</li>
                <li>Типы задач: один к одному, один ко многим, многие к одному, многие ко многим.</li>
                <li>Сеть долгой краткосрочной памяти.</li>
                <li>Применение LSTM для посимвольной генерации.</li>
                </td>
            <td class="link-column"><a href="https://github.com/Xeanst/project_tasks_in_compling/blob/main/1_theoretical_part/03_Language_modeling.ipynb">Colab-блокнот</a></td>
        </tr>
        <tr>
            <td>4. Механизм внимания</td>
            <td>
                <li>Постановка задачи sequence2sequence (seq2seq) на примере машинного перевода.</li>
                <li>Архитектура энкодер-декодер.</li>
                <li>Недостатки стандартной модели.</li>
                <li>Пример реализации машинного перевода.</li>
                <li>Визуализация весов внимания.</li>
                <li>Оценка качества машинного перевода.</li>
                </td>
            <td><a href="https://github.com/Xeanst/project_tasks_in_compling/blob/main/1_theoretical_part/04_Attention.ipynb">Colab-блокнот</a></td>
        </tr>
        <tr>
            <td>5. Архитектура Трансформер</td>
            <td>
                <li>Механизм внутреннего внимания.</li>
                <li>Множественное внимание.</li>
                <li>Кодирование позиции.</li>
                <li>Нормализация слоя. Сквозная связь.</li>
                <li>Оптимизация и регуляризация.</li>
                <li>Примеры на искусственных и на реальных данных.</li>
                <li>Развитие архитектуры Трансформер.</li>
                <li>Модели BART, T5.</li>
            </td>
            <td><a href="https://github.com/Xeanst/project_tasks_in_compling/blob/main/1_theoretical_part/05_Transformer.ipynb">Colab-блокнот</a></td>
        </tr>
        <tr>
            <td>6. Модели на основе энкодера Трансформера</td>
            <td>
                <li>Использование предобученных векторов ELMo.</li>
                <li>Модель BERT на основе энкодера трансформера.</li>
                <li>Маскированное языковое моделирование.</li>
                <li>Предсказание следующего предложения.</li>
                <li>Библиотека Transformers.</li>
                <li>Токенизация на подслова.</li>
                <li>Тонкая настройка для определения логического следования.</li>
                </td>
            <td><a href="https://github.com/Xeanst/project_tasks_in_compling/blob/main/1_theoretical_part/06_Encoder.ipynb">Colab-блокнот</a></td>
        </tr>
        <tr>
            <td>7. Модели на основе декодера Трансформера</td>
            <td>
                <li>Модель GPT и открытые модели.</li>
                <li>Методы генерации текста: жадный поиск, поиск по лучу, сэмплирование с температурой.</li>
                <li>Затравочное программирование.</li>
                <li>Обучение с подкреплением с обратной связью от человека.</li>
                <li>Проблемы дообучения больших моделей.</li>
                <li>Методы эффективной тонкой настройки.</li>
                <li>Пример тонкой настройки с помощью LoRA.</li>
            </td>
            <td><a href="https://github.com/Xeanst/project_tasks_in_compling/blob/main/1_theoretical_part/07_Decoder.ipynb">Colab-блокнот</a></td>
        </tr>
        <tr>
            <td colspan="3"><a href="https://github.com/Xeanst/project_tasks_in_compling/tree/main/2_project_part">II. Проектная часть</a></td>
        </tr>
        <tr>
            <td>8. Анализ тональности к именованным сущностям в новостных текстах</td>
            <td>
                <li>Особенности новостных текстов с точки зрения анализа тональности.</li>
                <li>Соревнование RuSentNE-2023:
                    <ul>
                        <li>постановка задачи,</li>
                        <li>нализ датасета,</li>
                        <li>метрики.</li>
                        </ul></li>
                <li>Воспроизведение бейзлайна: тонкая настройка модели RuBERT base conversational для классификации пары предложений:
                    <ul>
                      <li>1) Вопрос «Как относятся к X?» где Х — сущность в дательном падеже;</li>
                      <li>2) Текст предложения.</li>
                    </ul></li>
            </td>
            <td>
                <a href="https://github.com/Xeanst/project_tasks_in_compling/blob/main/2_project_part/08_RuSentNE/08_RuSentNE.pdf">Презентация</a><br>
                <a href="https://github.com/Xeanst/project_tasks_in_compling/blob/main/2_project_part/08_RuSentNE/08_RuSentNE.ipynb">Colab-блокнот</a>
            </td>
        </tr>
        <tr>
            <td>9. Извлечение мнений из новостных текстов</td>
            <td>
                <li>Предшествующие исследования: графовый подход, разметка последовательности.</li>
                <li>Соревнование RuOpinionNE-2024:
                    <ul>
                        <li>постановка задачи,</li>
                        <li>анализ датасета,</li>
                        <li>метрики.</li>
                    </ul>
                    </li>
                <li>Воспроизведение бейзлайна: применение модели Qwen2.5 72B instruct в режиме few-shot.</li>
            </td>
            <td>
                <a href="https://github.com/Xeanst/project_tasks_in_compling/blob/main/2_project_part/09_RuOpinionNE/09_RuOpinionNE.pdf">Презентация</a><br>
                <a href="https://github.com/Xeanst/project_tasks_in_compling/blob/main/2_project_part/09_RuOpinionNE/09_RuOpinionNE.ipynb">Colab-блокнот</a>
            </td>
        </tr>
        <tr>
            <td>10. Анализ аргументации</td>
            <td>
                <li>Аргумент как утверждение, содержащее позицию и довод.</li>
                <li>Соревнование RuArg-2022:
                    <ul>
                        <li>постановка задачи,</li>
                        <li>анализ датасета,</li>
                        <li>метрики.</li>
                    </ul></li>
                <li>Воспроизведение бейзлайна: тонкая настройка отдельной модели Sentence RuBERT по каждой теме:
                    <ul>
                        <li>«маски»,</li>
                        <li>«карантин»,</li>
                        <li>«вакцины».</li>
                    </ul></li></li></td>
            <td>
                <a href="https://github.com/Xeanst/project_tasks_in_compling/blob/main/2_project_part/10_RuArg/10_RuArg.pdf">Презентация</a><br>
                <a href="https://github.com/Xeanst/project_tasks_in_compling/blob/main/2_project_part/10_RuArg/10_RuArg.ipynb">Colab-блокнот</a>
            </td>
        </tr>
        <tr>
            <td>11. Представление тем проектных работ</td>
            <td>
                <li>Выступления студентов.</li>
                <li>Постановка цели и задач проектной работы.</li>
                <li>Обзор существующих методов и подходов.</li>
                <li>Определение репрезентативности данных, их дисбаланс, выбросы и пропуски в данных.</li>
                <li>Выбор и обоснование целевых метрик.</li>
                <li>Выбор моделей для планируемых экспериментов.</li>
                <li>Обсуждение с преподавателем и другими студентами.</li></td>
            <td><a href="https://github.com/Xeanst/project_tasks_in_compling/tree/main/2_project_part/11_Topic_presentation">Презентации</a></td>
        </tr>
        <tr>
            <td>12. Методы подбора инструкций для больших языковых моделей</td>
            <td>
                <li>Платформы для доступа к LLM по API: Yandex Cloud, Sber, Mistral AI, Together AI, Hugging Face, GroqCloud.</li>
                <li.Преимущества и недостатки: скорость работы, стоимость, ограничения.</li>
                <li>Методы подбора инструкций (prompt engineering) для работы с LLM.</li>
                <li>Генерация ответа в режиме zero-shot и few-shot.</li>
                </li>Наиболее продвинутые техники: цепочка размышлений (Chain-of-Thoughts), самосогласованность (self-consistency), установка роли (role prompting).</li>
                </td>
            <td><a href="https://github.com/Xeanst/project_tasks_in_compling/blob/main/2_project_part/12_LLM_prompting.ipynb">Colab-блокнот</a></td>
        </tr>
        <tr>
            <td>13. Объяснимость моделей машинного обучения</td>
            <td>
                <li>Важность понимания решений моделей.
                <li>Деление моделей на прозрачные и непрозрачные с точки зрения интерпретируемости.</li>
                <li>Объяснимость моделей классического ML: линейных моделей, деревьев решений.</li>
                <li>Методы объяснения, независимые от модели (model-agnostic): ICE, LIME, SHAP.</li>
                <li>Практическая реализация для различных задач.</li>
            </td>
            <td><a href="https://github.com/Xeanst/project_tasks_in_compling/blob/main/2_project_part/13_Explainability.ipynb">Colab-блокнот</a></td>
        </tr>
        <tr>
            <td>14. Итоговая защита проектов</td>
            <td>
                <li>Представление результатов выполненных проектов.</li>
                <li>Описание опробованных гиперпараметров модели и проведенных экспериментов по улучшению качества.</li>
                <li>Сопоставление итогов проекта с предыдущими работами в этой области.</li>
                <li>Практическая применимость результатов.</li>
                <li>Рецензирование работ друг друга.</li>
                <li>Ответы на вопросы.</li>
            </td>
            <td><a href="https://github.com/Xeanst/project_tasks_in_compling/tree/main/2_project_part/14_Project_defense">Проекты</a></td>
        </tr>
</table>
</html>
