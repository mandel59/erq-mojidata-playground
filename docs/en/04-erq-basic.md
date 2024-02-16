# Playing with Erq: Basic

With Erq, you can search and aggregate data using the kanji database.

Start the terminal and change the current directory to `erq-mojidata-playground`.

- Command: `cd erq-mojidata-playground`

When the prompt displays `erq-mojidata-playground`, enter the following command.

- Command: `npx erq --init mojidata.erq`

Then...

```
Connected to :memory:
attach 'node_modules/@mandel59/mojidata/dist/moji.db' as moji
ok (0.006s)
erq> 
```

Erq is now running and ready to accept queries!

## Writing queries

A query specifies the operation to be performed on the database.

Try running the following query. This query displays a list of tables in the database.

- Query: `pragma_table_list;;`

Then...

```
erq> pragma_table_list;;
select * from pragma_table_list
["schema","name","type","ncol","wr","strict"]
["main","sqlite_schema","table",5,0,0]
["temp","sqlite_temp_schema","table",5,0,0]
["moji","kdpv_rels","table",4,0,0]
["moji","kdpv_jisx0213/variant","table",3,0,0]
["moji","kdpv_hydzd/variant","table",3,0,0]
["moji","kdpv_twedu/variant","table",3,0,0]
["moji","kdpv_jp/borrowed","table",3,0,0]
["moji","kdpv_dypytz/variant/1993","table",3,0,0]
["moji","kdpv","view",4,0,0]
["moji","kdpv_non-cjk/kangxi","table",3,0,0]
["moji","kdpv_cjkvi/duplicate","table",3,0,0]
["moji","kdpv_non-cjk/kanbun","table",3,0,0]
["moji","kdpv_cjkvi/variant-simplified","table",3,0,0]
["moji","aj1_UniJISX0213_H","view",2,0,0]
["moji","ivs","view",3,0,0]
["moji","joyo_kangxi","table",2,0,0]
["moji","joyo_acceptable","table",1,0,0]
["moji","unihan_source","view",3,0,0]
["moji","kdpv_cjkvi/radical-split","table",3,0,0]
["moji","unihan_kSpecializedSemanticVariant","table",2,0,0]
["moji","kdpv_non-cjk/strokes","table",3,0,0]
["moji","unihan_kVietnamese","table",2,0,0]
["moji","aj1_UniJISX0213_V","view",2,0,0]
["moji","kdpv_cjkvi/simplified","table",3,0,0]
["moji","doon","table",5,0,0]
["moji","ids","table",3,0,0]
["moji","unihan_kSMSZD2003Readings","table",2,0,0]
["moji","unihan_kTGHZ2013","table",2,0,0]
["moji","unihan_kSpoofingVariant","table",2,0,0]
["moji","unihan_kMandarin","table",2,0,0]
["moji","aj1_UniJISX02132004_V","view",2,0,0]
["moji","kdpv_jinmei2/variant","table",3,0,0]
["moji","unihan_kDefinition","table",2,0,0]
["moji","kdpv_hyogai/variant","table",3,0,0]
["moji","unihan_kHanyuPinyin","table",2,0,0]
["moji","unihan_kCNS1986","table",2,0,0]
["moji","unihan_kCCCII","table",2,0,0]
["moji","kdpv_sawndip/variant","table",3,0,0]
["moji","unihan_kKoreanName","table",2,0,0]
["moji","unihan_kTGH","table",2,0,0]
["moji","unihan_kVietnameseNumeric","table",2,0,0]
["moji","tghb","table",5,0,0]
["moji","kdpv_jinmei1/variant","table",3,0,0]
["moji","kdpv_dypytz/variant/1997","table",3,0,0]
["moji","kdpv_cjkvi/traditional","table",3,0,0]
["moji","unihan_kXHC1983","table",2,0,0]
["moji","unihan_kIRG_VSource","table",2,0,0]
["moji","aj1_UniJIS2004_H","view",2,0,0]
["moji","kdpv_jp/old-style","table",3,0,0]
["moji","unihan_kHanyuPinlu","table",2,0,0]
["moji","unihan_kIRG_KSource","table",2,0,0]
["moji","kdpv_non-cjk/parenthesized","table",3,0,0]
["moji","unihan_kBigFive","table",2,0,0]
["moji","unihan_kJIS0213","table",2,0,0]
["moji","unihan_kRSUnicode","table",2,0,0]
["moji","kdpv_non-cjk/radical","table",3,0,0]
["moji","unihan_kIRG_TSource","table",2,0,0]
["moji","aj1_UniJISX02132004_H","view",2,0,0]
["moji","kdpv_non-cjk/bracketed","table",3,0,0]
["moji","nyukan_ruiji","table",5,0,0]
["moji","unihan_kJa","table",2,0,0]
["moji","unihan_kGradeLevel","table",2,0,0]
["moji","kdpv_cjkvi/variant","table",3,0,0]
["moji","unihan_kIRG_UKSource","table",2,0,0]
["moji","unihan_kFrequency","table",2,0,0]
["moji","unihan_kCheungBauer","table",2,0,0]
["moji","kdpv_cjkvi/pseudo-simplified","table",3,0,0]
["moji","unihan_kKorean","table",2,0,0]
["moji","unihan_kZhuangNumeric","table",2,0,0]
["moji","unihan_kFourCornerCode","table",2,0,0]
["moji","kdpv_jp/old-style/compat","table",3,0,0]
["moji","unihan_kTaiwanTelegraph","table",2,0,0]
["moji","unihan_kUnihanCore2020","table",2,0,0]
["moji","aj1_UniJIS_H","view",2,0,0]
["moji","unihan_kJis1","table",2,0,0]
["moji","unihan_kFenn","table",2,0,0]
["moji","kdpv_koseki/variant","table",3,0,0]
["moji","unihan_kJinmeiyoKanji","table",2,0,0]
["moji","unihan_kGB8","table",2,0,0]
["moji","unihan_kCangjie","table",2,0,0]
["moji","kdpv_cjkvi/numeric","table",3,0,0]
["moji","unihan_kTraditionalVariant","table",2,0,0]
["moji","unihan_kIRGDaeJaweon","table",2,0,0]
["moji","unihan_kCheungBauerIndex","table",2,0,0]
["moji","unihan_kGB5","table",2,0,0]
["moji","unihan_kKoreanEducationHanja","table",2,0,0]
["moji","unihan_kJoyoKanji","table",2,0,0]
["moji","unihan_kDaeJaweon","table",2,0,0]
["moji","unihan_kSMSZD2003Index","table",2,0,0]
["moji","aj1_UniJIS_V","view",2,0,0]
["moji","unihan_kOtherNumeric","table",2,0,0]
["moji","unihan_kHanYu","table",2,0,0]
["moji","mjsm_辞書類等による関連字","table",3,0,0]
["moji","unihan_kCowles","table",2,0,0]
["moji","unihan_kIRG_KPSource","table",2,0,0]
["moji","unihan_kMatthews","table",2,0,0]
["moji","kdpv_cjkvi/radical-variant","table",3,0,0]
["moji","kdpv_dypytz/variant","table",3,0,0]
["moji","unihan_kRSAdobe_Japan1_6","table",2,0,0]
["moji","unihan_kIRG_MSource","table",2,0,0]
["moji","unihan_kTotalStrokes","table",2,0,0]
["moji","unihan_kMojiJoho","table",2,0,0]
["moji","unihan_kFennIndex","table",2,0,0]
["moji","mjsm_民一2842号通達別表_誤字俗字正字一覧表_俗字","table",3,0,0]
["moji","mjsm_JIS包摂規準UCS統合規則","table",3,0,0]
["moji","kdpv_ucs-scs/variant","table",3,0,0]
["moji","kdpv_joyo/variant","table",3,0,0]
["moji","unihan_kGB3","table",2,0,0]
["moji","unihan_kEACC","table",2,0,0]
["moji","unihan_kIRG_JSource","table",2,0,0]
["moji","unihan_kGSR","table",2,0,0]
["moji","unihan_variant","view",4,0,0]
["moji","unihan_kGB1","table",2,0,0]
["moji","unihan_kIRG_HSource","table",2,0,0]
["moji","mji_changelog","table",2,0,0]
["moji","unihan","view",3,0,0]
["moji","kdpv_x0213-x0212/variants","table",3,0,0]
["moji","kdpv_cjkvi/non-cognate","table",3,0,0]
["moji","unihan_kXerox","table",2,0,0]
["moji","unihan_kJis0","table",2,0,0]
["moji","radeqv","table",2,0,0]
["moji","kdpv_hydzd/simplified","table",3,0,0]
["moji","aj1","table",7,0,0]
["moji","unihan_kZVariant","table",2,0,0]
["moji","unihan_kHangul","table",2,0,0]
["moji","unihan_kAlternateTotalStrokes","table",2,0,0]
["moji","mjsm_note","table",2,0,0]
["moji","aj1_UniJIS2004_V","view",2,0,0]
["moji","unihan_kSimplifiedVariant","table",2,0,0]
["moji","unihan_kIICore","table",2,0,0]
["moji","mjih","table",10,0,0]
["moji","ivs_Hanyo-Denshi","table",2,0,0]
["moji","joyo","table",4,0,0]
["moji","unihan_kJapaneseOn","table",2,0,0]
["moji","unihan_kStrange","table",2,0,0]
["moji","mjih_phonetic","table",3,0,0]
["moji","unihan_kIRGKangXi","table",2,0,0]
["moji","kdpv_dypytz/variant/1956","table",3,0,0]
["moji","mji","table",24,0,0]
["moji","mjsm_民二5202号通知別表_正字俗字等対照表","table",3,0,0]
["moji","kdpv_non-cjk/bopomofo","table",3,0,0]
["moji","unihan_kPrimaryNumeric","table",2,0,0]
["moji","unihan_kIRG_USource","table",2,0,0]
["moji","unihan_kHKGlyph","table",2,0,0]
["moji","ivs_Adobe-Japan1","table",2,0,0]
["moji","unihan_kCantonese","table",2,0,0]
["moji","unihan_kGB7","table",2,0,0]
["moji","unihan_kMainlandTelegraph","table",2,0,0]
["moji","unihan_kMeyerWempe","table",2,0,0]
["moji","sqlite_schema","table",5,0,0]
["moji","mji_reading","table",2,0,0]
["moji","mjsm_戸籍統一文字情報_親字正字","table",4,0,0]
["moji","kdpv_non-cjk/circle","table",3,0,0]
["moji","kdpv_dypytz/variant/1988","table",3,0,0]
["moji","mjsm_読み字形による類推","table",3,0,0]
["moji","kdpv_non-cjk/square","table",3,0,0]
["moji","kdpv_non-cjk/hangzhou-num","table",3,0,0]
["moji","unihan_kJapanese","table",2,0,0]
["moji","mjsm_民一2842号通達別表_誤字俗字正字一覧表_別字","table",3,0,0]
["moji","mjsm_法務省告示582号別表第四_一","table",4,0,0]
["moji","unihan_kIRGHanyuDaZidian","table",2,0,0]
["moji","kdpv_jisx0212/variant","table",3,0,0]
["moji","unihan_kAccountingNumeric","table",2,0,0]
["moji","ivs_MSARG","table",2,0,0]
["moji","kdpv_hydcd/borrowed","table",3,0,0]
["moji","kdpv_dypytz/variant/1986","table",3,0,0]
["moji","unihan_kKarlgren","table",2,0,0]
["moji","radicals","table",7,0,0]
["moji","mjsm","view",6,0,0]
["moji","unihan_kTang","table",2,0,0]
["moji","unihan_kPseudoGB1","table",2,0,0]
["moji","unihan_kPhonetic","table",2,0,0]
["moji","mjsm_民一2842号通達別表_誤字俗字正字一覧表_無印","table",3,0,0]
["moji","unihan_kMorohashi","table",2,0,0]
["moji","kdpv_non-cjk/katakana","table",3,0,0]
["moji","nyukan_itaiji","table",5,0,0]
["moji","unihan_kIBMJapan","table",2,0,0]
["moji","unihan_kHDZRadBreak","table",2,0,0]
["moji","unihan_kLau","table",2,0,0]
["moji","mji_duplicated_ivs","table",2,0,0]
["moji","ivs_KRName","table",2,0,0]
["moji","nyukan","view",6,0,0]
["moji","unihan_kSemanticVariant","table",2,0,0]
["moji","unihan_kIRG_GSource","table",2,0,0]
["moji","usource","table",9,0,0]
["moji","unihan_strange","view",3,0,0]
["moji","unihan_kGB0","table",2,0,0]
["moji","unihan_kCNS1992","table",2,0,0]
["moji","mjsm_法務省告示582号別表第四_二","table",4,0,0]
["moji","usource_source","table",2,0,0]
["moji","kdpv_cjkvi/radical-variant-simplified","table",3,0,0]
["moji","ivs_Moji_Joho","table",2,0,0]
["moji","svs_cjkci","table",2,0,0]
["moji","unihan_kKangXi","table",2,0,0]
["moji","unihan_kCihaiT","table",2,0,0]
["moji","ids_comment","table",2,0,0]
["moji","unihan_kJapaneseKun","table",2,0,0]
["moji","unihan_kIRG_SSource","table",2,0,0]
["moji","unihan_kSBGY","table",2,0,0]
["moji","tghb_variants","table",5,0,0]
["moji","unihan_kCompatibilityVariant","table",2,0,0]
["moji","mji_rsindex","table",3,0,0]
["moji","unihan_kNelson","table",2,0,0]
203 rows (0.008s)
```

You can see a list of tables in the database!

The first line of the output is equivalent query in SQL. You can ignore it for now.

```sql
select * from pragma_table_list
```

The second line is the column names of the table. The rest of the output is the data in the table.

```json
["schema","name","type","ncol","wr","strict"]
```

The last line shows the number of rows and the time it took to execute the query.

```
203 rows (0.008s)
```

## Limiting the number of rows

In Erq, you can display the data in a table by write the name of the table followed by `;;`. `;;` indicates the end of the query.

By the way, 203 rows is a bit long. To limit the number of rows, you can use the `limit` keyword.

- Query: `pragma_table_list limit 5;;`

```
erq> pragma_table_list limit 5;;
select * from pragma_table_list limit 5
["schema","name","type","ncol","wr","strict"]
["main","sqlite_schema","table",5,0,0]
["temp","sqlite_temp_schema","table",5,0,0]
["moji","kdpv_rels","table",4,0,0]
["moji","kdpv_jisx0213/variant","table",3,0,0]
["moji","kdpv_hydzd/variant","table",3,0,0]
5 rows (0.001s)
```

This will display only the first 5 rows of the table. Basically, you can limit the number of rows by writing `limit 【number of rows】` at the end of the query.

## Stopping the display in the middle

Basically, it's easier to limit the number of rows with the `limit` keyword, but sometimes you may want to display the entire table without using the `limit` keyword. In that case, you can stop the display in the middle by pressing `Ctrl+C`.

For example, try running the following query.

- クエリ: `unihan;;`

The table `unihan` has about 1.47 million rows. It's a bit long to display all at once. Now try pressing `Ctrl+C`.

```
["𢧽","kIRGHanyuDaZidian","21411.090"]
["𢧾","kIRGHanyuDaZidian","21411.140"]
["𢧿","kIRGHanyuDaZidian","21411.150"]
["𢨀","kIRGHanyuDaZidian","21412.020"]
["𢨁","kIRGHanyuDaZidian","21412.060"]
["𢨂","kIRGHanyuDaZidian","21412.070"]
["𢨇","kIRGHanyuDaZidian","21412.110"]
["𢨈","kIRGHanyuDaZidian","21413.040"]
["𢨉","kIRGHanyuDaZidian","21413.030"]
["𢨊","kIRGHanyuDaZidian","21413.060"]
["𢨋","kIRGHanyuDaZidian","21412.100"]
["𢨌","kIRGHanyuDaZidian","21413.080"]
["𢨍","kIRGHanyuDaZidian","21413.020"]
["𢨎","kIRGHanyuDaZidian","21412.080"]
["𢨏","kIRGHanyuDaZidian","21412.090"]
["𢨐","kIRGHanyuDaZidian","21413.010"]
["𢨑","kIRGHanyuDaZidian","21413.050"]
["𢨒","kIRGHanyuDaZidian","21413.070"]
["𢨓","kIRGHanyuDaZidian","21414.020"]
["𢨔","kIRGHanyuDaZidian","21414.010"]
["𢨖","kIRGHanyuDaZidian","21413.100"]
["𢨗","kIRGHanyuDaZidian","21413.120"]
["𢨚","kIRGHanyuDaZidian","21414.050"]
Interrupted
89800 rows (0.908s)
erq> 
```

The output stopped in the middle, and the prompt `erq> ` was displayed, allowing you to enter the next query.

## Searching a table

Let's search for data in a table.
The following query displays a list of tables whose names start with `mji`.

- Query: `pragma_table_list [name glob "mji*"] limit 20;;`

```
erq> pragma_table_list [name glob "mji*"] limit 20;;
select * from pragma_table_list where (name glob 'mji*') limit 20
["schema","name","type","ncol","wr","strict"]
["moji","mji_changelog","table",2,0,0]
["moji","mjih","table",10,0,0]
["moji","mjih_phonetic","table",3,0,0]
["moji","mji","table",24,0,0]
["moji","mji_reading","table",2,0,0]
["moji","mji_duplicated_ivs","table",2,0,0]
["moji","mji_rsindex","table",3,0,0]
7 rows (0.001s)
```

The list of tables is `pragma_table_list`.
After that, `[name glob "mji*"]` specifies the condition that the `name` column starts with `mji`. `*` is a wildcard that represents any string. So `[name glob "mji*"]` matches any string that starts with `mji`, and `[name glob "*mji"]` matches any string that ends with `mji`. If you want to match any string that contains `mji`, you can write `[name glob "*mji*]`.

You can specify multiple conditions. You can put spaces between conditions, or you can put line breaks between conditions.

For example, to search for kanji that can be read as "あげる" and "ショウ"...

- Query: `unihan_kJapanese[value glob "*あげる*"][value glob "*ショウ*"] limit 20;;`

```
erq> unihan_kJapanese[value glob "*あげる*"][value glob "*ショウ*"] limit 20;;
select * from unihan_kJapanese where (value glob '*あげる*') and (value glob '*ショウ*') limit 20
["UCS","value"]
["上","ジョウ ショウ うえ うわ かみ あげる あがる のぼる のぼせる のぼす たっとぶ たてまつる ほとり"]
["称","ショウ あげる かなう たたえる となえる はかり はかる"]
2 rows (0.010s)
```

...like this!

Now you can peek at tables and search for data.

> [!TIP]
>
> If the table name contains symbols, enclose the table name in ` `` ` in the query.
> For example, if you want to see the contents of `kdpv_cjkvi/simplified`, write the query `` `kdpv_cjkvi/simplified` limit 20;; ``.
