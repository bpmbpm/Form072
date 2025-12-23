## Example 
## 1 Easy
### 1.1 fragment of process TprKO6
ТпрКО6 - открытие и ведение счетов ФЛ. Данные из https://github.com/bpmbpm/doc/blob/main/IT/reliability_risk/risk/850P/f072/server.md
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

[mermaid.live](https://mermaid.live/view#pako:eNrtl8tu00AUhl_laFap5Fj2uEkdgyqVlooCFQi6gqCRSdwmUmMHxxGXqhItsGJBEay6SC8gNmxCISjQUiSe4PiNODNxLi1poRILoChSNGPP_-fM5-M_9hIrBEWPOWwhdKsluHztTN7HbfwaP8R1bGQhnR4HXMPnuGUKfIOvcTuVTKEzPXs7HMdGvIJfcB936LsZP0sUgO-wSUc-Y1OThxqJw8gQVwfX4ofxE0u3UqnecOT4lU4tmI_uuqGXSnVHQxU9AW7QttpUzy7V9UFV3BK4gQ0nWZkmmapYHqVF8Wr8GPdJtBc_FXx2ckJMnZtxcBPbPHVzmBsoNzjkBj-6gXQDcpP8uJ7TLQWSICViDWzTuDUC__Ll2MIWbWxHfgu1xzZh2seP2KIy2_jJERNVt1DyxFxQKbhRD_yADobqoKODjk4yyemGbmfkKDl1PSkRpoO6X3SjcuAT8tF_Hjltq0Xd2hTYppK_Usm7VKACFz9zxJXQLSx64uLUJdHH3dXAUA10NEAakCzMMWJtmnKYnJnxC_qpgCv5xKtEZm8gXDSBDdyiiNmUFNVEDLbwQFsfkqs0ob1JOXTkagKDcoXc0HmHlPzAt7fdxVuUN4_j1W-7f2GclNyw2MHfHf0Ef4MqoniNH1GvymqbKg1amqD6-7TFxJ26G5brNTFpZ_tNfpQYDoihKwYSq26fM6fhOrcvKFIvcF3CXyMo5CCDKX4Ur_wx9HmfPj-ePj9p8_Mj_1s12eyvSPPSEVeDWrQQejVxNQzEeT_ywmpYrnk__UfVoOcBXQ8gD-h7qNsgo2d18-CNsEFXVd5U72WIxSugfmP_dFyS_3n0O_GfMI_4UZFyII6wecJAgkPq4Yk0Zdu_FEhMowf_cpE5UVj3NFbxwoorp2wp7wPkWVTyKl6eOTQsevNufTHKs7y_TLKq698IgkpXGQb1hRJz5t3FGs3qVXqi8qbKLr1V9Jd4ftELJ-lxK2JOTjkwZ4ndYw63TJ3nLINzy7AtnrE0dp85aT6qG9wwctmMbRlWxswta-yB-k1TN3OZ7JiZoTO2YfIxjXnFchSEs52XGfVOs_wdSazPnQ)


