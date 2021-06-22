# Схема описания тега

```json
{
    "tagName": "", // имя тега - например "body"
    "structure": [
        {
            "type": "categories", // Виды контента (https://html.spec.whatwg.org/multipage/dom.html#kinds-of-content)
            "value": [""] // Доступные варианты:
            // 'metadata content'
            // 'flow content'
            // 'sectioning content'
            // heading content
            // phrasing content
            // embedded content
            // interactive content
        },
        {
            "type": "tag_omission", // Возможен ли пропуск тега
            "value": [""] // Доступные варианты:
            // Закрывающий тен обязателен.
        },
        {
            "type": "description", // Базовое описание компонента
            "value": [""] // Строки описывающие элемент. Каждый элемент массива (строка) являются параграфом и имеют отступы между собой.
        },
        {
            "type": "content_model", // Нормативное описание того, какой контент должен быть включен в качестве потомков
            "value": "---" // Текстовое описание.
        },
        {
            "type": "content_attributes", // Cписок атрибутов, которые могут быть указаны в элементе, а также ненормативные описания этих атрибутов.
            "value": {
                "global_attributes": false, // Есть ли у элемента список глобальных атрибутов.
                "custom_attributes": [ // частные случаи атрибутов на элементе
                    {
                        "name": "---", // имя аттрибута - например "type"
                        "description": "---" // описание атрибута - например - "Тип элемента"
                    }
                ]
            }
        },
        {
            "type": "example", // Присутствует ли пример для данного тега.
            "value": false
        },
        // Необязательный - указывать только если элемент устаревший
        {
            "type": "obsolete", // Является ли элемент устаревшим
            "value": true
        }
    ]
}

```
