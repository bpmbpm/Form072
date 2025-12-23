## Example 
## 1 Easy
Особенности: 
- Данные взяты из https://github.com/bpmbpm/doc/blob/main/IT/reliability_risk/risk/850P/f072/server.md  
- Упрощено, включая, минимазацию компонентов, отказ от виртуализациии и т.п.
 
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

```

```

- [mermaid.live]
- 
- [edit]
                
### 1.3 TprKO6, link
Процесс ТпрКО6 - с взаимосвязью систем (АС), т.е. sysSourceTarget: 'yes' 

```

```

- [mermaid.live](https://mermaid.live/view#pako:eNrtWFtvG0UU_itH--RIzuJd39YLqhTsVBgaKHEkJDAaLd6JbcneNeM1aYkiNWl54qHh8lQkpymIF17cgpEhJZX6C2b_EWdmd32rndooqGlSRbFmds53fM53brPeVSquTRVTqTKrVYMbm2-XHf6IP_Pv8Ae8m4HV1WvAD_l3_Fgj_Ff-C38UC7cQbN_5gl3jXX-f_8NP-RP87Pn3QwTwx7yHT_7mvbh41A01rMzQavJD_47_TVJNxmLD5crZkmbb3fZ2LEZjsWg1EzEE8CN0a4D2nKBdf0iL-4Qf8a4ZSq4iTFosnqKQf-Df46cIeup_S_SN_BopvFs0-UM-0GOfzdIGUhtMaYMXtYHQBqhN8KerOTUpiUSSQnAcDC3x-QqUnfzmxgynLnOYjnkfHXsiPon0cYD0nfI_eR_NHPC_TLLWsio1SrbcZsXyhgEZw8FMHAQ4CHCCk5yaUI20WIVHpdBEuO52HNvy6q6DoUhd2VCgW33M7h7hAzT5GZp8ggZKQv37JvmIWZUGJe8XPiCjMEQYmImBAAOIAcGFlsUYaJpYhidFp6JeadIFb_4BMvZ0rEnFCe_yY2xVDwW7ckPGU36sDKbgsiuhbwIOAVxuYBwuQ5FQ9YAp8QfPf4uEj7Fv3fMPnp9corZUs5gdhCVavSQsXbQI27d_F3NbWNuTXaUfJ2j_KApk7cuOxeqdNskbmVFRzAPDBBgiMCBYVseWdh1KuvGeZOoH_kAE5RBJQQ2iwfl3_f0LHxV9FBX97KjoyxaLjqn5Mx78aJKbbturMtomN5lL1h2Pshart-lYWQSCEAkCCsJIUBZAWs2o2mQJHGHcRDn9Ltqavw9y7p9eddLfdKj_PyxLdih9XpOZaFC8t2SLgin07B5VMIxzblEoF8N_oVVAUOinCcbzjIrrGbwFW5QxS2TuSgQ8ayBMHM9PfRRb5MUhtGKBl4JQUvhj4I0nJx170YflLz4XiaiX3RfVD9e3Fr4oCuGIroxYbNQrzH39SfoeXXy8OnlrKIo55FAPF9sua8oXD1Ki7Kt6hbbjpFgsDWmbAYcIDmNwGMIB4WH3TFwiHs-eQkMnySd1x3Z32pJOyoie0PUFR9FQB4Q6INABQofgoORZ-JbI7NeC1bnzZILVRYdIgTYaeOnaoWzdrtKlp4iAwxAuPN_MZmR2ypP_9g54LjzOGNETxwtl59jFdJSIpY9vzEnC8Go6yjcUnc610VUV1u26qPCLkHXnxtYrr-WC5VkVKkie5lW7iLwuUs36q63mW_ZS9azElSqr24rpsQ6NK02Kg0xsld2yA1BWvBpt0rJi4tKm21an4ZWVsrOHsJblfOq6zQjJ3E61ppjbVqONu07LtjxaqFtVZo1EqGNTlnc7jqeYaalBMXeVW7jJZdSMjjHPadkUfsaV24qJk9MwtFw2rSW0ZDKTS6b24srX8is1VU_quXQiY2RTCSOVyibjCsX6dNlG8NO6_IV971_htYS_)
- [edit](https://mermaid.live/edit#pako:eNrtWFtvG0UU_itH--RI9rIXX9YLqhTsVBgaKHEkJDAaLd6JbcneNeM1aYkiNWl54qHh8lQkpymIF17cgpEhJZX6C2b_EWfG61tqpzYKappUUayZnfMdn_Od26x3lLLvUsVWKsxpVuHGxtsljz_iz8I7_AHvpCGRuAb8gH_Hj3TCf-W_8EexaAuD7TtfsGu8E-7xf_gJf4Kf3fB-hAD-mHfxyd-8GxePOpGGlRlabX4Q3gm_MVUzFhstV86WtFv-VrDtMBqLDVczESMAP0S3-mjPMdr1h7S4R_gh79iRZAJh0mLxFIXC_fAeP0HQ0_BbYqznVkn-3YLNH_K-EftsljaQ2uCUNnhRGwhtgNoEf4aaVU1JJJIUgeNg6drnK1DychvrM5y6zGE64j107In4JNLHPtJ3wv_kPTSzz_-yyWrTKVcp2fQbZScYBWQCBzNxMMDBACc4yaqaaqXEKjoqRibCdb_tuU5Q8z0MRfLKhgLd6mF2dwnvo8nP0ORjNFASGt63yUfMKdcpeT__ARmHYYiBmRgYYAAxILjQMxgDXRfL6KTgldUrTbrgLdxHxp5ONKk44R1-hK3qoWBXbshkyk-UwSm47Erom4DDAC43MAmXodBUY8CU-IPnvw2Fj7Bv3Qv3nx9forZUdZg7CMtw9ZKwdNAibN_hXcxtYW1XdpVenKD94yiQ1S_bDqu1WyRnpcdFMQ8MU2AYggHBsjo29etQNKz3JFM_8AciKAdICmoQDS68G-5d-KgY46gYZ0fFWLZYDEzNn_HgR5vc9FtBhdEWucl8suYFlDVZrUUnymIgCENBQEEYC8oCSKlpVZ8ugUOMmyin30VbC_dAzv2Tq076mw71_4dlyQ5lzGsyUw2Kd5dsUXAKPbtH5S3rnFsUysXwX2gVEBT6aYrxHKPiegZvwSZlzBGZuzIEnjUQpo7npz6KLfLiEFmxwEtBJCn8sfDGk5WOvejD8hefi0TUy-6L6odrmwtfFIXwkK60WKzXysx__Un6Hl18nJi-NRTEHPJogIstnzXkiwcpUvZVrUxbcVIoFEe0zYDDEA4TcBjBAeFR99QuEY9nT6GRk-STmuf62y1JJ2XE0AxjwVE00gGRDhjoAKFDcFAMHHxLZO5rwerceTLF6qJDJE_rdbx0bVO25lbo0lNEwGEEF55vZNIyO-XJf3sHPBceZ4zoqeOFsnPiYjpOxOLHN-YkYXQ1Hecbip7OtfFVFdbcmqjwi5B158bWK6_lvBM4ZSpIPs2rfhF5XaSajVdbzbfcpepZiSsVVnMVO2BtGlcaFAeZ2Co7JQ-gpARV2qAlxcalS7ecdj0oKSVvF2FNx_vU9xtDJPPblapibzn1Fu7aTdcJaL7mVJgzFqGeS1nOb3uBYqekBsXeUW4ptmkk1ZSh6ZapmXpaz5p4eluxE6alZrR0Nqtp2ayJjljp3bjytfxWXU2amZSeyaQN3UrqSTOuUKxQn60PflyXv7Hv_gvecYUb)

### 1.4 Comment
Получается много избыточных линий (соединений): с одной стороны "одна арх-запись" = один "сквозной путь" (end-to-end), т.е. можно выделив строку подсветить весь набор стрелок к ней. Первый end - это ТП, а послений end - "деталь" от ИТ-продукта.  
Замечания к форматам:
- в логическом формате "арх-записи" убрать дублирование
- в физическом формате "арх-записи" заменить "велосипед" из CSV (Comma-Separated Value) c разделителем "|" на какой-либо более "человеческий" формат типа JSON \ YAML, а еще лучше RDF. 

