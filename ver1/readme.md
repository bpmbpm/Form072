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
