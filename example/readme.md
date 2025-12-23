## Example 
## 1 Easy
Особенности: 
- Данные взяты из https://github.com/bpmbpm/doc/blob/main/IT/reliability_risk/risk/850P/f072/server.md  
- Упрощено, включая, минимазацию компонентов, отказ от виртуализациии и т.п.
- пример арх-строки из которой формируются объекты графа:
  - ТпрКО8|Lekton Classic|ОУ|БфКО22|Фронт-офисная система учета с использованием пластиковых карт|lekton|Урв1|АС1|АС2|Windows 10|Прин1| Ри2|microsoft|21H2|Клсо99|Клс1|840|Не применимо|Лиц9|Арх3.1|Не применимо|Закуп5|Поддерж4|Авт1|Обнв4|Уязв1|Упр1|ФСТЭК9|Не применимо|ФСБ9|Не применимо|Отсутствует|Не применимо|Отсутствует
   
### 1.1 fragment of process TprKO6
ТпрКО6 - открытие и ведение счетов ФЛ. 
```
const CONFIG = {
Settings: {
DataSetRef: 'DATASET_072v1',
```
``` mermaid
graph LR;
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.3((Арх3.3)) --> АБС1_ЦФТ:Арх3.3:software((software)) --> АБС1_ЦФТАрх3.3Прикладное_ПО:_ЦФТ-Банк_Платформы_2MCA_DBI:Ри2([Прикладное ПО: ЦФТ-Банк Платформы 2MCA DBI<br>2.9.3<br>АО ЦФТ, 810]) 
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.3((Арх3.3)) --> АБС1_ЦФТ:Арх3.3:software((software)) --> АБС1_ЦФТАрх3.3Сервер_приложений:_Apache_Tomcat:Ри2([Сервер приложений: Apache Tomcat<br>9.0.85<br>Apache Software Foundation, 840]) 
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.3((Арх3.3)) --> АБС1_ЦФТ:Арх3.3:software((software)) --> АБС1_ЦФТАрх3.3Среда_исполнения:_Oracle_JDK_:Ри2([Среда исполнения: Oracle JDK <br>17.0.11<br>Oracle Inc., 840]) 
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.3((Арх3.3)) --> АБС1_ЦФТ:Арх3.3:software((software)) --> АБС1_ЦФТАрх3.3Системное_ПО,_ОС:_Ред_ОС_Сервер:Ри2([Системное ПО, ОС: Ред ОС Сервер<br>10.2<br>ООО «Ред Софт», 810]) 
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.3((Арх3.3)) --> АБС1_ЦФТ:Арх3.3:hardware((hardware)) --> АБС1_ЦФТАрх3.3Оборудование,_сервер:_Aquarius_C86_:Ри2([Оборудование, сервер: Aquarius C86 <br>T1F S28H<br>ГК «Аквариус», 810]) 
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.2((Арх3.2)) --> АБС1_ЦФТ:Арх3.2:software((software)) --> АБС1_ЦФТАрх3.2Прикладное_ПО,_СУБД:_Postgres_Pro_Enterprise:Ри2([Прикладное ПО, СУБД: Postgres Pro Enterprise<br>15.6.1<br>ООО «Постгрес Про», 810]) 
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.2((Арх3.2)) --> АБС1_ЦФТ:Арх3.2:software((software)) --> АБС1_ЦФТАрх3.2Системное_ПО,_ОС:_Ред_ОС_Сервер:Ри2([Системное ПО, ОС: Ред ОС Сервер<br>10.2<br>ООО «Ред Софт», 810]) 
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.2((Арх3.2)) --> АБС1_ЦФТ:Арх3.2:hardware((hardware)) --> АБС1_ЦФТАрх3.2Оборудование_сервера:_Aquarius_C86_:Ри2([Оборудование сервера: Aquarius C86 <br>T1F D88<br>ГК «Аквариус», 810]) 
```

- [mermaid.live](https://mermaid.live/view#pako:eNrtl8tu00AUhl_laFap5Fj2uEkdgyqVlooCFQi6gqCRSdwmUmMHxxGXqhItsGJBEay6SC8gNmxCISjQUiSe4PiNODNxLi1poRILoChSNGPP_-fM5-M_9hIrBEWPOWwhdKsluHztTN7HbfwaP8R1bGQhnR4HXMPnuGUKfIOvcTuVTKEzPXs7HMdGvIJfcB936LsZP0sUgO-wSUc-Y1OThxqJw8gQVwfX4ofxE0u3UqnecOT4lU4tmI_uuqGXSnVHQxU9AW7QttpUzy7V9UFV3BK4gQ0nWZkmmapYHqVF8Wr8GPdJtBc_FXx2ckJMnZtxcBPbPHVzmBsoNzjkBj-6gXQDcpP8uJ7TLQWSICViDWzTuDUC__Ll2MIWbWxHfgu1xzZh2seP2KIy2_jJERNVt1DyxFxQKbhRD_yADobqoKODjk4yyemGbmfkKDl1PSkRpoO6X3SjcuAT8tF_Hjltq0Xd2hTYppK_Usm7VKACFz9zxJXQLSx64uLUJdHH3dXAUA10NEAakCzMMWJtmnKYnJnxC_qpgCv5xKtEZm8gXDSBDdyiiNmUFNVEDLbwQFsfkqs0ob1JOXTkagKDcoXc0HmHlPzAt7fdxVuUN4_j1W-7f2GclNyw2MHfHf0Ef4MqoniNH1GvymqbKg1amqD6-7TFxJ26G5brNTFpZ_tNfpQYDoihKwYSq26fM6fhOrcvKFIvcF3CXyMo5CCDKX4Ur_wx9HmfPj-ePj9p8_Mj_1s12eyvSPPSEVeDWrQQejVxNQzEeT_ywmpYrnk__UfVoOcBXQ8gD-h7qNsgo2d18-CNsEFXVd5U72WIxSugfmP_dFyS_3n0O_GfMI_4UZFyII6wecJAgkPq4Yk0Zdu_FEhMowf_cpE5UVj3NFbxwoorp2wp7wPkWVTyKl6eOTQsevNufTHKs7y_TLKq698IgkpXGQb1hRJz5t3FGs3qVXqi8qbKLr1V9Jd4ftELJ-lxK2JOTjkwZ4ndYw63TJ3nLINzy7AtnrE0dp85aT6qG9wwctmMbRlWxswta-yB-k1TN3OZ7JiZoTO2YfIxjXnFchSEs52XGfVOs_wdSazPnQ)
- [edit](https://mermaid.live/edit#pako:eNrtl11P01AYx7_Kk3M1ktKs7Vq6akgQJKISiXClMyd1K2wJa2fXxRdCwptXXoDRKy7Gi8YbbyY6MwUh4RM8_UY-52xjAwdI4oWCadKcc3r-T5_z69N_T-dYNsh5zGEzoVvKw9371zI-buNBvIDrWLWgv38QcA1f45bG8QO-x-1EqwvN7vXH4SBW40X8gfu4Q-davNpSAH7CGo18x5oihqqtCH09ojq4Fi_ELw3VSCSOmn1nz3TKwXT01A29RKLd6qk4EuAGLatB-exSXl9kxnWOG1h1WjP7SSYzFqM0KV6KV3CfRHvxK66PDw_xkRtjDm5iQ0887BUNZDQ4EQ1-jQYiGlA0wU9X06ohQRKkllgBW0s-6oPL_Di2sE4L2xFnLtfYIEz7-BXrlGYDvzl8qORm8x6fCopZNzoC36WDnjpo6qCpE0zSalK1TdFqXZpspQijQcXPuVEh8Al56tIjp2XVqVprHBuU8gGlvEsJSnDxqsPvhW521uO3R-7wDu62BnpqoKkB0oBgoQ0Qa00TzdaVMT-rXgm4gk-8RGT2usxF4VjFLbKYTUFRdnh3CXeV9Qm5dBNam5BDUy470C2XyJOq3iQlDjj82J68RX6zEi8d7v6DdpJ3w1wTf7t1Dv4qZUT2Gi9TrYpsa9IN6gqn_Du0-dCTihsWKmU-bFudIj9NDMfE0BYDiWW1T2mjMKnbtySpN7gu4K8RFIogjClejhf_Gvp6h75-Nn39osWvn_ptVUSxvyPNW4dPBOVoJvTKfCIM-E0_8sJSWCh7535RFTiKAe0YQDGgE0O-BqZqqdrxF2GDnqp4qT4LE4sXQd5j_2o8kv9-9CfxX9CP9NMs5ZgdYe2ChgQn1L0dacS2f8uQmEIb_0KOOVFY8RRW9MKiK7psLuMDZFiU94pehjnUzHnTbmU2yrCMP0-ykus_CIJiWxkGlZk8c6bd2TL1KiXaUXkjBZf-KjpTPD_nhcO03YqYk5YRmDPHnjFHT1mqbWmmoZm6ZhlJW2HPmWOl1ZSppXRjIJk2adCaV9gLeUvayg2kTdswLCNlmloyTQIvV4iCcLz5MyP_aeZ_AlWqz8s)

### 1.2 TprKO6, no link
Процесс ТпрКО6 - открытие и ведение счетов ФЛ из двух АС (автоматизированных систем и 4 серверов). Тоже упрощение, и без взаимосвязи систем (АС).
```
const CONFIG = {
Settings: {
DataSetRef: 'DATASET_072v2',   
sysSourceTarget: 'no'    
```

``` mermaid
graph LR;
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.3((Арх3.3)) --> АБС1_ЦФТ:Арх3.3:software((software)) --> АБС1_ЦФТАрх3.3Прикладное_ПО:_ЦФТ-Банк_Платформы_2MCA_DBI:Ри2([Прикладное ПО: ЦФТ-Банк Платформы 2MCA DBI<br>2.9.3<br>АО ЦФТ, 810]) 
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.3((Арх3.3)) --> АБС1_ЦФТ:Арх3.3:software((software)) --> АБС1_ЦФТАрх3.3Сервер_приложений:_Apache_Tomcat:Ри2([Сервер приложений: Apache Tomcat<br>9.0.85<br>Apache Software Foundation, 840]) 
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.3((Арх3.3)) --> АБС1_ЦФТ:Арх3.3:software((software)) --> АБС1_ЦФТАрх3.3Среда_исполнения:_Oracle_JDK_:Ри2([Среда исполнения: Oracle JDK <br>17.0.11<br>Oracle Inc., 840]) 
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.3((Арх3.3)) --> АБС1_ЦФТ:Арх3.3:software((software)) --> АБС1_ЦФТАрх3.3Системное_ПО,_ОС:_Ред_ОС_Сервер:Ри2([Системное ПО, ОС: Ред ОС Сервер<br>10.2<br>ООО «Ред Софт», 810]) 
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.3((Арх3.3)) --> АБС1_ЦФТ:Арх3.3:hardware((hardware)) --> АБС1_ЦФТАрх3.3Оборудование,_сервер:_Aquarius_C86_:Ри2([Оборудование, сервер: Aquarius C86 <br>T1F S28H<br>ГК «Аквариус», 810]) 
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.2((Арх3.2)) --> АБС1_ЦФТ:Арх3.2:software((software)) --> АБС1_ЦФТАрх3.2СУБД:_Postgres_Pro_Enterprise:Ри2([СУБД: Postgres Pro Enterprise<br>15.6.1<br>ООО «Постгрес Про», 810]) 
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.2((Арх3.2)) --> АБС1_ЦФТ:Арх3.2:software((software)) --> АБС1_ЦФТАрх3.2Системное_ПО,_ОС:_Ред_ОС_Сервер:Ри2([Системное ПО, ОС: Ред ОС Сервер<br>10.2<br>ООО «Ред Софт», 810]) 
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.2((Арх3.2)) --> АБС1_ЦФТ:Арх3.2:hardware((hardware)) --> АБС1_ЦФТАрх3.2Оборудование_сервера:_Aquarius_C86_:Ри2([Оборудование сервера: Aquarius C86 <br>T1F D88<br>ГК «Аквариус», 810]) 
ТпрКО6 --> CRM(CRM<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM:Арх3.3((Арх3.3)) --> CRM:Арх3.3:software((software)) --> CRMАрх3.3Прикладное_ПО:_Creatio:Ри2([Прикладное ПО: Creatio<br>8.0.9<br>Creatio / Terrasoft, 840]) 
ТпрКО6 --> CRM(CRM<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM:Арх3.3((Арх3.3)) --> CRM:Арх3.3:software((software)) --> CRMАрх3.3Среда_исполнения:_.NET:Ри2([Среда исполнения: .NET<br>8.0.6<br>Microsoft, 840]) 
ТпрКО6 --> CRM(CRM<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM:Арх3.3((Арх3.3)) --> CRM:Арх3.3:software((software)) --> CRMАрх3.3Веб-сервер:_Internet_Information_Services,_IIS:Ри2([Веб-сервер: Internet Information Services, IIS<br>10.0<br>Microsoft, 840]) 
ТпрКО6 --> CRM(CRM<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM:Арх3.3((Арх3.3)) --> CRM:Арх3.3:software((software)) --> CRMАрх3.3Системное_ПО,_ОС:_Microsoft_Windows_Server_2022:Ри2([Системное ПО, ОС: Microsoft Windows Server 2022<br>Standard<br>Microsoft, 840]) 
ТпрКО6 --> CRM(CRM<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM:Арх3.3((Арх3.3)) --> CRM:Арх3.3:hardware((hardware)) --> CRMАрх3.3Оборудование_сервера:_Dell_PowerEdge:Ри2([Оборудование сервера: Dell PowerEdge<br>R760<br>Dell Inc., 840]) 
ТпрКО6 --> CRM(CRM<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM:Арх3.2((Арх3.2)) --> CRM:Арх3.2:software((software)) --> CRMАрх3.2СУБД:_Microsoft_SQL_Server_2022:Ри2([СУБД: Microsoft SQL Server 2022<br>Enterprise Edition<br>Microsoft, 840]) 
ТпрКО6 --> CRM(CRM<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM:Арх3.2((Арх3.2)) --> CRM:Арх3.2:software((software)) --> CRMАрх3.2Системное_ПО,_ОС:_Microsoft_Windows_Server_2022:Ри2([Системное ПО, ОС: Microsoft Windows Server 2022<br>Datacenter<br>Microsoft, 810]) 
ТпрКО6 --> CRM(CRM<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM:Арх3.2((Арх3.2)) --> CRM:Арх3.2:hardware((hardware)) --> CRMАрх3.2Оборудование_сервера:_Dell_PowerEdge:Ри2([Оборудование сервера: Dell PowerEdge<br>R760xd<br>Dell Inc., 840]) 
```

- [mermaid.live](https://mermaid.live/view#pako:eNrtmFtvG0UUx7_K0T45kr14d31ZL6hSsFNhaKDEkZDAaLR4J7Yle9eM16QlitSk5YmHhstTkZymIF54cQtGhpRU6ieY_UacGe_6ktqugyKStFUUZ2bn_E_O_HzmzLF3lIrnUMVSqsxu1eDGxttllz_iz4I7_AHvZiCRuAb8gH_HjzTCf-W_8EexcArD6TtfsGu8G-zxf_gJf4KvveB-qAD-mPfwyd-8FxePuqGHlRleLX4Q3Am-MVQjFhsNVxZbWm1vy9-2GY3FotFMxUjAD3FbA4znGOP6Q0bcJ_yQd63QMoEyGbF4ikbBfnCPn6DoafAt0dfzq6TwbtHiD_lAj302yxtIb3DKG7zoDYQ3QG-Cn67mVEOCREihOA6mlvx8BV7lt-OI93FjT8QrkXscIKYT_ifvY5gD_pdFVlt2pUbJptes2P4I_IQOZupgqIOhTjDJqUnVTItRuFQKQ4TrXsd1bL_uuYg89cojx231MVt7hA8w5GcY8jEGKMEF9y3yEbMrDUreL3xAxrgjDczUwFADqAHBQssia00Tw3Cl6FbU1wKu4BPsI5mnE8UlTniXH2GJeSgoygmZTOGJtD4ll9UE9ybkMJTLCUzKJfKkqg9JiR94_ltkfIT15l6w__z4CpaTms2cIf5o9BL8XYwIy2twF3NVRNuT1aAfJxj_mDZZ_bJjs3qnTfJmZpzk88QwJYZIDCiW2b6pXYeSbr4nSf3AHwj4BwgFPYjCFNwN9i4NfX1MX19MXz9r8uuYaj_jwo8Wuem1_SqjbXKTeWTN9SlrsXqbTqT50BAiQ0BDGBvKhE6rGVWbTulDfH_E8fhdlKNgD-T9e_K6wH1TWc4P_xkriz6vOEwVFt47Y2mBU-rZtaVgmv-xtOQ31mP4K9T4B3BHP02RzTMq2h54CzYpY7bIxJVIuKhgTy3PT2U0W6bxDqNYoqkOLcV-TOwwcnJjL-5hfqNxmYC8rA9TP1zbXLoBE8YRlowYrNcrzLs6ML7HrTxOTN_SRXEfuNTHwZbHmrJBJyXKvqpXaDtOisXSCM8MOURymJDDSA4oD6tb8gryWnwbjDZDPqm7jrfdltgoI3pS15e8EkY-IPQBQx8gfAgGJd_GT03MuVT05tb1KXrLFvMCbTSwmdmmbM2p0jNXcyGHkVzsfCObkdkmVxZ_JjoXXjOuxKnlpbJtorEbJ1bp4xtzkips7cb5g6anc2fc6sGaUxcn8__MonOjcuFnsGD7doUKmKf5aRfJb5lTqF_sKbzlzDyHSlypsrqjWD7r0LjSpHhxiKmyU3YByopfo01aViwcOnTL7jT8slJ2d1HWst1PPa8ZKZnXqdYUa8tutHHWaTm2Twt1u8rssQl1HcryXsf1FUszpAvF2lFuKZZh6KqZSuX0dErTk-lkNhtXbitWIq3iSiZrZEw9k0unzfRuXPla_ldNTRnZtGYmTcPQskY6mYsrFI-Wx9aH3-7KL3l3_wVLmcsj)
- [edit](https://mermaid.live/edit#pako:eNrtmN9vGkcQx_-V0T1hCa7cwcFxrSK54Ki0cZsaS5VaqtWVWwMS3NHlqJNalmInfepD3B9PqYTjtOpLX0haKlqnjpS_YO8_6uxyxw8HCK6s2k4iy3j3dr7j2Q-zswM7SsVzqGIpVWa3anBj4-2yyx_xZ8Ed_oB3M5BIXAN-wL_jRxrhv_Jf-KNYOIXh9J0v2DXeDfb4P_yEP8HXXnA_VAB_zHv45G_ei4tH3dDDygyvFj8I7gTfpNRULDYariy2tNrelr9tMxqLRaOZipGAH-K2BhjPMcb1h4y4T_gh71qhZQJlMmLxFI2C_eAeP0HR0-Bboq_nV0nh3aLFH_KBHvtsljeQ3uCUN3jRGwhvgN4EP13NqSkJEiGF4jiYWvLzFXiV344j3seNPRGvRO5xgJhO-J-8j2EO-F8WWW3ZlRolm16zYvsj8BM6mKmDoQ6GOsEkpyZV0xCjcKkUhgjXvY7r2H7dcxF5-pVHjtvqY7b2CB9gyM8w5GMMUIIL7lvkI2ZXGpS8X_iAjHFHGpipgaEGUAOChZZF1pomhuFK0a2orwVcwSfYRzJPJ4pLnPAuP8IS81BQlBMymcITaX1KLqsJ7k3IYSiXE5iUS-RJVR-SEj_w_LfI-Ajrzb1g__nxFSwnNZs5Q_zR6CX4uxgRltfgLuaqiLYnq0E_TjD-MW2y-mXHZvVOm-TNzDjJ54lhSgyRGFAss31Tuw4l3XxPkvqBPxDwDxAKehCFKbgb7F0a-vqYvr6Yvn7W5Ncx1X7GhR8tctNr-1VG2-Qm88ia61PWYvU2nUjzoSFEhoCGMDaUCW2oGVWbTulDfH_E8fhdlKNgD-T9e_K6wH1TWc4P_xkriz6vOEwVFt47Y2mBU-rZtaVgmv-xtOQ31mP4K9T4B3BHP02RzTMq2h54CzYpY7bIxJVIuKhgTy3PT2U0W6bxDqNYoqkOLcV-TOwwcnJjL-5hfqNxmYC8rA9TP1zbXLoBE8YRlowYrNcrzLs6ML7HrTxOTN_SRXEfuNTHwZbHmrJBJyXKvqpXaDtOisXSCM8MOURymJDDSA4oD6tb8gryWnwbjDZDPqm7jrfdltgoI3pS15e8EkY-IPQBQx8gfAgGJd_GT03MuVT05tb1KXrLFvMCbTSwmdmmbM2p0jNXcyGHkVzsfCObkdkmVxZ_JjoXXjOuxKnlpbJtorEbJ1bp4xtzkips7cb5g6anc2fc6sGaUxcn8__MonOjcuFnsGD7doUKmKf5aRfJb5lTqF_sKbzlzDyHSlypsrqjWD7r0LjSpHhxiKmyU3YByopfo01aViwcOnTL7jT8slJ2d1HWst1PPa8ZKZnXqdYUa8tutHHWaTm2Twt1u8rssQl1HcryXsf1FcuQHhRrR7mlWKmUrprpdE430pqeNJLZbFy5rVgJQ8WVTDaVMfVMzjBMYzeufC3_qaamU1lDMzUtZ6JE01BB8WR5bH345a78jnf3X4aQyuw)
  
                
### 1.3 TprKO6, link
Процесс ТпрКО6 - с взаимосвязью систем (АС, т.е. CRM --> АБС1), т.е. sysSourceTarget: 'yes' 

``` mermaid
graph LR;
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.3((Арх3.3)) --> АБС1_ЦФТ:Арх3.3:software((software)) --> АБС1_ЦФТАрх3.3Прикладное_ПО:_ЦФТ-Банк_Платформы_2MCA_DBI:Ри2([Прикладное ПО: ЦФТ-Банк Платформы 2MCA DBI<br>2.9.3<br>АО ЦФТ, 810]) 
CRM --> АБС1_ЦФТ
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.3((Арх3.3)) --> АБС1_ЦФТ:Арх3.3:software((software)) --> АБС1_ЦФТАрх3.3Сервер_приложений:_Apache_Tomcat:Ри2([Сервер приложений: Apache Tomcat<br>9.0.85<br>Apache Software Foundation, 840]) 
CRM --> АБС1_ЦФТ
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.3((Арх3.3)) --> АБС1_ЦФТ:Арх3.3:software((software)) --> АБС1_ЦФТАрх3.3Среда_исполнения:_Oracle_JDK_:Ри2([Среда исполнения: Oracle JDK <br>17.0.11<br>Oracle Inc., 840]) 
CRM --> АБС1_ЦФТ
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.3((Арх3.3)) --> АБС1_ЦФТ:Арх3.3:software((software)) --> АБС1_ЦФТАрх3.3Системное_ПО,_ОС:_Ред_ОС_Сервер:Ри2([Системное ПО, ОС: Ред ОС Сервер<br>10.2<br>ООО «Ред Софт», 810]) 
CRM --> АБС1_ЦФТ
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.3((Арх3.3)) --> АБС1_ЦФТ:Арх3.3:hardware((hardware)) --> АБС1_ЦФТАрх3.3Оборудование,_сервер:_Aquarius_C86_:Ри2([Оборудование, сервер: Aquarius C86 <br>T1F S28H<br>ГК «Аквариус», 810]) 
CRM --> АБС1_ЦФТ
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.2((Арх3.2)) --> АБС1_ЦФТ:Арх3.2:software((software)) --> АБС1_ЦФТАрх3.2СУБД:_Postgres_Pro_Enterprise:Ри2([СУБД: Postgres Pro Enterprise<br>15.6.1<br>ООО «Постгрес Про», 810]) 
CRM --> АБС1_ЦФТ
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.2((Арх3.2)) --> АБС1_ЦФТ:Арх3.2:software((software)) --> АБС1_ЦФТАрх3.2Системное_ПО,_ОС:_Ред_ОС_Сервер:Ри2([Системное ПО, ОС: Ред ОС Сервер<br>10.2<br>ООО «Ред Софт», 810]) 
CRM --> АБС1_ЦФТ
ТпрКО6 --> АБС1_ЦФТ(АБС1 ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС1_ЦФТ:Арх3.2((Арх3.2)) --> АБС1_ЦФТ:Арх3.2:hardware((hardware)) --> АБС1_ЦФТАрх3.2Оборудование_сервера:_Aquarius_C86_:Ри2([Оборудование сервера: Aquarius C86 <br>T1F D88<br>ГК «Аквариус», 810]) 
CRM --> АБС1_ЦФТ
ТпрКО6 --> CRM(CRM<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM:Арх3.3((Арх3.3)) --> CRM:Арх3.3:software((software)) --> CRMАрх3.3Прикладное_ПО:_Creatio:Ри2([Прикладное ПО: Creatio<br>8.0.9<br>Creatio / Terrasoft, 840]) 
CRM --> АБС1_ЦФТ
ТпрКО6 --> CRM(CRM<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM:Арх3.3((Арх3.3)) --> CRM:Арх3.3:software((software)) --> CRMАрх3.3Среда_исполнения:_.NET:Ри2([Среда исполнения: .NET<br>8.0.6<br>Microsoft, 840]) 
CRM --> АБС1_ЦФТ
ТпрКО6 --> CRM(CRM<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM:Арх3.3((Арх3.3)) --> CRM:Арх3.3:software((software)) --> CRMАрх3.3Веб-сервер:_Internet_Information_Services,_IIS:Ри2([Веб-сервер: Internet Information Services, IIS<br>10.0<br>Microsoft, 840]) 
CRM --> АБС1_ЦФТ
ТпрКО6 --> CRM(CRM<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM:Арх3.3((Арх3.3)) --> CRM:Арх3.3:software((software)) --> CRMАрх3.3Системное_ПО,_ОС:_Microsoft_Windows_Server_2022:Ри2([Системное ПО, ОС: Microsoft Windows Server 2022<br>Standard<br>Microsoft, 840]) 
CRM --> АБС1_ЦФТ
ТпрКО6 --> CRM(CRM<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM:Арх3.3((Арх3.3)) --> CRM:Арх3.3:hardware((hardware)) --> CRMАрх3.3Оборудование_сервера:_Dell_PowerEdge:Ри2([Оборудование сервера: Dell PowerEdge<br>R760<br>Dell Inc., 840]) 
CRM --> АБС1_ЦФТ
ТпрКО6 --> CRM(CRM<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM:Арх3.2((Арх3.2)) --> CRM:Арх3.2:software((software)) --> CRMАрх3.2СУБД:_Microsoft_SQL_Server_2022:Ри2([СУБД: Microsoft SQL Server 2022<br>Enterprise Edition<br>Microsoft, 840]) 
CRM --> АБС1_ЦФТ
ТпрКО6 --> CRM(CRM<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM:Арх3.2((Арх3.2)) --> CRM:Арх3.2:software((software)) --> CRMАрх3.2Системное_ПО,_ОС:_Microsoft_Windows_Server_2022:Ри2([Системное ПО, ОС: Microsoft Windows Server 2022<br>Datacenter<br>Microsoft, 810]) 
CRM --> АБС1_ЦФТ
ТпрКО6 --> CRM(CRM<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM:Арх3.2((Арх3.2)) --> CRM:Арх3.2:hardware((hardware)) --> CRMАрх3.2Оборудование_сервера:_Dell_PowerEdge:Ри2([Оборудование сервера: Dell PowerEdge<br>R760xd<br>Dell Inc., 840]) 
CRM --> АБС1_ЦФТ
```

- [mermaid.live](https://mermaid.live/view#pako:eNrtWFtvG0UU_itH--RIzuJd39YLqhTsVBgaKHEkJDAaLd6JbcneNeM1aYkiNWl54qHh8lQkpymIF17cgpEhJZX6C2b_EWdmd32rndooqGlSRbFmds53fM53brPeVSquTRVTqTKrVYMbm2-XHf6IP_Pv8Ae8m4HV1WvAD_l3_Fgj_Ff-C38UC7cQbN_5gl3jXX-f_8NP-RP87Pn3QwTwx7yHT_7mvbh41A01rMzQavJD_47_TVJNxmLD5crZkmbb3fZ2LEZjsWg1EzEE8CN0a4D2nKBdf0iL-4Qf8a4ZSq4iTFosnqKQf-Df46cIeup_S_SN_BopvFs0-UM-0GOfzdIGUhtMaYMXtYHQBqhN8KerOTUpiUSSQnAcDC3x-QqUnfzmxgynLnOYjnkfHXsiPon0cYD0nfI_eR_NHPC_TLLWsio1SrbcZsXyhgEZw8FMHAQ4CHCCk5yaUI20WIVHpdBEuO52HNvy6q6DoUhd2VCgW33M7h7hAzT5GZp8ggZKQv37JvmIWZUGJe8XPiCjMEQYmImBAAOIAcGFlsUYaJpYhidFp6JeadIFb_4BMvZ0rEnFCe_yY2xVDwW7ckPGU36sDKbgsiuhbwIOAVxuYBwuQ5FQ9YAp8QfPf4uEj7Fv3fMPnp9corZUs5gdhCVavSQsXbQI27d_F3NbWNuTXaUfJ2j_KApk7cuOxeqdNskbmVFRzAPDBBgiMCBYVseWdh1KuvGeZOoH_kAE5RBJQQ2iwfl3_f0LHxV9FBX97KjoyxaLjqn5Mx78aJKbbturMtomN5lL1h2Pshart-lYWQSCEAkCCsJIUBZAWs2o2mQJHGHcRDn9Ltqavw9y7p9eddLfdKj_PyxLdih9XpOZaFC8t2SLgin07B5VMIxzblEoF8N_oVVAUOinCcbzjIrrGbwFW5QxS2TuSgQ8ayBMHM9PfRRb5MUhtGKBl4JQUvhj4I0nJx170YflLz4XiaiX3RfVD9e3Fr4oCuGIroxYbNQrzH39SfoeXXy8OnlrKIo55FAPF9sua8oXD1Ki7Kt6hbbjpFgsDWmbAYcIDmNwGMIB4WH3TFwiHs-eQkMnySd1x3Z32pJOyoie0PUFR9FQB4Q6INABQofgoORZ-JbI7NeC1bnzZILVRYdIgTYaeOnaoWzdrtKlp4iAwxAuPN_MZmR2ypP_9g54LjzOGNETxwtl59jFdJSIpY9vzEnC8Go6yjcUnc610VUV1u26qPCLkHXnxtYrr-WC5VkVKkie5lW7iLwuUs36q63mW_ZS9azElSqr24rpsQ6NK02Kg0xsld2yA1BWvBpt0rJi4tKm21an4ZWVsrOHsJblfOq6zQjJ3E61ppjbVqONu07LtjxaqFtVZo1EqGNTlnc7jqeYaalBMXeVW7jJZdSMjjHPadkUfsaV24qJk9MwtFw2rSW0ZDKTS6b24srX8is1VU_quXQiY2RTCSOVyibjCsX6dNlG8NO6_IV971_htYS_)
- [edit](https://mermaid.live/edit#pako:eNrtWFtvG0UU_itH--RI9rIXX9YLqhTsVBgaKHEkJDAaLd6JbcneNeM1aYkiNWl54qHh8lQkpymIF17cgpEhJZX6C2b_EWfG61tqpzYKappUUayZnfMdn_Od26x3lLLvUsVWKsxpVuHGxtsljz_iz8I7_AHvpCGRuAb8gH_Hj3TCf-W_8EexaAuD7TtfsGu8E-7xf_gJf4Kf3fB-hAD-mHfxyd-8GxePOpGGlRlabX4Q3gm_MVUzFhstV86WtFv-VrDtMBqLDVczESMAP0S3-mjPMdr1h7S4R_gh79iRZAJh0mLxFIXC_fAeP0HQ0_BbYqznVkn-3YLNH_K-EftsljaQ2uCUNnhRGwhtgNoEf4aaVU1JJJIUgeNg6drnK1DychvrM5y6zGE64j107In4JNLHPtJ3wv_kPTSzz_-yyWrTKVcp2fQbZScYBWQCBzNxMMDBACc4yaqaaqXEKjoqRibCdb_tuU5Q8z0MRfLKhgLd6mF2dwnvo8nP0ORjNFASGt63yUfMKdcpeT__ARmHYYiBmRgYYAAxILjQMxgDXRfL6KTgldUrTbrgLdxHxp5ONKk44R1-hK3qoWBXbshkyk-UwSm47Erom4DDAC43MAmXodBUY8CU-IPnvw2Fj7Bv3Qv3nx9forZUdZg7CMtw9ZKwdNAibN_hXcxtYW1XdpVenKD94yiQ1S_bDqu1WyRnpcdFMQ8MU2AYggHBsjo29etQNKz3JFM_8AciKAdICmoQDS68G-5d-KgY46gYZ0fFWLZYDEzNn_HgR5vc9FtBhdEWucl8suYFlDVZrUUnymIgCENBQEEYC8oCSKlpVZ8ugUOMmyin30VbC_dAzv2Tq076mw71_4dlyQ5lzGsyUw2Kd5dsUXAKPbtH5S3rnFsUysXwX2gVEBT6aYrxHKPiegZvwSZlzBGZuzIEnjUQpo7npz6KLfLiEFmxwEtBJCn8sfDGk5WOvejD8hefi0TUy-6L6odrmwtfFIXwkK60WKzXysx__Un6Hl18nJi-NRTEHPJogIstnzXkiwcpUvZVrUxbcVIoFEe0zYDDEA4TcBjBAeFR99QuEY9nT6GRk-STmuf62y1JJ2XE0AxjwVE00gGRDhjoAKFDcFAMHHxLZO5rwerceTLF6qJDJE_rdbx0bVO25lbo0lNEwGEEF55vZNIyO-XJf3sHPBceZ4zoqeOFsnPiYjpOxOLHN-YkYXQ1Hecbip7OtfFVFdbcmqjwi5B158bWK6_lvBM4ZSpIPs2rfhF5XaSajVdbzbfcpepZiSsVVnMVO2BtGlcaFAeZ2Co7JQ-gpARV2qAlxcalS7ecdj0oKSVvF2FNx_vU9xtDJPPblapibzn1Fu7aTdcJaL7mVJgzFqGeS1nOb3uBYqekBsXeUW4ptmkk1ZSh6ZapmXpaz5p4eluxE6alZrR0Nqtp2ayJjljp3bjytfxWXU2amZSeyaQN3UrqSTOuUKxQn60PflyXv7Hv_gvecYUb)

### 1.4 Comment
Получается много избыточных линий (соединений): с одной стороны "одна арх-запись" = один "сквозной путь" (end-to-end), т.е. можно выделив строку подсветить весь набор стрелок к ней. Первый end - это ТП, а послений end - "деталь" от ИТ-продукта. С другой стороны - "паутина" подчеркивает насколько избыточен формат 18-МР (ф072).  
Если Одна АС поддерживает 10 ТП (тех процессов) и в этой АС есть 20 ИТ-продуктов, то нужно будет сформировать 200 строк (арх-строк)! Зачем?     
Замечания к формату 18-МР (ф072):
- в логическом формате "арх-записи" убрать дублирование
- в физическом формате "арх-записи" заменить "велосипед" из CSV (Comma-Separated Value) c разделителем "|" на какой-либо более "человеческий" формат типа JSON \ YAML, а еще лучше RDF. 

## 2 TprKO6 + TprKO3 
Добавим простой вариант **ТПрКО3** Технологический процесс, обеспечивающий размещение привлеченных во вклады денежных средств физических и (или) юридических лиц от своего имени и за свой счет  
в виде кредитного конвеера ЮЛ и CRM ЮЛ
### 2.1 TprKO6 + TprKO3, no link
TprKO6 = CRM ФЛ + АБС
TprKO3 (в части ЮЛ) = кредитный конвеер ЮЛ + CRM ЮЛ + АБС
``` mermaid
graph LR;
ТпрКО6 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.3((Арх3.3)) --> АБС_ЦФТ:Арх3.3:software((software)) --> АБС_ЦФТАрх3.3Прикладное_ПО:_ЦФТ-Банк_Платформы_2MCA_DBI:Ри2([Прикладное ПО: ЦФТ-Банк Платформы 2MCA DBI<br>2.9.3<br>АО ЦФТ, 810]) 
ТпрКО6 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.3((Арх3.3)) --> АБС_ЦФТ:Арх3.3:software((software)) --> АБС_ЦФТАрх3.3Сервер_приложений:_Apache_Tomcat:Ри2([Сервер приложений: Apache Tomcat<br>9.0.85<br>Apache Software Foundation, 840]) 
ТпрКО6 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.3((Арх3.3)) --> АБС_ЦФТ:Арх3.3:software((software)) --> АБС_ЦФТАрх3.3Среда_исполнения:_Oracle_JDK_:Ри2([Среда исполнения: Oracle JDK <br>17.0.11<br>Oracle Inc., 840]) 
ТпрКО6 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.3((Арх3.3)) --> АБС_ЦФТ:Арх3.3:software((software)) --> АБС_ЦФТАрх3.3Системное_ПО,_ОС:_Ред_ОС_Сервер:Ри2([Системное ПО, ОС: Ред ОС Сервер<br>10.2<br>ООО «Ред Софт», 810]) 
ТпрКО6 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.3((Арх3.3)) --> АБС_ЦФТ:Арх3.3:hardware((hardware)) --> АБС_ЦФТАрх3.3Оборудование,_сервер:_Aquarius_C86_:Ри2([Оборудование, сервер: Aquarius C86 <br>T1F S28H<br>ГК «Аквариус», 810]) 
ТпрКО6 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.2((Арх3.2)) --> АБС_ЦФТ:Арх3.2:software((software)) --> АБС_ЦФТАрх3.2СУБД:_Postgres_Pro_Enterprise:Ри2([СУБД: Postgres Pro Enterprise<br>15.6.1<br>ООО «Постгрес Про», 810]) 
ТпрКО6 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.2((Арх3.2)) --> АБС_ЦФТ:Арх3.2:software((software)) --> АБС_ЦФТАрх3.2Системное_ПО,_ОС:_Ред_ОС_Сервер:Ри2([Системное ПО, ОС: Ред ОС Сервер<br>10.2<br>ООО «Ред Софт», 810]) 
ТпрКО6 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.2((Арх3.2)) --> АБС_ЦФТ:Арх3.2:hardware((hardware)) --> АБС_ЦФТАрх3.2Оборудование_сервера:_Aquarius_C86_:Ри2([Оборудование сервера: Aquarius C86 <br>T1F D88<br>ГК «Аквариус», 810]) 
ТпрКО6 --> CRM_ФЛ(CRM ФЛ<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM_ФЛ:Арх3.3((Арх3.3)) --> CRM_ФЛ:Арх3.3:software((software)) --> CRM_ФЛАрх3.3Прикладное_ПО:_Creatio:Ри2([Прикладное ПО: Creatio<br>8.0.9<br>Creatio / Terrasoft, 840]) 
ТпрКО6 --> CRM_ФЛ(CRM ФЛ<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM_ФЛ:Арх3.3((Арх3.3)) --> CRM_ФЛ:Арх3.3:software((software)) --> CRM_ФЛАрх3.3Среда_исполнения:_.NET:Ри2([Среда исполнения: .NET<br>8.0.6<br>Microsoft, 840]) 
ТпрКО6 --> CRM_ФЛ(CRM ФЛ<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM_ФЛ:Арх3.3((Арх3.3)) --> CRM_ФЛ:Арх3.3:software((software)) --> CRM_ФЛАрх3.3Веб-сервер:_Internet_Information_Services,_IIS:Ри2([Веб-сервер: Internet Information Services, IIS<br>10.0<br>Microsoft, 840]) 
ТпрКО6 --> CRM_ФЛ(CRM ФЛ<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM_ФЛ:Арх3.3((Арх3.3)) --> CRM_ФЛ:Арх3.3:software((software)) --> CRM_ФЛАрх3.3Системное_ПО,_ОС:_Microsoft_Windows_Server_2022:Ри2([Системное ПО, ОС: Microsoft Windows Server 2022<br>Standard<br>Microsoft, 840]) 
ТпрКО6 --> CRM_ФЛ(CRM ФЛ<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM_ФЛ:Арх3.3((Арх3.3)) --> CRM_ФЛ:Арх3.3:hardware((hardware)) --> CRM_ФЛАрх3.3Оборудование_сервера:_Dell_PowerEdge:Ри2([Оборудование сервера: Dell PowerEdge<br>R760<br>Dell Inc., 840]) 
ТпрКО6 --> CRM_ФЛ(CRM ФЛ<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM_ФЛ:Арх3.2((Арх3.2)) --> CRM_ФЛ:Арх3.2:software((software)) --> CRM_ФЛАрх3.2СУБД:_Microsoft_SQL_Server_2022:Ри2([СУБД: Microsoft SQL Server 2022<br>Enterprise Edition<br>Microsoft, 840]) 
ТпрКО6 --> CRM_ФЛ(CRM ФЛ<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM_ФЛ:Арх3.2((Арх3.2)) --> CRM_ФЛ:Арх3.2:software((software)) --> CRM_ФЛАрх3.2Системное_ПО,_ОС:_Microsoft_Windows_Server_2022:Ри2([Системное ПО, ОС: Microsoft Windows Server 2022<br>Datacenter<br>Microsoft, 810]) 
ТпрКО6 --> CRM_ФЛ(CRM ФЛ<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM_ФЛ:Арх3.2((Арх3.2)) --> CRM_ФЛ:Арх3.2:hardware((hardware)) --> CRM_ФЛАрх3.2Оборудование_сервера:_Dell_PowerEdge:Ри2([Оборудование сервера: Dell PowerEdge<br>R760xd<br>Dell Inc., 840]) 
ТпрКО3 --> CRM_ЮЛ(CRM ЮЛ<br>CRM ЮЛ банка, Creatio / Terrasoft) --> CRM_ЮЛ:Арх3.3((Арх3.3)) --> CRM_ЮЛ:Арх3.3:software((software)) --> CRM_ЮЛАрх3.3Прикладное_ПО:_Creatio:Ри2([Прикладное ПО: Creatio<br>8.0.9<br>Creatio / Terrasoft, 840]) 
ТпрКО3 --> CRM_ЮЛ(CRM ЮЛ<br>CRM ЮЛ банка, Creatio / Terrasoft) --> CRM_ЮЛ:Арх3.3((Арх3.3)) --> CRM_ЮЛ:Арх3.3:software((software)) --> CRM_ЮЛАрх3.3Среда_исполнения:_.NET:Ри2([Среда исполнения: .NET<br>8.0.6<br>Microsoft, 840]) 
ТпрКО3 --> CRM_ЮЛ(CRM ЮЛ<br>CRM ЮЛ банка, Creatio / Terrasoft) --> CRM_ЮЛ:Арх3.3((Арх3.3)) --> CRM_ЮЛ:Арх3.3:software((software)) --> CRM_ЮЛАрх3.3Веб-сервер:_Internet_Information_Services,_IIS:Ри2([Веб-сервер: Internet Information Services, IIS<br>10.0<br>Microsoft, 840]) 
ТпрКО3 --> CRM_ЮЛ(CRM ЮЛ<br>CRM ЮЛ банка, Creatio / Terrasoft) --> CRM_ЮЛ:Арх3.3((Арх3.3)) --> CRM_ЮЛ:Арх3.3:software((software)) --> CRM_ЮЛАрх3.3Системное_ПО,_ОС:_Microsoft_Windows_Server_2022:Ри2([Системное ПО, ОС: Microsoft Windows Server 2022<br>Standard<br>Microsoft, 840]) 
ТпрКО3 --> CRM_ЮЛ(CRM ЮЛ<br>CRM ЮЛ банка, Creatio / Terrasoft) --> CRM_ЮЛ:Арх3.3((Арх3.3)) --> CRM_ЮЛ:Арх3.3:hardware((hardware)) --> CRM_ЮЛАрх3.3Оборудование_сервера:_Dell_PowerEdge:Ри2([Оборудование сервера: Dell PowerEdge<br>R760<br>Dell Inc., 840]) 
ТпрКО3 --> CRM_ЮЛ(CRM ЮЛ<br>CRM ЮЛ банка, Creatio / Terrasoft) --> CRM_ЮЛ:Арх3.2((Арх3.2)) --> CRM_ЮЛ:Арх3.2:software((software)) --> CRM_ЮЛАрх3.2СУБД:_Microsoft_SQL_Server_2022:Ри2([СУБД: Microsoft SQL Server 2022<br>Enterprise Edition<br>Microsoft, 840]) 
ТпрКО3 --> CRM_ЮЛ(CRM ЮЛ<br>CRM ЮЛ банка, Creatio / Terrasoft) --> CRM_ЮЛ:Арх3.2((Арх3.2)) --> CRM_ЮЛ:Арх3.2:software((software)) --> CRM_ЮЛАрх3.2Системное_ПО,_ОС:_Microsoft_Windows_Server_2022:Ри2([Системное ПО, ОС: Microsoft Windows Server 2022<br>Datacenter<br>Microsoft, 810]) 
ТпрКО3 --> CRM_ЮЛ(CRM ЮЛ<br>CRM ЮЛ банка, Creatio / Terrasoft) --> CRM_ЮЛ:Арх3.2((Арх3.2)) --> CRM_ЮЛ:Арх3.2:hardware((hardware)) --> CRM_ЮЛАрх3.2Оборудование_сервера:_Dell_PowerEdge:Ри2([Оборудование сервера: Dell PowerEdge<br>R760xd<br>Dell Inc., 840]) 
ТпрКО3 --> Кредиты_ЮЛ(Кредиты ЮЛ<br>Кредитный конвейер ЮЛ банка, Интегратор 1) --> Кредиты_ЮЛ:Арх3.3((Арх3.3)) --> Кредиты_ЮЛ:Арх3.3:software((software)) --> Кредиты_ЮЛАрх3.3Прикладное_ПО:_ELMA_BPM_Suite_Enterprise:Ри2([Прикладное ПО: ELMA BPM Suite Enterprise<br>4.2.10.55<br>ELMA, 810]) 
ТпрКО3 --> Кредиты_ЮЛ(Кредиты ЮЛ<br>Кредитный конвейер ЮЛ банка, Интегратор 1) --> Кредиты_ЮЛ:Арх3.3((Арх3.3)) --> Кредиты_ЮЛ:Арх3.3:software((software)) --> Кредиты_ЮЛАрх3.3Среда_исполнения:_.NET_Core_Runtime:Ри2([Среда исполнения: .NET Core Runtime<br>8.0.6<br>Microsoft, 840]) 
ТпрКО3 --> Кредиты_ЮЛ(Кредиты ЮЛ<br>Кредитный конвейер ЮЛ банка, Интегратор 1) --> Кредиты_ЮЛ:Арх3.3((Арх3.3)) --> Кредиты_ЮЛ:Арх3.3:software((software)) --> Кредиты_ЮЛАрх3.3Веб-сервер:_Internet_Information_Services,_IIS:Ри2([Веб-сервер: Internet Information Services, IIS<br>10.0<br>Microsoft, 840]) 
ТпрКО3 --> Кредиты_ЮЛ(Кредиты ЮЛ<br>Кредитный конвейер ЮЛ банка, Интегратор 1) --> Кредиты_ЮЛ:Арх3.3((Арх3.3)) --> Кредиты_ЮЛ:Арх3.3:software((software)) --> Кредиты_ЮЛАрх3.3Системное_ПО,_ОС:_Microsoft_Windows_Server_2022:Ри2([Системное ПО, ОС: Microsoft Windows Server 2022<br>Standard<br>Microsoft, 840]) 
ТпрКО3 --> Кредиты_ЮЛ(Кредиты ЮЛ<br>Кредитный конвейер ЮЛ банка, Интегратор 1) --> Кредиты_ЮЛ:Арх3.3((Арх3.3)) --> Кредиты_ЮЛ:Арх3.3:hardware((hardware)) --> Кредиты_ЮЛАрх3.3Оборудование_сервера:_Dell_PowerEdge:Ри2([Оборудование сервера: Dell PowerEdge<br>R760<br>Dell Inc., 840]) 
ТпрКО3 --> Кредиты_ЮЛ(Кредиты ЮЛ<br>Кредитный конвейер ЮЛ банка, Интегратор 1) --> Кредиты_ЮЛ:Арх3.2((Арх3.2)) --> Кредиты_ЮЛ:Арх3.2:software((software)) --> Кредиты_ЮЛАрх3.2СУБД:_Microsoft_SQL_Server_2022:Ри2([СУБД: Microsoft SQL Server 2022<br>Enterprise Edition<br>Microsoft, 840]) 
ТпрКО3 --> Кредиты_ЮЛ(Кредиты ЮЛ<br>Кредитный конвейер ЮЛ банка, Интегратор 1) --> Кредиты_ЮЛ:Арх3.2((Арх3.2)) --> Кредиты_ЮЛ:Арх3.2:software((software)) --> Кредиты_ЮЛАрх3.2Системное_ПО,_ОС:_Microsoft_Windows_Server_2022:Ри2([Системное ПО, ОС: Microsoft Windows Server 2022<br>Datacenter<br>Microsoft, 810]) 
ТпрКО3 --> Кредиты_ЮЛ(Кредиты ЮЛ<br>Кредитный конвейер ЮЛ банка, Интегратор 1) --> Кредиты_ЮЛ:Арх3.2((Арх3.2)) --> Кредиты_ЮЛ:Арх3.2:hardware((hardware)) --> Кредиты_ЮЛАрх3.2Оборудование_сервера:_Dell_PowerEdge:Ри2([Оборудование сервера: Dell PowerEdge<br>R760xd<br>Dell Inc., 840]) 
ТпрКО3 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.3((Арх3.3)) --> АБС_ЦФТ:Арх3.3:software((software)) --> АБС_ЦФТАрх3.3Прикладное_ПО:_ЦФТ-Банк_Платформы_2MCA_DBI:Ри2([Прикладное ПО: ЦФТ-Банк Платформы 2MCA DBI<br>2.9.3<br>АО ЦФТ, 810]) 
ТпрКО3 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.3((Арх3.3)) --> АБС_ЦФТ:Арх3.3:software((software)) --> АБС_ЦФТАрх3.3Сервер_приложений:_Apache_Tomcat:Ри2([Сервер приложений: Apache Tomcat<br>9.0.85<br>Apache Software Foundation, 840]) 
ТпрКО3 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.3((Арх3.3)) --> АБС_ЦФТ:Арх3.3:software((software)) --> АБС_ЦФТАрх3.3Среда_исполнения:_Oracle_JDK_:Ри2([Среда исполнения: Oracle JDK <br>17.0.11<br>Oracle Inc., 840]) 
ТпрКО3 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.3((Арх3.3)) --> АБС_ЦФТ:Арх3.3:software((software)) --> АБС_ЦФТАрх3.3Системное_ПО,_ОС:_Ред_ОС_Сервер:Ри2([Системное ПО, ОС: Ред ОС Сервер<br>10.2<br>ООО «Ред Софт», 810]) 
ТпрКО3 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.3((Арх3.3)) --> АБС_ЦФТ:Арх3.3:hardware((hardware)) --> АБС_ЦФТАрх3.3Оборудование,_сервер:_Aquarius_C86_:Ри2([Оборудование, сервер: Aquarius C86 <br>T1F S28H<br>ГК «Аквариус», 810]) 
ТпрКО3 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.2((Арх3.2)) --> АБС_ЦФТ:Арх3.2:software((software)) --> АБС_ЦФТАрх3.2СУБД:_Postgres_Pro_Enterprise:Ри2([СУБД: Postgres Pro Enterprise<br>15.6.1<br>ООО «Постгрес Про», 810]) 
ТпрКО3 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.2((Арх3.2)) --> АБС_ЦФТ:Арх3.2:software((software)) --> АБС_ЦФТАрх3.2Системное_ПО,_ОС:_Ред_ОС_Сервер:Ри2([Системное ПО, ОС: Ред ОС Сервер<br>10.2<br>ООО «Ред Софт», 810]) 
ТпрКО3 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.2((Арх3.2)) --> АБС_ЦФТ:Арх3.2:hardware((hardware)) --> АБС_ЦФТАрх3.2Оборудование_сервера:_Aquarius_C86_:Ри2([Оборудование сервера: Aquarius C86 <br>T1F D88<br>ГК «Аквариус», 810]) 
```
- [mermaid.live](https://mermaid.live/view#pako:eNrtW1tPG0cU_itH-2Qks7V38W1bRSJAVFpoKUaq1FKNtvYAlrCXjtclLUIKJH3iIfTyUFEJQlr1pZLlpKWCJiFSfsHsP-qZ2V3f7dio1F7bsmTNrs93fOabM2e-8Y73lIyVpYqhbDJzZwuWVt9dL_Cn_LXzgJ_w0zhMT98Bfsy_5-eE_85_409D7hW4V-99ye7wU-eAv-LX_Dm-V5zH4Fs84xW88w-vhMWtU8_BVKtPgx87D5zvdFUPharNqa6GRtHasHdNRkMhv9UOULXnZ9ijSwzmBQb1lwz3gvAzfmp4ltOIkuGKu2jkHDqP-DWCXjpHRFuemyXzdxcN_oRfaqHP23kD6Q2avEGrNxDeAL0J8jQ1peqSRWTIA4chGY18MQUjOhLn_AL79Fy8E9m9S2Tomv_NLzDGS35lkNkdM7NFyZqVz5h2lfM6HLTFgYsDFycISakRNRkTLe-jtBch3LNKhaxp56wCsj0zymxjjy4wRyuEX2K8rzHeFxid5Mx5bJCPmZnZpuSD-Q9JjWkfA20x4GIAMSCIiCaQ5mhUNL1PFgsZddR5FdQ4h0jKy7pqEib8lJ9jTXkiCJQXpD5x65K5CS7LB3ZMwMGFywuoh0u2I6rm0iRe8OYP3_gcC8wj5_DNi4DVjy2TZV3m_VZ35k8xHCylzkPMUBFqRU7_izDB4GtEk9mvSibLlYpkLhmvpXYnMDSAwQcDgmWOr0XvQVpLvi9p-pGfCN6PkRH0ICqR89A5GA7itRrxWlfitT5TXsME-xXv_2SQFatobzJaJCvMIgsFm7IdlivSuuR2DcE3BDSEmqFM45gaV6ONiXyGQyMmxZ-i_jgHIJfZ6zHgdVJK_hvm-yslWqdq0FBJeKXPWgJN6PbFZD6ZvGEtmVtdJtiNX0LYANEQfvx2A8FzjAqJA-_AGmXMFNk41eCiW7lutemc2L5tL3LbC6oHKe1Ziu4lUWGkZD9bu9RZaASCqbcJNPWjhbWelZkw9vmKi8ZyLsOsEWDpB-zjs-nGFX5RLCgFamNjw2J5qeZJmrKvcxlaDJPFxXSVtzZw8OFQB4cqHBDu1cjIKBHZfbGp9pJ8mitkrd2i5JMyokU0rccVp-oDPB_g-gDhQ1CStk3ce7Hs0NPacTlppbXXlWSebm-jftqlbCG7SfteSgQcqnBBxGoiLvNTftJ933UbRLZZnFttes_POpFZS8X0J0sd0tCTmbWMQ9PmbKvJTljI5sQkH2De3QJdA5_O86ZtZqhguZnY6LAR2_OE1gY7oe9n3zql9VrcZZ_Kch2V5b6oLPdQG8t9LDnlIdKCAWJqgFowQCwNtxYMUroFSAsOmtbuS0c5OFrw9ojstAaX-xA35WHTgoGiK0hacNDE9jyhg6IF-YknCC6dQ-fIZbXxXpXg-tv8lXPErwBJvsa4MBh-5T5ibR4A_jOaiswQP89XsIV9guhUp-_u-iiom3mX389bYb2ozIWl5Vlyd2WZpEs5m7Z7YNFZdwosIBYktukZxoyqqagJYvIJs7DsnOdjPji9CFsyZzFKVksFO5enfalcEEjwkP1K3jEfmSCI6XGfPIGT6SMzYJ0fKHYbsCBsAIZ1iNo97e1mfqM5NUxbi7EfiOBtWkZmyG5S3gKzHZqcWh74qWV9cmr5fzy1rE9OLd_KqWV9cmp5QEcN9cmp5cGcWtYnp5Zv5dSyPjm1PCalZLxPLSthZZPlsophsxINK3nK8qa4VPbWCwDrir1F83RdMbCZpRtmadteV9YL-wjbMQufWVbeRzKrtLmlGBvmdhGvSjuofuh8ztxkZs2EFrKUzaE0shUjMSNdKMaecl8xdD2upnQ9ouuxVCSZiuph5RvFmE7EZtQE3p5JJXFHocVj-2HlW_mlmhpJzKQSsWhKQx0QjWiIoLidt9iy-zdJ-W_J_X8Bp4deSQ)
- [edit](https://mermaid.live/edit#pako:eNrtW1tPG0cU_itH-2Qks7V38YVtFYlgotJCSzFSpZZqtLUHsIS9dLwuaRFSIOkTD6GXh4pKENKqL5UsJy0VNAmR8gtm_1HPzO76bsdGpfbaliVrdn2-4zPfnDnzjXe8p2SsLFUMZZOZO1uwtPrueoE_5a-dB_yEn8ZhevoO8GP-PT8n_Hf-G38acq_AvXrvS3aHnzoH_BW_5s_xveI8Bt_iGa_gnX94JSxunXoOplp9GvzYeeB8p6t6KFRtTnU1NIrWhr1rMhoK-a12gKo9P8MeXWIwLzCov2S4F4Sf8VPDs5xGlAxX3EUj59B5xK8R9NI5Itry_BxJ3V00-BN-qYU-b-cNpDdo8gat3kB4A_QmyNPUWVWXLCJDHjgMyWjkiykY0ZE45xfYp-fincjuXSJD1_xvfoExXvIrg8ztmJktStasfMa0q5zX4aAtDlwcuDhByKwaUZMx0fI-SnsRwj2rVMiads4qINszo8w29ugCc7RC-CXG-xrjfYHRSc6cxwb5mJmZbUo-SH1Iakz7GGiLARcDiAFBRDSBNEejoul9sljIqKPOq6DGOURSXtZVkzDhp_wca8oTQaC8IPWJW5fMTXBZPrBjAg4uXF5APVyyHVE1lybxgjd_-MbnWGAeOYdvXgSsfmyZLOsy77e6M3-K4WApdR5ihopQK3L6X4QJBl8jmsx9VTJZrlQk88l4LbU7gaEBDD4YECxzfC16D9Ja8n1J04_8RPB-jIygB1GJnIfOwXAQr9WI17oSr_WZ8hom2K94_yeDrFhFe5PRIllhFlko2JTtsFyR1iW3awi-IaAh1AxlGsfUuBptTOQzHBoxKf4U9cc5ALnMXo8Br5NS8t8w318p0TpVg4ZKwit91hJoQrcvJqlk8oa1ZH51mWA3fglhA0RD-PHbDQTPMyokDrwDa5QxU2TjVIOLbuW61aZzYvu2vchtL6gepLRnKbqXRIUxK_vZ2qXOQiMQTL1NoKkfLaz1rMyEsc9XXDSWcxlmjQBLP2Afn003rvCLYkEpUBsbGxbLSzVP0pR9ncvQYpgsLqarvLWBgw-HOjhU4YBwr0ZGRonI7otNtZfk01wha-0WJZ-UES2iaT2uOFUf4PkA1wcIH4KStG3i3otlh57WjstJK629riQpur2N-mmXsoXsJu17KRFwqMIFEauJuMxP-Un3fddtENlmcW616T0_60RmLRXTnyx1SENPZtYyDk2bs60mO2EhmxOTfIB5dwt0DXw6p0zbzFDBcjOx0WEjtucJrQ12Qt_PvnVK67W4yz6V5Toqy31RWe6hNpb7WHLKQ6QFA8TUALVggFgabi0YpHQLkBYcNK3dl45ycLTg7RHZaQ0u9yFuysOmBQNFV5C04KCJ7XlCB0UL8hNPEFw6h86Ry2rjvSrB9bf5K-eIXwGSfI1xYTD8yn3E2jwA_Gc0FZkhfp6vYAv7BNGpTt_d9VFQN_Muv5-3wnpRmQtLy3Pk7soySZdyNm33wKKz7hRYQCxIbNMzjBlVU1ETxOQTZmHZOc_HfHB6EbZk3mKUrJYKdi5P-1K5IJDgIfuVvGM-MkEQ0-M-eQIn00dmwDo_UOw2YEHYAAzrELV72tvN_EZzapi2FmM_EMHbtIzMkN2kvAVmOzQ5tTzwU8v65NTy_3hqWZ-cWr6VU8v65NTygI4a6pNTy4M5taxPTi3fyqllfXJqeUxKyXifWlbCyibLZRXDZiUaVvKU5U1xqeytFwDWFXuL5um6YmAzSzfM0ra9rqwX9hG2YxY-s6y8j2RWaXNLMTbM7SJelXZQ_dBUztxkZs2EFrKUzaM0shVDj0oXirGn3FeMhK7OzCYxpEQsos0koomw8o1iTEf1eFyNzeK7punRZEyf2Q8r38pv1dVYLDKbTES0hI44PY4Qivt5iy27_5OUf5fc_xcAiF5-)

### 2.2 TprKO6 + TprKO3, link
Немного упрощено (АБС не включена в TprKO3)  
Используемые связи:
``` mermaid
graph LR;
CRM_ЮЛ --> АБС <--> Credit_ЮЛ;
CRM_ФЛ --> АБС;
```
- [mermaid.live/edit](https://mermaid.live/edit#pako:eNpVUEFOwzAQ_Iq15zTKOo2dGMQlPdJLj8gSsrDbRGrsyHUkIMof4MwJiTNvyZNwgorEbXd2ZnZ3Rnhy2oCAk1d9Q-4PN9LWh_3j_D1_kM3mjsxv8_v8SW6XuvZGt2GdXWlf_2gRlRaSaNZqEMEPJoHO-E4tLYzSEiIhNKYzEkQstTmq4RwkSDtFWa_sg3PdVendcGpAHNX5Eruh1yqYXavipd0f6o3VxtdusAEEYrmagBjhGUReYcq3WGw5YzxHigm8RBLDNK8KigXDoqQ4JfC6Ls1SlnHGOWY0K8uKljSB5V_n978RrUlNPwouZTU)
``` mermaid
graph LR;
ТпрКО6 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.3((Арх3.3)) --> АБС_ЦФТ:Арх3.3:software((software)) --> АБС_ЦФТАрх3.3Прикладное_ПО:_ЦФТ-Банк_Платформы_2MCA_DBI:Ри2([Прикладное ПО: ЦФТ-Банк Платформы 2MCA DBI<br>2.9.3<br>АО ЦФТ, 810]) 
CRM_ФЛ -. source .-> АБС_ЦФТ
CRM_ЮЛ -. source .-> АБС_ЦФТ
АБС_ЦФТ -. target .-> Кредиты_ЮЛ
ТпрКО6 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.3((Арх3.3)) --> АБС_ЦФТ:Арх3.3:software((software)) --> АБС_ЦФТАрх3.3Сервер_приложений:_Apache_Tomcat:Ри2([Сервер приложений: Apache Tomcat<br>9.0.85<br>Apache Software Foundation, 840]) 
CRM_ФЛ -. source .-> АБС_ЦФТ
CRM_ЮЛ -. source .-> АБС_ЦФТ
АБС_ЦФТ -. target .-> Кредиты_ЮЛ
ТпрКО6 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.3((Арх3.3)) --> АБС_ЦФТ:Арх3.3:software((software)) --> АБС_ЦФТАрх3.3Среда_исполнения:_Oracle_JDK_:Ри2([Среда исполнения: Oracle JDK <br>17.0.11<br>Oracle Inc., 840]) 
CRM_ФЛ -. source .-> АБС_ЦФТ
CRM_ЮЛ -. source .-> АБС_ЦФТ
АБС_ЦФТ -. target .-> Кредиты_ЮЛ
ТпрКО6 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.3((Арх3.3)) --> АБС_ЦФТ:Арх3.3:software((software)) --> АБС_ЦФТАрх3.3Системное_ПО,_ОС:_Ред_ОС_Сервер:Ри2([Системное ПО, ОС: Ред ОС Сервер<br>10.2<br>ООО «Ред Софт», 810]) 
CRM_ФЛ -. source .-> АБС_ЦФТ
CRM_ЮЛ -. source .-> АБС_ЦФТ
АБС_ЦФТ -. target .-> Кредиты_ЮЛ
ТпрКО6 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.3((Арх3.3)) --> АБС_ЦФТ:Арх3.3:hardware((hardware)) --> АБС_ЦФТАрх3.3Оборудование,_сервер:_Aquarius_C86_:Ри2([Оборудование, сервер: Aquarius C86 <br>T1F S28H<br>ГК «Аквариус», 810]) 
CRM_ФЛ -. source .-> АБС_ЦФТ
CRM_ЮЛ -. source .-> АБС_ЦФТ
АБС_ЦФТ -. target .-> Кредиты_ЮЛ
ТпрКО6 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.2((Арх3.2)) --> АБС_ЦФТ:Арх3.2:software((software)) --> АБС_ЦФТАрх3.2СУБД:_Postgres_Pro_Enterprise:Ри2([СУБД: Postgres Pro Enterprise<br>15.6.1<br>ООО «Постгрес Про», 810]) 
CRM_ФЛ -. source .-> АБС_ЦФТ
CRM_ЮЛ -. source .-> АБС_ЦФТ
АБС_ЦФТ -. target .-> Кредиты_ЮЛ
ТпрКО6 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.2((Арх3.2)) --> АБС_ЦФТ:Арх3.2:software((software)) --> АБС_ЦФТАрх3.2Системное_ПО,_ОС:_Ред_ОС_Сервер:Ри2([Системное ПО, ОС: Ред ОС Сервер<br>10.2<br>ООО «Ред Софт», 810]) 
CRM_ФЛ -. source .-> АБС_ЦФТ
CRM_ЮЛ -. source .-> АБС_ЦФТ
АБС_ЦФТ -. target .-> Кредиты_ЮЛ
ТпрКО6 --> АБС_ЦФТ(АБС ЦФТ<br>Основная АБС банка, АО_ЦФТ) --> АБС_ЦФТ:Арх3.2((Арх3.2)) --> АБС_ЦФТ:Арх3.2:hardware((hardware)) --> АБС_ЦФТАрх3.2Оборудование_сервера:_Aquarius_C86_:Ри2([Оборудование сервера: Aquarius C86 <br>T1F D88<br>ГК «Аквариус», 810]) 
CRM_ФЛ -. source .-> АБС_ЦФТ
CRM_ЮЛ -. source .-> АБС_ЦФТ
АБС_ЦФТ -. target .-> Кредиты_ЮЛ
ТпрКО6 --> CRM_ФЛ(CRM ФЛ<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM_ФЛ:Арх3.3((Арх3.3)) --> CRM_ФЛ:Арх3.3:software((software)) --> CRM_ФЛАрх3.3Прикладное_ПО:_Creatio:Ри2([Прикладное ПО: Creatio<br>8.0.9<br>Creatio / Terrasoft, 840]) 
CRM_ФЛ -. target .-> АБС_ЦФТ
ТпрКО6 --> CRM_ФЛ(CRM ФЛ<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM_ФЛ:Арх3.3((Арх3.3)) --> CRM_ФЛ:Арх3.3:software((software)) --> CRM_ФЛАрх3.3Среда_исполнения:_.NET:Ри2([Среда исполнения: .NET<br>8.0.6<br>Microsoft, 840]) 
CRM_ФЛ -. target .-> АБС_ЦФТ
ТпрКО6 --> CRM_ФЛ(CRM ФЛ<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM_ФЛ:Арх3.3((Арх3.3)) --> CRM_ФЛ:Арх3.3:software((software)) --> CRM_ФЛАрх3.3Веб-сервер:_Internet_Information_Services,_IIS:Ри2([Веб-сервер: Internet Information Services, IIS<br>10.0<br>Microsoft, 840]) 
CRM_ФЛ -. target .-> АБС_ЦФТ
ТпрКО6 --> CRM_ФЛ(CRM ФЛ<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM_ФЛ:Арх3.3((Арх3.3)) --> CRM_ФЛ:Арх3.3:software((software)) --> CRM_ФЛАрх3.3Системное_ПО,_ОС:_Microsoft_Windows_Server_2022:Ри2([Системное ПО, ОС: Microsoft Windows Server 2022<br>Standard<br>Microsoft, 840]) 
CRM_ФЛ -. target .-> АБС_ЦФТ
ТпрКО6 --> CRM_ФЛ(CRM ФЛ<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM_ФЛ:Арх3.3((Арх3.3)) --> CRM_ФЛ:Арх3.3:hardware((hardware)) --> CRM_ФЛАрх3.3Оборудование_сервера:_Dell_PowerEdge:Ри2([Оборудование сервера: Dell PowerEdge<br>R760<br>Dell Inc., 840]) 
CRM_ФЛ -. target .-> АБС_ЦФТ
ТпрКО6 --> CRM_ФЛ(CRM ФЛ<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM_ФЛ:Арх3.2((Арх3.2)) --> CRM_ФЛ:Арх3.2:software((software)) --> CRM_ФЛАрх3.2СУБД:_Microsoft_SQL_Server_2022:Ри2([СУБД: Microsoft SQL Server 2022<br>Enterprise Edition<br>Microsoft, 840]) 
CRM_ФЛ -. target .-> АБС_ЦФТ
ТпрКО6 --> CRM_ФЛ(CRM ФЛ<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM_ФЛ:Арх3.2((Арх3.2)) --> CRM_ФЛ:Арх3.2:software((software)) --> CRM_ФЛАрх3.2Системное_ПО,_ОС:_Microsoft_Windows_Server_2022:Ри2([Системное ПО, ОС: Microsoft Windows Server 2022<br>Datacenter<br>Microsoft, 810]) 
CRM_ФЛ -. target .-> АБС_ЦФТ
ТпрКО6 --> CRM_ФЛ(CRM ФЛ<br>CRM ФЛ банка, Creatio / Terrasoft) --> CRM_ФЛ:Арх3.2((Арх3.2)) --> CRM_ФЛ:Арх3.2:hardware((hardware)) --> CRM_ФЛАрх3.2Оборудование_сервера:_Dell_PowerEdge:Ри2([Оборудование сервера: Dell PowerEdge<br>R760xd<br>Dell Inc., 840]) 
CRM_ФЛ -. target .-> АБС_ЦФТ
ТпрКО3 --> CRM_ЮЛ(CRM ЮЛ<br>CRM ЮЛ банка, Creatio / Terrasoft) --> CRM_ЮЛ:Арх3.3((Арх3.3)) --> CRM_ЮЛ:Арх3.3:software((software)) --> CRM_ЮЛАрх3.3Прикладное_ПО:_Creatio:Ри2([Прикладное ПО: Creatio<br>8.0.9<br>Creatio / Terrasoft, 840]) 
CRM_ЮЛ -. target .-> АБС_ЦФТ
CRM_ЮЛ -. target .-> Кредиты_ЮЛ
ТпрКО3 --> CRM_ЮЛ(CRM ЮЛ<br>CRM ЮЛ банка, Creatio / Terrasoft) --> CRM_ЮЛ:Арх3.3((Арх3.3)) --> CRM_ЮЛ:Арх3.3:software((software)) --> CRM_ЮЛАрх3.3Среда_исполнения:_.NET:Ри2([Среда исполнения: .NET<br>8.0.6<br>Microsoft, 840]) 
CRM_ЮЛ -. target .-> АБС_ЦФТ
CRM_ЮЛ -. target .-> Кредиты_ЮЛ
ТпрКО3 --> CRM_ЮЛ(CRM ЮЛ<br>CRM ЮЛ банка, Creatio / Terrasoft) --> CRM_ЮЛ:Арх3.3((Арх3.3)) --> CRM_ЮЛ:Арх3.3:software((software)) --> CRM_ЮЛАрх3.3Веб-сервер:_Internet_Information_Services,_IIS:Ри2([Веб-сервер: Internet Information Services, IIS<br>10.0<br>Microsoft, 840]) 
CRM_ЮЛ -. target .-> АБС_ЦФТ
CRM_ЮЛ -. target .-> Кредиты_ЮЛ
ТпрКО3 --> CRM_ЮЛ(CRM ЮЛ<br>CRM ЮЛ банка, Creatio / Terrasoft) --> CRM_ЮЛ:Арх3.3((Арх3.3)) --> CRM_ЮЛ:Арх3.3:software((software)) --> CRM_ЮЛАрх3.3Системное_ПО,_ОС:_Microsoft_Windows_Server_2022:Ри2([Системное ПО, ОС: Microsoft Windows Server 2022<br>Standard<br>Microsoft, 840]) 
CRM_ЮЛ -. target .-> АБС_ЦФТ
CRM_ЮЛ -. target .-> Кредиты_ЮЛ
ТпрКО3 --> CRM_ЮЛ(CRM ЮЛ<br>CRM ЮЛ банка, Creatio / Terrasoft) --> CRM_ЮЛ:Арх3.3((Арх3.3)) --> CRM_ЮЛ:Арх3.3:hardware((hardware)) --> CRM_ЮЛАрх3.3Оборудование_сервера:_Dell_PowerEdge:Ри2([Оборудование сервера: Dell PowerEdge<br>R760<br>Dell Inc., 840]) 
CRM_ЮЛ -. target .-> АБС_ЦФТ
CRM_ЮЛ -. target .-> Кредиты_ЮЛ
ТпрКО3 --> CRM_ЮЛ(CRM ЮЛ<br>CRM ЮЛ банка, Creatio / Terrasoft) --> CRM_ЮЛ:Арх3.2((Арх3.2)) --> CRM_ЮЛ:Арх3.2:software((software)) --> CRM_ЮЛАрх3.2СУБД:_Microsoft_SQL_Server_2022:Ри2([СУБД: Microsoft SQL Server 2022<br>Enterprise Edition<br>Microsoft, 840]) 
CRM_ЮЛ -. target .-> АБС_ЦФТ
CRM_ЮЛ -. target .-> Кредиты_ЮЛ
ТпрКО3 --> CRM_ЮЛ(CRM ЮЛ<br>CRM ЮЛ банка, Creatio / Terrasoft) --> CRM_ЮЛ:Арх3.2((Арх3.2)) --> CRM_ЮЛ:Арх3.2:software((software)) --> CRM_ЮЛАрх3.2Системное_ПО,_ОС:_Microsoft_Windows_Server_2022:Ри2([Системное ПО, ОС: Microsoft Windows Server 2022<br>Datacenter<br>Microsoft, 810]) 
CRM_ЮЛ -. target .-> АБС_ЦФТ
CRM_ЮЛ -. target .-> Кредиты_ЮЛ
ТпрКО3 --> CRM_ЮЛ(CRM ЮЛ<br>CRM ЮЛ банка, Creatio / Terrasoft) --> CRM_ЮЛ:Арх3.2((Арх3.2)) --> CRM_ЮЛ:Арх3.2:hardware((hardware)) --> CRM_ЮЛАрх3.2Оборудование_сервера:_Dell_PowerEdge:Ри2([Оборудование сервера: Dell PowerEdge<br>R760xd<br>Dell Inc., 840]) 
CRM_ЮЛ -. target .-> АБС_ЦФТ
CRM_ЮЛ -. target .-> Кредиты_ЮЛ
ТпрКО3 --> Кредиты_ЮЛ(Кредиты ЮЛ<br>Кредитный конвейер ЮЛ банка, Интегратор 1) --> Кредиты_ЮЛ:Арх3.3((Арх3.3)) --> Кредиты_ЮЛ:Арх3.3:software((software)) --> Кредиты_ЮЛАрх3.3Прикладное_ПО:_ELMA_BPM_Suite_Enterprise:Ри2([Прикладное ПО: ELMA BPM Suite Enterprise<br>4.2.10.55<br>ELMA, 810]) 
АБС_ЦФТ -. source .-> Кредиты_ЮЛ
Кредиты_ЮЛ -. target .-> АБС_ЦФТ
ТпрКО3 --> Кредиты_ЮЛ(Кредиты ЮЛ<br>Кредитный конвейер ЮЛ банка, Интегратор 1) --> Кредиты_ЮЛ:Арх3.3((Арх3.3)) --> Кредиты_ЮЛ:Арх3.3:software((software)) --> Кредиты_ЮЛАрх3.3Среда_исполнения:_.NET_Core_Runtime:Ри2([Среда исполнения: .NET Core Runtime<br>8.0.6<br>Microsoft, 840]) 
АБС_ЦФТ -. source .-> Кредиты_ЮЛ
Кредиты_ЮЛ -. target .-> АБС_ЦФТ
ТпрКО3 --> Кредиты_ЮЛ(Кредиты ЮЛ<br>Кредитный конвейер ЮЛ банка, Интегратор 1) --> Кредиты_ЮЛ:Арх3.3((Арх3.3)) --> Кредиты_ЮЛ:Арх3.3:software((software)) --> Кредиты_ЮЛАрх3.3Веб-сервер:_Internet_Information_Services,_IIS:Ри2([Веб-сервер: Internet Information Services, IIS<br>10.0<br>Microsoft, 840]) 
АБС_ЦФТ -. source .-> Кредиты_ЮЛ
Кредиты_ЮЛ -. target .-> АБС_ЦФТ
ТпрКО3 --> Кредиты_ЮЛ(Кредиты ЮЛ<br>Кредитный конвейер ЮЛ банка, Интегратор 1) --> Кредиты_ЮЛ:Арх3.3((Арх3.3)) --> Кредиты_ЮЛ:Арх3.3:software((software)) --> Кредиты_ЮЛАрх3.3Системное_ПО,_ОС:_Microsoft_Windows_Server_2022:Ри2([Системное ПО, ОС: Microsoft Windows Server 2022<br>Standard<br>Microsoft, 840]) 
АБС_ЦФТ -. source .-> Кредиты_ЮЛ
Кредиты_ЮЛ -. target .-> АБС_ЦФТ
ТпрКО3 --> Кредиты_ЮЛ(Кредиты ЮЛ<br>Кредитный конвейер ЮЛ банка, Интегратор 1) --> Кредиты_ЮЛ:Арх3.3((Арх3.3)) --> Кредиты_ЮЛ:Арх3.3:hardware((hardware)) --> Кредиты_ЮЛАрх3.3Оборудование_сервера:_Dell_PowerEdge:Ри2([Оборудование сервера: Dell PowerEdge<br>R760<br>Dell Inc., 840]) 
АБС_ЦФТ -. source .-> Кредиты_ЮЛ
Кредиты_ЮЛ -. target .-> АБС_ЦФТ
ТпрКО3 --> Кредиты_ЮЛ(Кредиты ЮЛ<br>Кредитный конвейер ЮЛ банка, Интегратор 1) --> Кредиты_ЮЛ:Арх3.2((Арх3.2)) --> Кредиты_ЮЛ:Арх3.2:software((software)) --> Кредиты_ЮЛАрх3.2СУБД:_Microsoft_SQL_Server_2022:Ри2([СУБД: Microsoft SQL Server 2022<br>Enterprise Edition<br>Microsoft, 840]) 
АБС_ЦФТ -. source .-> Кредиты_ЮЛ
Кредиты_ЮЛ -. target .-> АБС_ЦФТ
ТпрКО3 --> Кредиты_ЮЛ(Кредиты ЮЛ<br>Кредитный конвейер ЮЛ банка, Интегратор 1) --> Кредиты_ЮЛ:Арх3.2((Арх3.2)) --> Кредиты_ЮЛ:Арх3.2:software((software)) --> Кредиты_ЮЛАрх3.2Системное_ПО,_ОС:_Microsoft_Windows_Server_2022:Ри2([Системное ПО, ОС: Microsoft Windows Server 2022<br>Datacenter<br>Microsoft, 810]) 
АБС_ЦФТ -. source .-> Кредиты_ЮЛ
Кредиты_ЮЛ -. target .-> АБС_ЦФТ
ТпрКО3 --> Кредиты_ЮЛ(Кредиты ЮЛ<br>Кредитный конвейер ЮЛ банка, Интегратор 1) --> Кредиты_ЮЛ:Арх3.2((Арх3.2)) --> Кредиты_ЮЛ:Арх3.2:hardware((hardware)) --> Кредиты_ЮЛАрх3.2Оборудование_сервера:_Dell_PowerEdge:Ри2([Оборудование сервера: Dell PowerEdge<br>R760xd<br>Dell Inc., 840]) 
АБС_ЦФТ -. source .-> Кредиты_ЮЛ
Кредиты_ЮЛ -. target .-> АБС_ЦФТ
```

- [mermaid.live](https://mermaid.live/view#pako:eNrtW11PG0cU_StX-2Qks_WusbG3VSSCiUoTWoqRKrWuRlt7MJZgl47XTdooUiDpEw-hHw9VKpGQVn2pZDlpqaAkRMovmP1HvTO7628vNirBJiska3Z9z_Xcc-7cmes1d5WiXaKKoZSZubUOt1beL1j8GX_t3ueP-X4apqevAd_jP_ADwv_gv_NnMe8KvKsPvmLX-L67zV_xU_4CXxvuIwgsnvMG3vmXN-Li1r7vYKrXp8H33Pvu90k1GYs1h1OhhkbVXnNum4zGYsGoH6Bpz59gREc4mROc1N9yuoeEP-H7hm85jSg5XXEXjdwd9yE_RdBLd5foS_NzJHd90eBP-ZEe-6KfN5DeoMsb9HoD4Q3QmyBPV7NqUrKIDPngOGS0xJdTULDmV5YI3vkVplWo2jVWpKB2h-hb1c-y6rgUpo7JytTxTB_j1A4xkiOc6K50dkXT4IAfYkwvxCuR4R2hPKf8H4z-FY6PDTK3ZRbXKVm1N4um0xS8DQd9ceDhwMMJQrJqQs2kxMh_K-_PEG7YNatkOhXbQqlnIqkvSGo_0AbBWLf5a5zvCc5OCuY-MsgnzCxuUPJR7iZpyRxgoC8GPAwgBgQR2ixqrGli6L-zaBXVSNSLXL-oi7uDwb5sK-Jxwvf5AZbyp4IFeUHal2zbMu6Cy6qNgQk4eHB5Ae1wKXVC1T2axB-8-TMwPsC6_tDdeXMSle3hZV83WcmTPRiFy76P08Ht032AwYqpNmTVPYwTnHxLZTL3dc1klVqVzGfSrUU9CAwdYAjAgGC5ule1G5DXMx9Kmn7ij4Xoe8gIehAbgPvA3Y5UV_WW6nqo6vqIi13HpfUb3v_ZIMt21SkzWiXLzCYLlkPZFqtUaduy9gwhMAQ0hJahXMApNa1qnUv4CeaFKAd_CUbdbZDnutNI1IsVNargV0D20Sq4PqgIdxRw3hixhEMXun8Nz2Uyk1jCg8nEcABiIIIIxh3qzjMqugl4D1YpY6ZYh1MdLsK26F6bwUs6sB2mrfYnNUTL7FuK8DJ4ns7KOHtD6n-sbme1S4BJ5POspkX9eGF16G5FGAespsVgqVJk9jvD5Y_IxPPpzhPiojgTWNTBwZrNNmUTTvKUfVMp0mqcLC7mm-z2gUMAhzY4NOGAcH-nSbx7dIdv7E0uyGcVq2TfrkrWKSN6QteH3N2bPsD3AZ4PED4EJXnHtEq4HV0R8gfusb3kD7u95ujGBh6nb1O2UCrTkfdXAYcmXBCxMpuWuS7fGfztx-XS3edc02szfK63dSattM5_emtASvu9SSt70bQ7c1u9CiyUKqKsjH0OXwCpl15AcqZjFqnQopt-bTLpH7qE6JdbQu6U_qcikmxFVw8Ir7cRXh-J8PoQNbs-woZZH4-zc_0sPgdZhfctE8T95ZyzI97H9kweSTMh5_crKlT4Rl2fiLP-xEkz6AxVH-EIWx-jviASYGJ6iCsq1dBlbKz7jQsVp49RrPNeU7L22_yVu8uPAWU7xUgxPH7s_RqpW1L-C5qK7BVPNRs4QpZAmxr02aGP78PMQ5789cKG6XoWbi3NkevLSyRfqzi033PewX2QwAJiQWK7Hv3OqLqK57-U_DGWsGytxZ6nNO0PdPqq2XtztNb0HZd_mMaLzNuMkpWa5VQ26UhdGAgk-MizWrJI-7es_Tg2f1ESvO0CMPZtZpQS506Jwb8KCUuJcWxooyQI-1FQmPm56sJlts6R1G9d6vFv0qOkOHdSnGcTGNevAy46DZS4UmaVkmI4rEbjyibFM6y4VO4WLICC4qzTTVpQDByW6JpZ23AKSsG6h7At0_rctjcDJLNr5XXFWDM3qnhV2yqZDs1VzDIzWybUKlE2b2N3pBjZpHShGHeVO4qhZRNqNqknUplkQtOyKS2ufKsY09nZlJpMzcwkZnQ9k9Uzs_fiynfyQzU1k8jOJmezqUQyk0pn03GFYpG12ZL374Tyvwrv_QfIu3ft)

- [edit](https://mermaid.live/edit#pako:eNrtW11PG0cU_StX-2Qks_WusbG3VSSCiUoTWoqRKrWuRlt7MJZgl47XTdooUiDpEw-hHw9VKpGQVn2pZDlpqaAkRMovmP1HvTO7628vNirBJiska2Z8z3juOXfuzPWau0rRLlHFUMrM3FqHWyvvFyz-jL927_PHfD8N09PXgO_xH_gB4X_w3_mzmNcDr_fBV-wa33e3-St-yl_ga8N9BIHFc97AkX95Iy6G9v0JpnrnNPiee9_9PqkmY7FmcyrU0Kjaa85tk9FYLGj1AzTt-RP06AgXc4KL-lsu95DwJ3zf8C2nESWXK0bRyN1xH_JTBL10d4m-ND9HctcXDf6UH-mxL_rNBnI26JoNemcDMRvgbII8Xc2qSckiMuSD45DREl9OQcGaX1kiOPIrTKtQtWusSEHtdtG3qp9l1dEVpo7JytTxTB_j0g7RkyNc6K6c7IqGwQE_RJ9eiFci3TtCeU75P-j9K2wfG2RuyyyuU7JqbxZNpyl4Gw764sDDgYcThGTVhJpJiZb_Vt5fIdywa1bJdCq2hVLPRFJfkNS-ow2Cvm7z17jeE1ydFMx9ZJBPmFncoOSj3E3SkjnAQF8MeBhADAgitFnUWNNE039n0SqqkagXuX9RF3cHnX3ZlsTjhO_zA0zlTwULskPat2zbNu6Cy6yNjgk4eHDZgXa4lDqh6h5N4g_e_BkYH2Bef-juvDmJ0vbwsq-brOTJHrTCZd_H5eDx6T5AZ8VSGzLrHsYJLr6lMpn7umaySq1K5jPp1qYeBIYOMARgQLDc3avaDcjrmQ8lTT_xx0L0PWQEZxAHgPvA3Y5UV_WW6nqo6vqIm13HrfUbjv9skGW76pQZrZJlZpMFy6Fsi1WqtG1be4YQGAIaQstQbuCUmla1zi38BONCpIO_BKPuNsh73Wkk6sWKGmXwKyD7aBlcH5SEOxI4b4yYwqEL3T-H5zKZSUzhwWJi2ADREE4E7Q515xkV1QS8B6uUMVPsw6mOKcKO6F6bwVs6sB2mrPYXNUTJ7FsK9zJ4n85KP3td6n-tbme1S4BJ5POsokX9eGF16GpFGAespkVjqVJk9jvD5Y_IxPPpzhviorgTWNTBxprNNmURTvKUfVMp0mqcLC7mm-z2gUMAhzY4NOGAcP-kSbx7dIcf7E0uyGcVq2TfrkrWKSN6QteHPN2bc4A_B3hzgJhDUJJ3TKuEx9EVIX_gGdtL_rDHa45ubOB1-jZlC6UyHfl8FXBowgURK7NpGevyncHfflwu3X3uNb02w8d6W2XSCuv8p7cGhLRfm7SiF027I7dVq8BCqSLSytjH8AWQeukJJGc6ZpEKLbrp1yaT_qFTiH65KeRO6X9KIsmWd_WA8Hob4fWRCK8PkbPrIxyY9fG4O9fP4nOQVXjdMkHcX849O-J9bO_kkTQTcn-_okKFH9T1ibjrT5w0g-5Q9RGusPUxqgsiASamhriiUg2dxsa63rhQcfoYxTrHmpK1D_NX7i4_BpTtFD1F9_ix92ukbkn5L2gqolc81WxgC1kCbWrQZ4c-vg8zD3ny1wsbpupZuLU0R64vL5F8reLQfs95B9dBAguIBYntevQ7o-oq3v9S8sdYwrK1F3ue0rQ_0OmrZu_gaKXpOy7_MIUXmbcZJSs1y6ls0pGqMBBI8JFnlWSR9m9Z-3Es_qIgeNsJYOzLzCgkzh0Sg38VEhYS41jQRkEQ9qOgMPNz5YXLLJ0jqd-61ONfpEdBce6gOM8hMK5fB1x0GChxpcwqJcVwWI3GlU2Kd1jRVe4WLICC4qzTTVpQDGyW6JpZ23AKSsG6h7At0_rctjcDJLNr5XXFWDM3qtirbZVMh-YqZpmZLRNqlSibt7E6UgwtJadQjLvKHexpKVVL6slsNqPNZLOpxGxc-VYxpjOJlJrQUklN01NpLa2l7sWV7-SnYkWtJRKJ5ExyJpGaTaZnEUExzdpsyfuHQvl_hff-A6kveB0)

- без упрощения [edit](https://mermaid.live/view#pako:eNrtXFtvG0UU_itH--RIzrLeTRx7QZXSJIhAAyWOhARGo8WeOJbi3TBe00JVqWnLUx9aLg-oSGlTEC9IllsISmmbSv0Fs_-IM7O7vntjR6TxZRXFml2fbzLn-86cmZP1-IZScIpUMZUSs_Z24Mrmu3mbP-GvvVv8IT9Iw_z8JeAP-A_8kPA_-O_8ScK_Av_qva_YJX7g7fNX_IQ_w9eGdx9Ci6e8gXf-5Y2kuHUQdDDX26fJH3i3vO8N1Ugkms25SEOz6my71yxGE4mw1Q_QtOeP0KNjHMwLHNTfcrhHhD_iB2ZgOY8oOVxxF428295dfoKgl949om-sLJPVy-smf8yP9cQX_XoD2Rt09Qa9vYHoDbA3QZ6uZlVDsogMBeAkZFLal3OQt1c2Nwje-RXmVag6NVagoHa7GFjVT7PquBSmrsVK1PVNH-LQjtCTYxzoPdnZlIbBIT9Cn56JVyLdO0Z5Tvg_6P0rbD83yfKeVdihZMupFCy3KXgbDvriwMeBjxOEZFVNzSyKVvBWLhghvO_U7KLllh0bpV6IpT4nqQNHGwR93eevcbwvcHRSMO--ST5hVmGXkg9XPyItmUMM9MWAjwHEgCAitYQap1KiGbyzbhfUWNTznL-oi3cbnX3ZlsSThB_wQ0zljwUL8oK0T9m2adwFl1kbHRNw8OHyAtrhUmpN1X2axA-8-TM0PsS8fte7_eZFnLaHl33HYkVf9rAVLfsBDgeXT-8OOiuG2pBZ9yhJcPAtlcny1zWLlWtVspJJtyb1IDB0gCEEA4Ll7N5KvQ85PfOBpOkn_lCI_gAZwR7EAuDd8fZj1VW9pboeqbo-4mTXcWr9hvd_NslVp-qWGK2Sq8wha7ZL2R4rV2nbtPYNITQENISWoZzAi2paTXVO4UcYFyId_CUY9fZB7utOYlHPV9Q4g0-B7KNlcH1QEu5I4LwxYgqHLnT_HL6ayUxiCg8Hk8AGiIZwImx3qLvCqKgm4B3YooxZYh7OdXQRtUT32gye0qHtMGV1MKghSubAUriXwf10VvrZ61L_bXU7q10CTCKfpxUt6sdrW0NXK8I4ZDUtGhvlAnNmhssfkYmn8507xHWxJ7Cpi41th1VkEU5ylH1TLtBqkqyv55rs9oFDCIc2ODThgPBgpdFmj-7ohb3JBfmsbBeda1XJOmVE13R9yNW92QcEfYDfB4g-BCU517KLuBxNCfkD19he8oddXlfp7i5up69RtlYs0ZHXVwGHJlwQsbmUlrEu3xn834-LpbvPvqbXZvhYb6tMWmGd-_TKgJAOapNW9KJpd-S2ahVYK5ZFWhn7GD4HUi88gaxarlWgQotu-lOTSf_QKUS_2BRyvfg_JRGj5V09JLzeRnh9JMLrQ-Ts-ggLZn089s710_gcZBVdt0wQ9xezz455H9s9eSzNhOzfp1So6IW6PhF7_YmTZtAeqj7CFrY-RnVBLMDE1BBTKtXQaWys641zFaePUaLzXlOy9tv8lXePPweU7QQ9Rff4c__TSN2S8l_QVESveKrZwBayBKm5QX878vF9lHnEk79e2DBVz9qVjWVy-eoGydXKLu33nHdwHSSwgFiQ2K5HvwuqruL-b1F-GEtYtuZiz1Oa9gc6fdXsvTlaaTrj8g9TeJEVh1GyWbPdcoWOVIWBQEKAPK0ki7V_y9qPY_EXB8HbTgBjX2bGIXHmkBj8qZCokBjHgjYOgqgPBUWZnykvXGTpHEv91qUe_yI9DoozB8VZFoFx_XfABYRBfNputk_bGfFpu1k5bWfEp-2m77SdEZ-2m8WzGkZ82m4GT9sZ8Wm76TttZ8Sn7eIMHp-2m-LTdkpSKbFyUTFdVqNJpUJZxRKXyo28DZBX3B1aoXnFxGaRblu1XTev5O2bCNuz7M8dpxIimVMr7SjmtrVbxavaHhYadLVslZjVMqF2kbIVrEJcxVySPSjmDeW6Yhq6oWbS2exCSl80MkYqm1S-Vcz5lK5rqrakawtpI5PV8PdmUvlO_lFD1RYW02ltSUtrC3pKW0wqtFh2Hbbhf4uP_DKfm_8BHSTIew)
  
### 2.3 Comment
К избыточности формата:
- Если мы хотим добавить на схему, например, [ТПрКО7](https://ivo.garant.ru/#/document/406750235/entry/100900/doclist/1821/1/0/0/6406-%D0%A3:0) Технологический процесс, обеспечивающий открытие и ведение банковских счетов юридических лиц, то нужно добавлять еще десяток строк, хотя все данные (системы) на схеме уже есть (CRM ЮЛ + АБС). Кроме чудовищной избыточности это ничего не даст.
- Если мы хотим добавить Типовое рабочее место Сотрудника банка с установленным на нем "клиентской частью" CRM, АБС, то нам нужно отдельными строчками (арх-строками) добавлять его в Каждую АС (например, в трехзвенной архитектуре как Арх3.1 - браузер, системное ПО, оборудование ПК) 
- Если бы ТП можно было перечислять в первой позиции, то это резко сократило бы избыточность.
- Системы источники и системы приемники - в большинстве случаеы одни и те же. Без указания типа данных (что передается) - смысл в этих связях - минимален, т.к. они двухстороние и без указания что же (какие сущности) передается 
