# Play with `ids-find` command

Let's play with the `ids-find` command!

The `ids-find` command searches for kanji by Ideographic Description Sequence (IDS).

Start the terminal and use the `cd` command to change the current directory.

- Command: `cd erq-mojidata-playground`

When the prompt displays `erq-mojidata-playground`, enter the following command.

- Command: `npx ids-find 鬼`

Then...

```
傀塊媿嵬巍廆愧槐櫆溾犩瑰瘣磈聭蒐藱蘶螝褢謉醜隗餽騩鬼鬽鬾鬿魀魁魂魃魄魅魆魇魈魉魊魋魌魍魎魏魐魑魒魓魔魕魖魗魘魙㟴㠕㠢㱱䁛䃬䈭䌆䕇䫥䭳䰟䰠䰡䰢䰣䰤䰥䰦䰧䰨䰩䰪䰫䰬䰭䰮䰯䰰䰱䴜𠎺𠏁𠐤𠑖𠺌𠿯𡂃𡄬𡓮𡦶𡳺𡾖𡾛𡾵𡾾𡿁𡿆𢄊𢋝𢡨𢢯𢣒𢧩𢶟𢶼𢷪𢹧𣉨𣝂𣝹𣰏𤀖𤁔𤄛𤌋𤐜𤐡𤗧𤛂𤛲𤜋𤜘𤩫𤪿𤫅𤮞𤮟𥋳𥖸𥗶𥡂𥣼𥴯𥶯𥶱𦓌𦞙𦞱𦢮𧀐𧁩𧃝𧕞𧝛𧥇𧪵𧫏𧭵𧮊𧮓𧷛𨇷𨉵𨍹𨝀𨣫𨪈𩌃𩏐𩏳𩙢𩥢𩪁𩱹𩱺𩱻𩱼𩱽𩱾𩱿𩲀𩲁𩲂𩲃𩲄𩲅𩲇𩲈𩲉𩲊𩲋𩲌𩲍𩲎𩲏𩲐𩲑𩲒𩲓𩲔𩲕𩲖𩲗𩲘𩲙𩲚𩲛𩲜𩲝𩲞𩲟𩲠𩲡𩲢𩲣𩲤𩲥𩲦𩲧𩲨𩲩𩲪𩲫𩲬𩲭𩲮𩲯𩲰𩲱𩲲𩲳𩲴𩲵𩲶𩲷𩲸𩲹𩲺𩲻𩲼𩲽𩲾𩲿𩳀𩳁𩳂𩳃𩳄𩳅𩳆𩳇𩳈𩳉𩳊𩳋𩳌𩳍𩳎𩳏𩳐𩳑𩳒𩳓𩳔𩳕𩳖𩳗𩳘𩳙𩳚𩳛𩳜𩳝𩳞𩳟𩳠𩳡𩳢𩳣𩳤𩳥𩳦𩳧𩳨𩳩𩳪𩳫𩳬𩳭𩳮𩳯𩳰𩳱𩳲𩳳𩳴𩳵𩳶𩳷𩳸𩳹𩳺𩳻𩳼𩳽𩳾𩳿𩴀𩴁𩴂𩴃𩴄𩴅𩴆𩴇𩴈𩴉𩴊𩴋𩴌𩴍𩴎𩴏𩴐𩴑𩴒𩴓𩴔𩴕𩴖𩴗𩴘𩴙𩴚𩴛𩴜𩴝𩴞𩴟𩴠𩴡𩴢𩴣𩴤𩴥𩴦𩴧𩴨𩴩𩴪𩴬𩴭𩴮𩴯𩴱𩴲𩴳𩴴𩴵𩴶𩴷𩴸𩴹𩴺𩴻𩴼𩴽𩴾𩴿𩵀𩵁𩵂𩵃𩵄𩵅𩵆𩵇𩵈𩵉𩵊𩹷𩽤𪄔𪇋𪇫𪊃𪋺𪖾𪧄𪩜𪻆𫀢𫁖𫍷𫙈𫙉𫙊𫙋𫙌𫙍𫙎𫴒𫸄𫻣𬞴𬤱𬨐𬬖𬴽𬴾𬴿𬵙𬵲𭀸𭔉𭕩𭕼𭗪𭡏𭤞𭻻𮓀𮗙𮫝𮫞𮫟𮫠𮫡𮫣𮫤𮫥𮫦𮫧𮫨𮫩𮫪𮫫𮭺𰳒𰷨𱅡𱆖𱆗𱆘𱆙𱆚𱆛𱆜𱆝𱆞𱆟𱆠𱆡𱆢𱰑𱳆𱴹𲈔𲌧𲌨𲌩𲌪𲌫𲌬𲌮𲌯𲌰
```

A lot of kanji containing "鬼" were displayed!

If you got garbled characters, try installing a font. The following fonts are recommended.

- [IPAmj Mincho Font](https://moji.or.jp/mojikiban/font/)
- [Jigmo Font](https://kamichikoichi.github.io/jigmo/)
- [BabelStone Han](https://babelstone.co.uk/Fonts/Han.html)

> [!NOTE]
>
> I'm sorry, but even if you try hard to install fonts in a Windows environment, I don't think you can display all of them without garbling. Instead, try playing with the web version of [Mojidata Web App](https://mojidata.ryusei.dev/).

## Complex search

When you specify multiple kanji separated by spaces, it searches for kanji that contain all of them.

- Command: `npx ids-find 木 目 火`

```
瞅矁驦鷍鸘㸊䲚𢺱𣡲𤒟𤓥𥤛𥨽𧡣𧷂𩓮𩼱𩽓𪂼𪃥𪈈𪈎𪈐𮩦𱩃
```

When you specify an IDS, it searches for kanji that contain that IDS.

- Command: `npx ids-find ⿰日月`

```
奛奣擝明曌朚橗焽琞盟萌㿢䳟𠒫𠓓𡦀𡪙𡹌𢅆𢜏𢜠𢡗𢡰𢢤𣇴𣇵𣈂𣈇𣊧𣋐𣔂𣷠𤀄𤊉𥎒𥯋𦁠𦡉𦻽𧖽𧡜𧾆𨞚𨧹𨮠𨵛𩣶𪂡𪢣𪣦𪴞𪻪𫀹𫄁𬊚𬏾𬝡𬠫𬯿𭎮𭨽𮄱𰂚𰖫𱊂𱵗𱿋
```

Of course, you can specify multiple IDS. You can also search for kanji by combining kanji and IDS. (In fact, a single kanji itself is an IDS.)

- Command: `npx ids-find ⿰木目 水`

```
湘灀𩅪𪶛
```

You can search for kanji that have the shape of the specified IDS using the `--whole=` option. When combined with `？` (full-width question mark), you can search for kanji with the shape of a fish's radical "魚".

- Command: `npx ids-find --whole=⿰？魚`

```
漁龽䁩䐳䗨䲆𠽐𡐚𡠵𢐗𢠐𢳶𣊘𣩕𨢭𨫗𨫷𩥭𩵑𩵫𩶿𩸇𪫔𫙣𮃣𮬋𱆏𱜊𲍂
```

When you use the `*` (asterisk) character, you can search for kanji that contain the specified IDS multiple times.

- Command: `npx ids-find 木 耳＊３`

```
欇𣠞𥤋𬗂
```

This search does not work with `npx ids-find 木 耳 耳 耳`. With this specification, all kanji containing `木` and `耳` will be displayed. (This may be improved in future versions.)
