## ver 1
### Run
- скачть и открыть в браузере form072_v1.html
### Settings
form072_v1.html  
Конфигурация внутри js:
```
        const CONFIG = {
            Settings: {
                inData: 'File',             // 'File' или 'DataSet'. File - предложить открыть файл, а DataSet - брать из переменной DataSetRef: 'DATASET_072',
                outData: 'mermaid.live',    // 'mermaid.live' или 'text'
                DataSetRef: 'DATASET_072v3',// имя глобальной переменной с данными
                sysSourceTarget: 'no'      // показывать источники_8 и получатели_9 данных: yes - показывать (show) , иное не показывать
            }
        };
```
Опции:
- При выборе File (inData: 'File') есть примеры: f072r7v1.txt и f072r7v3.txt (более сложный), см. https://github.com/bpmbpm/Form072/tree/main/example
- При выборе outData: 'mermaid.live', открывается граф в https://mermaid.live/view с редактором: https://mermaid.live/edit

Файл f072r7v2ai.txt - как демонстрация от ["плохого парня" - архитектора ИИ](https://github.com/bpmbpm/Form072/wiki/example-form#2-%D0%BF%D1%80%D0%B8%D0%B2%D0%B5%D0%B4%D0%B8-%D0%BF%D1%80%D0%B8%D0%BC%D0%B5%D1%80-%D0%BE%D0%BF%D0%B8%D1%81%D1%8B%D0%B2%D0%B0%D1%8E%D1%89%D0%B8%D0%B9-%D0%B2%D1%81%D1%8E-%D0%B8%D1%82-%D1%81%D0%B8%D1%81%D1%82%D0%B5%D0%BC%D1%83-%D0%B1%D0%B0%D0%BD%D0%BA%D0%B0-%D0%BA%D0%B0%D0%BA-%D0%BC%D0%B8%D0%BD%D0%B8%D0%BC%D1%83%D0%BC-30-%D1%81%D1%82%D1%80%D0%BE%D0%BA)
