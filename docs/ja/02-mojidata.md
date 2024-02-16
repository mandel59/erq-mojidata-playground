# `mojidata` コマンドで遊ぶ

`mojidata` コマンドを使って遊んでみましょう。
`mojidata` コマンドは、漢字情報を検索して表示するコマンドです。

ターミナルを起動し、`cd`コマンドを使ってカレントディレクトリを変更してください。

- コマンド:  `cd erq-mojidata-playground`

プロンプトに `erq-mojidata-playground` と表示されたら、次のコマンドを入力してください。

- コマンド: `npx mojidata 漢字`

そうすると…

```
{"char":"漢","UCS":"U+6F22","aj1":{"CID":1533,"jp90":1533,"jp90_V":null,"jp04":1533,"jp04_V":null,"mac_jp90":1533,"mac_jp90_V":null,"mac_jp04":1533,"mac_jp04_V":null},"ids":[{"IDS":"⿰氵⿱廿⿻𠮡人","source":"GHKTV"},{"IDS":"⿰氵𦰩","source":"J"}],"ids_similar":[],"ids_comment":[],"ivs":[{"char":"漢󠄀","IVS":"6F22_E0100","collection":"Adobe-Japan1","code":"CID+1533"},{"char":"漢󠄁","IVS":"6F22_E0101","collection":"Adobe-Japan1","code":"CID+13332"},{"char":"漢󠄂","IVS":"6F22_E0102","collection":"Hanyo-Denshi","code":"JA2033"},{"char":"漢󠄃","IVS":"6F22_E0103","collection":"Hanyo-Denshi","code":"JC8705"},{"char":"漢󠄄","IVS":"6F22_E0104","collection":"Hanyo-Denshi","code":"KS552580"},{"char":"漢󠄅","IVS":"6F22_E0105","collection":"Hanyo-Denshi","code":"TK01051810"},{"char":"漢󠄆","IVS":"6F22_E0106","collection":"Hanyo-Denshi","code":"TK01051860"},{"char":"漢󠄂","IVS":"6F22_E0102","collection":"Moji_Joho","code":"MJ015841"},{"char":"漢󠄃","IVS":"6F22_E0103","collection":"Moji_Joho","code":"MJ030268"},{"char":"漢󠄇","IVS":"6F22_E0107","collection":"Moji_Joho","code":"MJ015842"}],"svs_cjkci":[{"SVS_char":"漢︀","SVS":"6F22_FE00","CJKCI_char":"漢","CJKCI":"U+FA47"},{"SVS_char":"漢︁","SVS":"6F22_FE01","CJKCI_char":"漢","CJKCI":"U+FA9A"}],"unihan":{"kHanYu":"31713.090","kIRGHanyuDaZidian":"31713.090","kIRGKangXi":"0646.170","kKangXi":"0646.170","kMorohashi":"18068' 18153:FE00 18068':E0102 18153:E0103","kCihaiT":"826.501","kSBGY":"401.50","kNelson":"2662 2665","kCowles":"1163","kMatthews":"2039","kGSR":"0144c","kFennIndex":"148.08","kKarlgren":"65","kSMSZD2003Index":"381.08","kMeyerWempe":"782","kLau":"1220","kDaeJaweon":"1055.150","kIRGDaeJaweon":"1055.150","kCangjie":"ETLO","kMojiJoho":"MJ015841 MJ030268:FE00 MJ015841:E0102 MJ030268:E0103 MJ015842:E0107","kPhonetic":"499A 546","kFenn":"107B","kUnihanCore2020":"HJKMPT","kFourCornerCode":"3413.4","kFrequency":"3","kGradeLevel":"4","kHKGlyph":"2291","kIRG_GSource":"G1-3A3A","kIRG_JSource":"J0-3441","kIRG_TSource":"T1-6947","kRSUnicode":"85.11","kTotalStrokes":"14","kIRG_KSource":"K0-7953","kIRG_KPSource":"KP0-F2D3","kIRG_VSource":"V1-5D3E","kIRG_HSource":"HB1-BA7E","kIICore":"ATJHKMP","kEACC":"4B4857","kTaiwanTelegraph":"3352","kBigFive":"BA7E","kCCCII":"214857","kCNS1986":"1-6947","kCNS1992":"1-6947","kGB1":"2626","kJis0":"2033","kJoyoKanji":"2010","kKoreanEducationHanja":"2007","kXerox":"243:330","kRSAdobe_Japan1_6":"C+1533+85.3.10","kCantonese":"hon3","kDefinition":"the Chinese people, Chinese language","kJapanese":"カン タン から","kMandarin":"hàn","kHanyuPinyin":"31713.090:hàn,tān","kXHC1983":"0441.041:hàn","kVietnamese":"hán","kSMSZD2003Readings":"hàn粵hon3","kHangul":"한:0E","kTang":"*xɑ̀n","kJapaneseKun":"KARA","kJapaneseOn":"KAN","kHanyuPinlu":"hàn(227)","kKorean":"HAN","kSimplifiedVariant":"U+6C49"},"unihan_fts":[["U+3D44","㵄","kDefinition","(same as 漢) name of a dynasty, belonging to China, the Milky Way the Han River, (interchangeable 域) a frontier; a boundary; a region; a country, to live; to stay"],["U+6C49","汉","kTraditionalVariant","U+6F22"],["U+FA47","漢","kCompatibilityVariant","U+6F22"],["U+FA47","漢","kJinmeiyoKanji","2010:U+6F22"],["U+FA9A","漢","kCompatibilityVariant","U+6F22"]],"unihan_variant":[["kSimplifiedVariant","U+6C49","汉"]],"unihan_variant_inverse":[["kCompatibilityVariant","U+FA47","漢"],["kCompatibilityVariant","U+FA9A","漢"],["kTraditionalVariant","U+6C49","汉"],["kJinmeiyoKanji","U+FA47","漢"]],"joyo":[{"音訓":"カン","例":["漢字","漢語","門外漢"],"備考":""}],"joyo_kangxi":["漢"],"joyo_kangxi_inverse":[],"doon":[],"nyukan":[{"正字の種類":"異体字","簡体字等の文字コード等":"3d44","簡体字等のUCS":"㵄","正字の文字コード等":"6f22","正字のUCS":"漢","順位":2},{"正字の種類":"異体字","簡体字等の文字コード等":"6c49","簡体字等のUCS":"汉","正字の文字コード等":"6f22","正字のUCS":"漢","順位":1}],"tghb":[{"序号":"0311","规范字":"汉","级":1,"笔画":5,"註解":null,"异体字":[{"繁体字":"漢","异体字":"漢","註解":null}]}],"mji":[{"文字":"漢","MJ文字図形名":"MJ015841","対応するUCS":"U+6F22","実装したUCS":"U+6F22","実装したMoji_JohoコレクションIVS":"6F22_E0102","実装したSVS":null,"戸籍統一文字番号":"203690","住基ネット統一文字コード":"J+6F22","入管正字コード":"0x6F22","入管外字コード":null,"漢字施策":"常用漢字","対応する互換漢字":null,"X0213":"1-20-33","X0213_包摂連番":null,"X0213_包摂区分":0,"X0212":null,"MJ文字図形バージョン":"1","登記統一文字番号":"00203690","部首・内画数":[[85,10]],"総画数":13,"読み":["カン","タン","から"],"大漢和":"18068'","日本語漢字辞典":6258,"新大字典":8694,"大字源":5145,"大漢語林":6170,"更新履歴":["Ver.006.02 「大漢和」親字番号の誤りを修正"],"備考":null,"mjsm":[["JIS包摂規準UCS統合規則","U+6F22","漢"]]},{"文字":"漢󠄇","MJ文字図形名":"MJ015842","対応するUCS":"U+6F22","実装したUCS":null,"実装したMoji_JohoコレクションIVS":"6F22_E0107","実装したSVS":null,"戸籍統一文字番号":"552580","住基ネット統一文字コード":null,"入管正字コード":null,"入管外字コード":null,"漢字施策":null,"対応する互換漢字":null,"X0213":null,"X0213_包摂連番":null,"X0213_包摂区分":null,"X0212":null,"MJ文字図形バージョン":"2","登記統一文字番号":"00552580","部首・内画数":[[85,11]],"総画数":14,"読み":["カン","タン"],"大漢和":null,"日本語漢字辞典":null,"新大字典":null,"大字源":null,"大漢語林":null,"更新履歴":["Ver.002.01 「MJ文字図形バージョン」を変更","Ver.002.01  「UCS対応カテゴリー」をA4に変更","Ver.005.02  「大漢和」を削除"],"備考":null,"mjsm":[["JIS包摂規準UCS統合規則","U+FA47","漢"]]},{"文字":"漢︀","MJ文字図形名":"MJ030268","対応するUCS":"U+6F22","実装したUCS":"U+FA47","実装したMoji_JohoコレクションIVS":"6F22_E0103","実装したSVS":"6F22_FE00","戸籍統一文字番号":"204710","住基ネット統一文字コード":"J+FA48","入管正字コード":"0xFA47","入管外字コード":null,"漢字施策":"人名用漢字","対応する互換漢字":"U+FA47","X0213":"1-87-05","X0213_包摂連番":null,"X0213_包摂区分":0,"X0212":null,"MJ文字図形バージョン":"1","登記統一文字番号":"00204710","部首・内画数":[[85,11]],"総画数":14,"読み":["カン","タン"],"大漢和":18153,"日本語漢字辞典":6259,"新大字典":8813,"大字源":5194,"大漢語林":6171,"更新履歴":["Ver.003.01 「対応するUCS」を変更","Ver.005.02  「実装したMoji_JohoIVS」を追加","Ver.006.02 「font」のUCSを「実装したUCS」に変更"],"備考":null,"mjsm":[["戸籍統一文字情報_親字正字","U+6F22","漢"],["JIS包摂規準UCS統合規則","U+FA47","漢"]]}],"mjsm_inverse":[{"表":"JIS包摂規準UCS統合規則","文字":"漢","MJ文字図形名":"MJ015841","対応するUCS":"U+6F22","実装したUCS":"U+6F22","実装したMoji_JohoコレクションIVS":"6F22_E0102","実装したSVS":null},{"表":"法務省告示582号別表第四_一","文字":"㵄","MJ文字図形名":"MJ002157","対応するUCS":"U+3D44","実装したUCS":"U+3D44","実装したMoji_JohoコレクションIVS":null,"実装したSVS":null},{"表":"戸籍統一文字情報_親字正字","文字":"㵄","MJ文字図形名":"MJ002157","対応するUCS":"U+3D44","実装したUCS":"U+3D44","実装したMoji_JohoコレクションIVS":null,"実装したSVS":null},{"表":"戸籍統一文字情報_親字正字","文字":"漢︀","MJ文字図形名":"MJ030268","対応するUCS":"U+6F22","実装したUCS":"U+FA47","実装したMoji_JohoコレクションIVS":"6F22_E0103","実装したSVS":"6F22_FE00"},{"表":"戸籍統一文字情報_親字正字","文字":"𣶔","MJ文字図形名":"MJ039359","対応するUCS":"U+23D94","実装したUCS":"U+23D94","実装したMoji_JohoコレクションIVS":null,"実装したSVS":null},{"表":"戸籍統一文字情報_親字正字","文字":"𤁉","MJ文字図形名":"MJ039676","対応するUCS":"U+24049","実装したUCS":"U+24049","実装したMoji_JohoコレクションIVS":null,"実装したSVS":null}],"mjih":[],"kdpv":{"cjkvi/simplified":["汉"],"hydzd/simplified":["汉"],"hydzd/variant":["㵄","𣶔","𤁉"],"jinmei2/variant":["漢"],"jisx0213/variant":["漢"],"joyo/variant":["漢"],"jp/new-style":["漢󠄀"],"jp/old-style":["漢󠄁"],"jp/old-style/compat":["漢"],"koseki/proper":["漢"],"koseki/variant":["漢"],"twedu/variant":["㵄","𣶔","𤁉"],"~cjkvi/traditional":["汉"]}}
{"char":"字","UCS":"U+5B57","aj1":{"CID":2248,"jp90":2248,"jp90_V":null,"jp04":2248,"jp04_V":null,"mac_jp90":2248,"mac_jp90_V":null,"mac_jp04":2248,"mac_jp04_V":null},"ids":[{"IDS":"⿱宀子","source":"GHJKTV"}],"ids_similar":[],"ids_comment":[],"ivs":[{"char":"字󠄀","IVS":"5B57_E0100","collection":"Adobe-Japan1","code":"CID+2248"}],"svs_cjkci":[],"unihan":{"kHanYu":"21010.020","kIRGHanyuDaZidian":"21010.020","kIRGKangXi":"0277.180","kKangXi":"0277.180","kMorohashi":"06942","kCihaiT":"398.103","kSBGY":"357.13","kNelson":"1281","kCowles":"4672","kMatthews":"6942","kGSR":"0964n","kFennIndex":"586.02 587.01","kSMSZD2003Index":"163.06 166.09","kMeyerWempe":"3536","kLau":"1446","kDaeJaweon":"0545.070","kIRGDaeJaweon":"0545.070","kCangjie":"JND","kMojiJoho":"MJ010057","kPhonetic":"134 147","kFenn":"112A","kUnihanCore2020":"GHJKMPT","kFourCornerCode":"3040.7","kFrequency":"2","kGradeLevel":"1","kHKGlyph":"0974","kIRG_GSource":"G0-5756","kIRG_JSource":"J0-3B7A","kIRG_TSource":"T1-4773","kRSUnicode":"39.3","kTotalStrokes":"6","kIRG_KSource":"K0-6D2E","kIRG_KPSource":"KP0-E6AF","kIRG_VSource":"V1-523E","kIRG_HSource":"HB1-A672","kIICore":"AGTJHKMP","kTGH":"2013:548","kEACC":"213A52","kTaiwanTelegraph":"1316","kBigFive":"A672","kCCCII":"213A52","kCNS1986":"1-4773","kCNS1992":"1-4773","kGB0":"5554","kGB1":"5554","kJis0":"2790","kJoyoKanji":"2010","kKoreanEducationHanja":"2007","kMainlandTelegraph":"1316","kXerox":"242:041","kRSAdobe_Japan1_6":"C+2248+39.3.3 C+2248+40.3.3","kCantonese":"zi6","kDefinition":"letter, character, word","kJapanese":"ジ シ あざ あざな やしなう","kMandarin":"zì","kHanyuPinyin":"21010.020:zì","kTGHZ2013":"492.140:zì","kXHC1983":"1533.040:zì","kVietnamese":"tự","kSMSZD2003Readings":"zì粵zi6","kHangul":"자:0E","kTang":"*dzhiə̀ dzhiə̀","kJapaneseKun":"AZA UMU MASU","kJapaneseOn":"JI","kHanyuPinlu":"zì(676) zi(138)","kKorean":"CA"},"unihan_fts":[],"unihan_variant":[],"unihan_variant_inverse":[],"joyo":[{"音訓":"ジ","例":["字画","文字","活字"],"備考":""},{"音訓":"あざ","例":["字","大字"],"備考":""}],"joyo_kangxi":[],"joyo_kangxi_inverse":[],"doon":[],"nyukan":[],"tghb":[{"序号":"0548","规范字":"字","级":1,"笔画":6,"註解":null,"异体字":[]}],"mji":[{"文字":"字","MJ文字図形名":"MJ010057","対応するUCS":"U+5B57","実装したUCS":"U+5B57","実装したMoji_JohoコレクションIVS":null,"実装したSVS":null,"戸籍統一文字番号":"078970","住基ネット統一文字コード":"J+5B57","入管正字コード":"0x5B57","入管外字コード":null,"漢字施策":"常用漢字","対応する互換漢字":null,"X0213":"1-27-90","X0213_包摂連番":null,"X0213_包摂区分":0,"X0212":null,"MJ文字図形バージョン":"1","登記統一文字番号":"00078970","部首・内画数":[[39,3],[40,3]],"総画数":6,"読み":["ジ","シ","あざ","あざな","やしなう"],"大漢和":6942,"日本語漢字辞典":2492,"新大字典":3396,"大字源":2042,"大漢語林":2447,"更新履歴":[],"備考":null,"mjsm":[["JIS包摂規準UCS統合規則","U+5B57","字"]]}],"mjsm_inverse":[{"表":"JIS包摂規準UCS統合規則","文字":"字","MJ文字図形名":"MJ010057","対応するUCS":"U+5B57","実装したUCS":"U+5B57","実装したMoji_JohoコレクションIVS":null,"実装したSVS":null},{"表":"戸籍統一文字情報_親字正字","文字":"𡥜","MJ文字図形名":"MJ033883","対応するUCS":"U+2195C","実装したUCS":"U+2195C","実装したMoji_JohoコレクションIVS":null,"実装したSVS":null},{"表":"戸籍統一文字情報_親字正字","文字":"𥤪","MJ文字図形名":"MJ043386","対応するUCS":"U+2592A","実装したUCS":"U+2592A","実装したMoji_JohoコレクションIVS":null,"実装したSVS":null},{"表":"辞書類等による関連字","文字":"𡥜","MJ文字図形名":"MJ033883","対応するUCS":"U+2195C","実装したUCS":"U+2195C","実装したMoji_JohoコレクションIVS":null,"実装したSVS":null},{"表":"辞書類等による関連字","文字":"𥤪","MJ文字図形名":"MJ043386","対応するUCS":"U+2592A","実装したUCS":"U+2592A","実装したMoji_JohoコレクションIVS":null,"実装したSVS":null}],"mjih":[],"kdpv":{"hydzd/variant":["𡥜","𥤪"],"koseki/variant":["𡥜","𥤪"],"non-cjk/square":["🈑"],"sawndip/regular":["只"],"twedu/variant":["𡥜","𥤪"]}}
```

…という感じで、漢字のデータが大量に！！！表示されます。ちょっと怖いぐらいに。

よく見ると、文字の読み方とか、部首とか、筆画数とか、いろいろな情報が表示されていますね。

`mojidata` コマンドは、渡した文字のデータを、JSON形式で表示します。複数の文字を渡した場合は、データを順番に1行ずつ表示します。

これでも使えるのですが、`jq` コマンドを使って、出力をもう少し見やすくしてみましょう。

- コマンド: `npx mojidata 漢字 | jq`

```json
{
  "char": "漢",
  "UCS": "U+6F22",
  "aj1": {
    "CID": 1533,
    "jp90": 1533,
    "jp90_V": null,
    "jp04": 1533,
    "jp04_V": null,
    "mac_jp90": 1533,
    "mac_jp90_V": null,
    "mac_jp04": 1533,
    "mac_jp04_V": null
  },
  "ids": [
    {
      "IDS": "⿰氵⿱廿⿻𠮡人",
      "source": "GHKTV"
    },
    {
...省略...
```

…という感じで、項目ごとに改行されて、少しだけ見やすくなりました。

## 項目を抜き出してみる

次に、文字と、その文字コード（UCS）だけを抜き出してみます。
先ほどのデータの先頭を見てください。

```json
{
  "char": "漢",
  "UCS": "U+6F22",
```

文字のキー（項目名）は `char` で、文字コードのキーは `UCS` になっていますね。
このキーを使って、項目を抜き出すことができます。


- コマンド: `npx mojidata 漢字 | jq '[.char, .UCS]'`

```json
[
  "漢",
  "U+6F22"
]
[
  "字",
  "U+5B57"
]
```

あるいは、出力にもキーをつけることができます。

- コマンド: `npx mojidata 漢字 | jq '{"文字": .char, "文字コード": .UCS}'`

```json
{
  "文字": "漢",
  "文字コード": "U+6F22"
}
{
  "文字": "字",
  "文字コード": "U+5B57"
}
```

1文字1行にするときは、`-c` オプションを使います。

- コマンド: `npx mojidata 漢字 | jq -c '{"文字": .char, "文字コード": .UCS}'`

```json
{"文字":"漢","文字コード":"U+6F22"}
{"文字":"字","文字コード":"U+5B57"}
```

## 深い項目を抜き出してみる

Unihanのデータから、読みを抜き出してみましょう。

深い項目は、キーを `.` でつなげて指定します。

- コマンド: `npx mojidata 漢字 | jq -c '[.char, .UCS, .unihan.kJapanese]'`

```json
["漢","U+6F22","カン タン から"]
["字","U+5B57","ジ シ あざ あざな やしなう"]
```

注意として、キーに漢字や記号など、英数字とアンダースコア（`_`）以外の文字が入っているときは、`[""]`で囲む必要があります。

- コマンド: `npx mojidata 漢字 | jq -c '[.char, .UCS, .kdpv.["cjkvi/simplified"]]'`

```json
["漢","U+6F22",["汉"]]
["字","U+5B57",null]
```

`jq` コマンドのもっと高度な使い方を知りたければ、[jq Manual](https://jqlang.github.io/jq/manual/)を読んでみてください。（このマニュアルは英語版なので、日本語版は検索するなどして適宜探してください。）
