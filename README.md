# hse_hw2_chip

Ссылка на колаб: https://colab.research.google.com/drive/1OkTINcEtY4aURBlSBg1zbTKVBgxJkx_h?usp=sharing


## FastQC отчеты
#### ENCFF000VIR
![Снимок экрана от 2022-03-11 11-33-19](https://user-images.githubusercontent.com/93282657/157831720-58fdf41f-576c-4def-a1dc-d972cb45ab70.png)
![Снимок экрана от 2022-03-11 11-37-09](https://user-images.githubusercontent.com/93282657/157831947-9579e1b7-cc84-4082-ab30-301f45f075b7.png)
![Снимок экрана от 2022-03-11 12-53-55](https://user-images.githubusercontent.com/93282657/157844290-1e86c7f5-4d76-4df9-9f93-f46afe849d14.png)
![Снимок экрана от 2022-03-11 12-54-03](https://user-images.githubusercontent.com/93282657/157844295-0e509077-6fd5-437d-81a9-0a4f8975f82b.png)
![Снимок экрана от 2022-03-11 12-54-12](https://user-images.githubusercontent.com/93282657/157844304-e8ad25f9-7f1d-4da0-b507-0b871ae69704.png)
![Снимок экрана от 2022-03-11 12-54-19](https://user-images.githubusercontent.com/93282657/157844317-9291edb2-bb4f-4f0c-8df6-a47f7d51838d.png)


В отчете обнаружилось одно предупреждение и одна ошибка:
1) ошибка Per tile sequence quality
2) предупреждение Per base sequence content

Per base sequence quality прошел проверку, эта характеристика является ключевой, так что наличие ошибки не так важно и можно не триммить файл.

#### ENCFF000VIP
![Снимок экрана от 2022-03-11 11-57-48](https://user-images.githubusercontent.com/93282657/157835184-c505253e-a6b8-4c45-9eb8-5a4f954cb873.png)
![Снимок экрана от 2022-03-11 11-58-45](https://user-images.githubusercontent.com/93282657/157835275-2a210d6b-380f-40f9-82ed-b8eee0e6d24d.png)
![Снимок экрана от 2022-03-11 12-01-01](https://user-images.githubusercontent.com/93282657/157835691-428462f5-dfbe-49ee-80db-958b2a9d6ab3.png)
![Снимок экрана от 2022-03-11 12-56-03](https://user-images.githubusercontent.com/93282657/157844622-c0f71259-1015-4697-90fa-560ed9898611.png)
![Снимок экрана от 2022-03-11 12-56-12](https://user-images.githubusercontent.com/93282657/157844632-811e686c-6767-4cab-9e14-45776cd975da.png)
![Снимок экрана от 2022-03-11 12-01-10](https://user-images.githubusercontent.com/93282657/157835699-9f425244-1f20-454d-b4de-39ea57b2b5b9.png)

Всего 3 предупреждения и нет ошибок. Per base sequence quality так же показывает хорошее качество. Можно не редактировать файл.
Предупреждения:
1) Per tile sequence quality
2) Per sequence GC content
3) Per base sequence content

#### ENCFF000VJK
![Снимок экрана от 2022-03-11 12-06-53](https://user-images.githubusercontent.com/93282657/157837048-5bca8e75-ef3f-4a18-bdf1-61d67332f5bf.png)
![Снимок экрана от 2022-03-11 12-07-01](https://user-images.githubusercontent.com/93282657/157837711-15f45c7c-6fd5-4f8c-b675-c88f66bcc589.png)
![Снимок экрана от 2022-03-11 12-07-28](https://user-images.githubusercontent.com/93282657/157837054-66e0c6e0-0e06-4b03-a7f1-44a4783700b2.png)
![Снимок экрана от 2022-03-11 12-07-37](https://user-images.githubusercontent.com/93282657/157837078-75cd0452-c09e-46c9-a81f-e2edd9baceef.png)
![Снимок экрана от 2022-03-11 12-07-45](https://user-images.githubusercontent.com/93282657/157837090-81b6e8bc-019e-4874-a034-0181efe982ee.png)

Всего одно предупреждение Per sequence GC content. Распределение слегка сдвинуто, но это не критично. Можно не редактировать файл.

## Таблица с статистикой

Образец | Кол-во ридов | выравнилось уникально | выравнилось НЕ-уникально |  НЕ выравнилось |
 --- |--- |--- |--- |---  
ENCFF000VIR | 26927551 | 1032269 (3.83%) | 3746410 (13.91%) | 22148872 (82.25%) |
ENCFF000VIP | 30482497 | 1021506 (3.35%) | 3092970 (10.15%) | 26368021 (86.50%) |
ENCFF000VJK | 41671673 | 1973730 (4.74%) | 9386141 (22.52%) | 30311802 (72.74%) |

Процент выравниваний  низкий. Вероятно, это из-за того, что выравнивание производилось только на одну хромосому и картировались те риды, что относятся к рассматриваемой хромосоме.


## Диаграммы Венна
![Снимок экрана от 2022-03-11 12-34-33](https://user-images.githubusercontent.com/93282657/157841324-84956ee5-d149-49f3-9dbc-f3b3340acadb.png)
![Снимок экрана от 2022-03-11 12-34-51](https://user-images.githubusercontent.com/93282657/157841323-a9e91641-2a16-45ce-b748-a92cb0a26743.png)
![Снимок экрана от 2022-03-11 12-35-09](https://user-images.githubusercontent.com/93282657/157841319-d8f2e288-505b-4e71-8a00-41e8b48a5b15.png)
![Снимок экрана от 2022-03-11 12-36-32](https://user-images.githubusercontent.com/93282657/157841312-e75be2e0-8906-4d35-8619-67135069e213.png)

Заметим, что пересечение довольно маленькое. Это можно объяснить тем, что у нас сначала было немного пиков из-за выравнивания всего на одну хромосому.
Количество пересечений различается при прямом и обратном сравнении. Сперва считается количество пиков в первом файле, что есть во втором. Затем считается количество пиков во втором файле, что есть в первом. 

