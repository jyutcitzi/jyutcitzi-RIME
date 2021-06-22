# jyutcitzi-RIME
![GitHub last commit](https://img.shields.io/github/last-commit/jyutcitzi/jyutcitzi-RIME.svg) ![GitHub](https://img.shields.io/github/license/jyutcitzi/jyutcitzi-RIME.svg)  
配方: ℞ **jyutcitzi/jyutcitzi-RIME**

其他 README 版本：香港粵語（[漢字](README.yue-hk.honzi.md)，[漢字粵切字](README.yue-hk.honzi-jcz.md)）| [英語](README.md)

一個用嚟實現漢字粵切字混寫嘅 RIME 鍵盤  
多謝支持粵切字嘅鍵盤同字體！下面會講點樣去安裝同用呢個鍵盤，最尾呢就會有個 FAQ section：  
1. [安裝步驟](#安裝步驟)  
2. [鍵盤特徵](#鍵盤特徵)
3. [常見問題](#常見問題)
4. [軟件更新](#軟件更新)  

![Cover Picture](https://github.com/jyutcitzi/jyutcitzi-RIME/blob/d5f0104ab5d2a111f9dc2a0ffa511709fb88f83e/images/cover_picture.png)

## 安裝步驟
### 第一步：裝 RIME 同 RIME Cantonese
唔該去 https://github.com/rime/rime-cantonese/wiki 同 https://github.com/rime/rime-cantonese/wiki/新手安裝教程 ，跟住嗰度啲步驟  
簡單啲嚟講，即係 download 同 install 依啲 file：  
Mac: [mac-2021.05.16-installer.pkg](https://github.com/rime/rime-cantonese/releases/download/2021.05.16/mac-2021.05.16-installer.pkg)  
Windows: [windows-sfx-2021.05.16-installer.exe](https://github.com/rime/rime-cantonese/releases/download/2021.05.16/windows-sfx-2021.05.16-installer.exe)  
Linux: Download 同 run [ibus-install.sh](https://github.com/rime/rime-cantonese/releases/download/2021.05.16/ibus-install.sh)  
安裝要成功咗先至可以去第三步。  

### 第二步：裝粵切字字體
1. 去 https://github.com/jyutcitzi/jyutcitzi-fonts download 晒啲粵切字字體  
2. 安裝字體  
Mac：用字體簿（Font Book）開咗先，跟住㩒「安裝」  
Windows：Right-click 個 TTF file，跟住揀「安裝」  
Linux：上網 google 「點樣喺**你用緊嘅Linux distro**安裝字體」  

做呢步嘅目的就係為咗可以顯示啲粵切字。字體嚟講， PMingLiU（標準字重）, SourceHanSerifTC（全部字重）and SourceHanSansHC（全部字重）呢啲字體冚唥都係增加咗粵切字嘅。至於SourceHanSansHWHC（全部字重）呢就淨係得粵切字，係冇漢字嘅。

### 第三部：安裝網上同字體版嘅粵切字鍵盤
#### Mac 呢就要：
   a. 喺 mon 頂嘅輸入法 menu 度揀有【ㄓ】icon 嘅「鼠鬚管」  
   b. 㩒「設定…」。㩒完應該會彈咗個 Finder window 出嚟。  
   c. 將啲 YAML 文件 copy and paste 落去個 RIME folder 入面。  
   d. 喺輸入法 menu度再揀「鼠鬚管」輸入法，跟住㩒「重新部署」  
   e. 等啲鍵盤 load（畀啲耐性！）  
   f. 㩒 F4 或者 CTRL + \` 嚟轉換到「粵切字 (禾旡·比\`·版)」（即網版鍵盤）或者「粵切字 (夫干·天\`·版)」（即字體版鍵盤）。  
   g. 噉就可以用倒個鍵盤㗎喇。  

#### Windows 呢就要：
   a. 㩒 Windows 掣，跟住輸入 %AppData%\Rime 同㩒 ENTER。  
   b. 將啲 YAML 文件 copy and paste 落去個 RIME folder 入面。  
   c. 喺 start menu 揾同開始 「【小狼毫】重新部署」  
   d. 等啲鍵盤 load（畀啲耐性！）  
   e. 㩒 F4 或者 CTRL + \` 嚟轉換到「粵切字 (禾旡·比\`·版)」（即網版鍵盤）或者「粵切字 (夫干·天\`·版)」（即字體版鍵盤）。  
   f. 噉就可以用倒個鍵盤㗎喇。  

## 文件描述
- **default.custom.yaml** - 嚟指明要用邊啲 RIME 鍵盤（即係RIME Cantonese同粵切字鍵盤）嘅config file
- **squirrel.custom.yaml** - 嚟指明RIME 嘅介面所用嘅字體（要呢個文件先至可以揀字嗰陣顯示到啲粵切字）
- **jyutcitzi_font.schema.yaml** - 字體版鍵盤嘅 config file
- **jyutcitzi_web.schema.yaml** - 網版鍵盤嘅 config file 
- **jyutcitzi_font.dict.yaml** - 字體版鍵盤嘅主要字典，含有好多唔同單音節網版粵切字
- **jyutcitzi_web.dict.yaml** - 網版鍵盤嘅主要字典，含有好多唔同單音節網版粵切字
- **jyutcitzi_core.lettered.dict.yaml** - 原本嚟自 jyut6ping3.lettered.dict.yaml
- **jyutcitzi_font.lettered.dict.yaml** - 一個顯示字體版粵切字而含拉丁字嘅粵語字典
- **jyutcitzi_web.lettered.dict.yaml** - 一個顯示網版粵切字而含拉丁字嘅粵語字典
- **jyutcitzi_font.compound.dict.yaml** - 一個顯示字體版粵切字嘅粵語詞語嘅字典  
- **jyutcitzi_web.compound.dict.yaml** - 一個顯示網版粵切字嘅粵語詞語嘅字典  
- **jyutcitzi_font.phrase.dict.yaml** - 一個顯示字體版粵切字嘅粵語組詞字典  
- **jyutcitzi_web.phrase.dict.yaml** - 一個顯示網版粵切字嘅粵語組詞字典  
- **jyutcitzi.jyutcit_phrases.dict.yaml** - 一個含有選自粵切字文學嘅字句嘅字典  
- **mapping.txt** - 一 list Unicode數字同佢哋所對應嘅粵切字同改革漢字  

## 鍵盤特徵
   0. 如果個鍵盤有問題可以㩒 CTRL + OPTION + \` 嚟重新部署，再唔得可以 restart 部電腦。  
   1. 轉換鍵盤可以㩒 F4 或者 CTRL + \` (即係ESC隔離嗰個掣)  
   2. 拉丁字同漢字粵切字鍵盤之間嘅轉換可以㩒 SHIFT 或者 CAPS LOCK
   3. 打字嗰陣為咗方便可以省略聲調，如果要標調嘅話可以噉樣打：  
	![RIME入面標調](https://github.com/jyutcitzi/jyutcitzi-RIME/blob/1efad951f8ef6e2cbc36f05b85726a21e3a2f1c5/images/tone_marks.png)  
   	The extended Jyutcitzi alphabet also contains two additional tone marks:  
   	![RIME入面擴展嘅標調點點](https://github.com/jyutcitzi/jyutcitzi-RIME/blob/4fc8bf49e4424a0743e854259ff2c454eed5a311/images/tone_marks_extended.png)
      基於美感嘅原因，有啲人用粵切字嗰陣會鐘意用 ' 同 " 多過用 - 同 = 嚟分別標粵語嘅第一同第四調。若想轉用 ' 同 " 嘅話，你可以喺揀用 jyutcitzi_font.schema.yaml 同 jyutcitzi_web.schema.yaml 嘅 第二個設定（setting 2）而唔用（setting 1）。
   4. ' 呢個符號係可以攞嚟分開一串粵拼入面啲字，噉樣嚟指定要點樣將一串嘅粵拼變做一個個嘅音節，譬如寫 song'kyun而唔寫songk'yun會噉樣：  
![用撇號嚟分](https://github.com/jyutcitzi/jyutcitzi-RIME/blob/194d5590b80284f298057cd7f67dbe43b7c151e2/images/apostrophe_for_separating.png)
   5. 重複符號「々」喺詞彙有用到：  
![Apostrophe for separating](https://github.com/jyutcitzi/jyutcitzi-RIME/blob/194d5590b80284f298057cd7f67dbe43b7c151e2/images/apostrophe_for_separating.png) 
   6. 啲粵切字鍵盤都有呢啲聲調鍵掣：  
      Q ⇒  ̄，W ⇒  ́，E ⇒ \`，A ⇒ =，S ⇒  ̋，D ⇒ ﾞ，R⇒々
   7. 兩個粵切字鍵盤都會顯示有聲調粵切字同冇聲調粵切字嘅 output 選擇。有啲單音節係淨係得個冇內置聲調嘅粵切字，嗰啲字如果想標調嘅話就可以用上面嗰啲聲調鍵掣。

注意：唔好一次過打太多，唔係嘅話會好易 lag 機㗎！

## 常見問題
問：個鍵盤唔 work 喎！  
答：可以喺輸入法 menu 度重新部署，再唔得就 restart 部電腦。

問：我打唔到某個粵切字，譬如 schweis！  
答：呢個粵切字鍵盤淨係會冚倒通常會喺英文同粵語見到嘅。如果你覺得個鍵盤係需要加某個單音節粵切字嘅話，你可以[開個新嘅 issue](https://github.com/jyutcitzi/jyutcitzi-RIME/issues/new)嚟畀意見！

問：鍵盤啲字詞喺邊度嚟㗎？  
答：啲字詞係嚟自 RIME Cantonese（準確嚟講應該係二〇二〇年二三月嗰個版本）

## 軟件更新
### 第 2.0 版
1. 啲蘇州數字太掗埞，塞唔到入去個字入面嘅四方𡃈，所以粵切字而家喺字嘅右上方用啲點點嚟標調喇
2. 重複符號「々」而家可以標調，譬如 Rv ⇒ 々 ̄：  
   ![Toneful repeat](https://github.com/jyutcitzi/jyutcitzi-RIME/blob/aee302bd087caba2e933d9f22a11b8455ace1e87/images/toneful_repeat.png)
3. 個鍵盤加咗某啲有複合聲母嘅粵切字，譬如「shwaang」（厶亾禾生）、「fwoe」（夫禾居）同 「jyue」（央仒旡）  
   ![shwaang fwoe jyue](https://github.com/jyutcitzi/jyutcitzi-RIME/blob/aee302bd087caba2e933d9f22a11b8455ace1e87/images/shwaang_fwoe_jyue.png)
4. 個鍵盤加咗啲冇聲調嘅複合聲母粵切字，譬如「soecj」同「witcj」（對應英文嘅「search」同）  
5. 鍵盤所包含嘅粵切字係可以攞嚟打英文、日文、台灣閩南話同台灣客家話。為咗可以噉做，呢個鍵盤亦都加咗呢啲粵切字部件：  
a. 圭（⿰）嚟代表喺台灣客家話同英文入面嘅 v-  
b. ㄖ（⿰）或者 禾力（⿰）嚟代表英文同官話入面嘅 r-  
c. 止 嚟代表早期粵語同官話拼音嘅 -i  
d. 亇 嚟代表官話拼音入面嘅 -e 同英文入面嘅 shwa 音。  
e. 艮 嚟代表官話拼音入面嘅 -en  
f. ㄦ 嚟代表官話拼音入面嘅 er  
   ![Extended components](https://github.com/jyutcitzi/jyutcitzi-RIME/blob/aee302bd087caba2e933d9f22a11b8455ace1e87/images/extended_components.png)

### 第 1.1 版
1. 加咗「尼」作為 'ne1'
2. fix咗一個打「best」會出字體版「比旡·乃力·」嘅痋
3. 淨係有聲母嘅同淨係有韻母嘅粵切字而家用 ⺍ 而唔用 \`
