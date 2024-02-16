# Erqで遊ぶ 基本編

Erqを使うと、漢字データベースを使っていろいろな検索や集計をすることができます。

ターミナルを起動し、`cd`コマンドを使ってカレントディレクトリを変更してください。

- コマンド: `cd erq-mojidata-playground`

プロンプトに `erq-mojidata-playground` と表示されたら、次のコマンドを入力してください。

- コマンド: `npx erq --init mojidata.erq`

そうすると…

```
Connected to :memory:
attach 'node_modules/@mandel59/mojidata/dist/moji.db' as moji
ok (0.003s)
erq>
```

Erqが起動し、クエリを入力することができるようになりました。

## クエリの書き方

クエリは、データベースに対して行う操作を指定するものです。

試しに、次のクエリを実行してみましょう。これは、データベースに保存されている表（テーブル）の一覧表を表示するクエリです。

- クエリ: `pragma_table_list;;`

そうすると…

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

こんなふうに表示されます！

最初に表示される

```sql
select * from pragma_table_list
```

は、Erqクエリに相当するSQLクエリです。これはとりあえず、無視して大丈夫です。

次に表示される

```json
["schema","name","type","ncol","wr","strict"]
```

は、表の列（カラム）名です。その次の行から、実際のデータが表示されます。

最後に、

```
203 rows (0.008s)
```

と、データの行（ロー）数と、クエリの実行時間が表示されます。

## 表の行数制限

Erqでは、表の名前につづけて `;;` を入力することで、その表のデータを表示することができます。
`;;` は、Erqのクエリの終わりを表します。

ところで、203行は長いですよね。これを制限するために、`limit` キーワードを使って、行数を制限することができます。

- クエリ: `pragma_table_list limit 5;;`

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

これで、表の最初の5行だけ表示されます。基本的に、クエリの最後に `limit 【行数】` と書くことで、行数を制限することができます。

## 表示を途中で止める

基本的には `limit` キーワードを使って行数を制限すると見やすいですが、`limit`キーワードを使わず表の全部を表示してしまうことがあると思います。そういうときは `Ctrl+C` を押すことで、表示を途中で止めることができます。

たとえば、次のクエリを実行してみてください。

- クエリ: `unihan;;`

この表は約147万行（1,477,210行）あります。これを全部表示しようとすると、かなり時間がかかります。そこで、`Ctrl+C` を押してみてください。

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

途中で表示が止まって `erq> ` というプロンプトが表示され、次のクエリを入力することができるようになりました。

## 表を検索する

表からデータを検索してみましょう。次のクエリは、表の名前が `mji` で始まる表の一覧を表示するクエリです。

- クエリ: `pragma_table_list [name glob "mji*"] limit 20;;`

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

表の一覧表が `pragma_table_list` でした。
その後にある `[name glob "mji*"]` は、`name`列の項目が `mji` で始まるという条件を指定しています。`*`はワイルドカードといって、任意の文字列を表します。つまり、`[name glob "mji*"]` なら `mji` で始まる任意の文字列にマッチするし、`[name glob "*mji"]` なら任意の文字列で終わる `mji` にマッチします。`mji`を含む、なら `[name glob "*mji*"]` と書けばいいです。

条件は複数指定することもできます。条件の間の空白は開けても開けなくても、改行をいれても大丈夫です。
たとえば「あげる」「ショウ」と読む漢字を検索するなら…

- クエリ: `unihan_kJapanese[value glob "*あげる*"][value glob "*ショウ*"] limit 20;;`

```
erq> unihan_kJapanese[value glob "*あげる*"][value glob "*ショウ*"] limit 20;;
select * from unihan_kJapanese where (value glob '*あげる*') and (value glob '*ショウ*') limit 20
["UCS","value"]
["上","ジョウ ショウ うえ うわ かみ あげる あがる のぼる のぼせる のぼす たっとぶ たてまつる ほとり"]
["称","ショウ あげる かなう たたえる となえる はかり はかる"]
2 rows (0.010s)
```

…こんな感じです！

これで、表を覗いて見たり、データを検索してみることができるようになりました。

> [!TIP]
>
> 表の名前に記号が入っている場合は、クエリ中の表の名前を ` `` ` で囲ってください。
> たとえば、`kdpv_cjkvi/simplified` の中身を見たいなら
> `` `kdpv_cjkvi/simplified` limit 20;; `` というクエリを書きます。
