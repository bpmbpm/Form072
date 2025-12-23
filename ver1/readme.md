## ver 1
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
- При выборе File (inData: 'File') есть примеры: f072r7v1.txt и f072r7v3.txt (более сложный), см. https://github.com/bpmbpm/Form072/tree/main/example
- При выборе outData: 'mermaid.live', открывается граф в https://mermaid.live/view с редактором: https://mermaid.live/edit
