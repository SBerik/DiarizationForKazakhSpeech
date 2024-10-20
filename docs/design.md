# Описание пайплайна

Пайплайн обработки аудио выглядит следующим образом:

## Шаги пайплайна

1. **Входные данные**: Подается сырая аудио дорожка.

2. **Удаление не речевых сегментов**: 
   - Используется метод VAD (Voice Activity Detection) для устранения промежутков, где отсутствует речь. 
   - На этом этапе производится сегментация аудио, оставляя только тайминг речевых фрагментов.

3. **Извлечение признаков**: 
   - Из выделенных речевых сегментов извлекаются характеристики (признаки) для дальнейшей обработки.

## Примечания
- Убедитесь, что аудио дорожка в подходящем формате перед подачей в систему.
- Рекомендуется протестировать VAD на различных типах аудио для оптимизации качества сегментации.