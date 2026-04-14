模擬臨床研究データセット

このCSVは「最初から解析用に完成したデータ」ではなく、生データを想定している。
以下について処理する必要がある。



・研究対象者の選択・除外

・欠損値の確認と処理

・性別や病棟区分などカテゴリ変数のダミー変数化

・ロジスティック回帰とランダムフォレストの比較

・結果の解釈



**アウトカム**

adverse\_event：対象薬投与後の有害事象発現（0/1）



**選択・除外の検討に使う列**

target\_drug\_use: A薬が実際に使用されたか否か（0/1）

followup\_days：観察日数

baseline\_same\_ae：投与開始前に同一有害事象があるか（0/1）

severe\_hepatic\_failure：重度肝障害（0/1）

pregnancy\_status：妊娠状態（No / Yes / Unknown / Not applicable）



**変数一覧**

patient\_id：患者ID

age：年齢

sex：性別（M/F）

pregnancy\_status：妊娠状態

ward\_type：病棟区分（Outpatient / General ward / ICU）

primary\_disease：主病名

target\_drug\_started：A薬使用の有無

followup\_days：観察日数

baseline\_same\_ae：投与開始前に同一有害事象があるか

severe\_hepatic\_failure：重度肝障害

BMI：BMI

eGFR：推算糸球体濾過量（腎機能の指標）

Albumin：アルブミン

AST：AST（肝機能の指標）

ALT：ALT（肝機能の指標）

comorbidity\_count：併存疾患の数

concomitant\_drugs\_count：併用薬の数

dose\_mg\_day：投与量（mg/day）

adverse\_event：有害事象発現（0/1）

adverse\_event\_grade：有害事象重症度

hospitalization\_days：入院日数

admission\_30d：A薬投与30日前の入院（0/1）

