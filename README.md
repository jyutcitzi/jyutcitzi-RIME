# jyutcitzi-RIME
RIME keyboard for realizing the Honzi-Jyutcitzi mixed script in Hong Kong Cantonese.  
Thanks for supporting this Jyutcitzi keyboard and font project! The following sections contains the installation instruction for Mac and Windows, as well as some words on how to use the keyboard itself, and concludes with a FAQ section:  
1. [Installation Instructions](#installation-instructions)  
2. [File Descriptions](#file-descriptions)  
3. [Keyboard Features](#keyboard-features)  
4. [Frequently Asked Questions](#frequently-asked-questions)  
5. [Software Updates](#software-updates)

![Cover Picture](https://github.com/jyutcitzi/jyutcitzi-RIME/blob/d5f0104ab5d2a111f9dc2a0ffa511709fb88f83e/images/cover_picture.png)


## Installation Instructions
1. Install RIME ([Squirrel](https://github.com/rime/squirrel) for Mac, [Weasel](https://github.com/rime/weasel) for Windows)

2. Install [RIME Cantonese](https://github.com/rime/rime-cantonese)  
   For instructions please see https://github.com/rime/rime-cantonese/wiki
   Don't forget to try it out and give it a feel, the Jyutcitzi RIME keyboard is very similar to it :)

3. Install the Jyutcitizi font (available at https://github.com/jyutcitzi/jyutcitzi-fonts)  
   For Mac: Open the TTF file using Font Book, and click “install”  
   For Windows: Right-click on the TTF file and select install  
   Without the font, the Jyutcitzi characters cannot be properly rendered. In terms of fonts, PMingLiU (Regular), SourceHanSerifTC (all weights) and SourceHanSansHC (all weights) have all been augmented with Jyutcitzi characters. SourceHanSansHWHC (all weights) has also been included in the set of fonts, though it only contains Jyutcitzi characters.

4.  Install the Jyutcitzi keyboards (web and font version)  
   For Mac:  
   a. Switch to “Squirrel” on the language tab at the top of the screen  
   b. Click “Settings...”. A new Finder window should appear  
   c. Copy and paste the YAML files to the Rime folder  
   d. Under the language tab, having Squirrel selected, click “Deploy”  
   e. Wait for the keyboards to load, which takes a bit more than a minute  
   f. Hit F4 or CTRL + \` to switch to either:  
      i. “粵切字 (禾旡·比\`·版)” (web version of the keyboard), or  
      ii. “粵切字 (夫干·天\`·版)” (font version of the keyboard),  
   g. Start typing!
   
   For Windows: To be Updated. Please contact us if you can help us extend this part of the README.

## File Descriptions
For those who want to know more about what the keyboard contains, here is a description of the keyboard-related files in this folder:
- **default.custom.yaml** - config file for specifying the list of RIME keyboards to use (i.e. RIME Cantonese and Jyutcitzi keyboard)
- **squirrel.custom.yaml** - config file for specifying the font used in the RIME interface, notably used for rendering the Jyutcitzis listed in the list of options when typing
- **jyutcitzi_font.schema.yaml** - config file for the Jyutcitzi font keyboard
- **jyutcitzi_web.schema.yaml** - config file for the Jyutcitzi web keyboard 
- **jyutcitzi_font.dict.yaml** - main dictionary for the Jyutcitzi font keyboard, and contains a wide selection of monosyllables rendered using font-based Jyutcitzi characters
- **jyutcitzi_web.dict.yaml** - main dictionary for the Jyutcitzi web keyboard, and contains a wide selection of monosyllables rendered using web-based Jyutcitzi characters
- **jyutcitzi_core.lettered.dict.yaml** - dictionary containing the original list of latin- containing compounds from jyut6ping3.lettered.dict.yaml 
- **jyutcitzi_font.lettered.dict.yaml** - dictionary containing Latin-containing compounds, which are rendered using font-based Jyutcitzi characters
- **jyutcitzi_web.lettered.dict.yaml** - dictionary containing Latin-containing compounds, which are rendered using web-based Jyutcitzi characters 
- **jyutcitzi_font.compound.dict.yaml** - dictionary containing Honzi compounds, which are rendered using font-based Jyutcitzi characters 
- **jyutcitzi_web.compound.dict.yaml** - dictionary containing Honzi vocabulary, which are rendered using font-based Jyutcitzi characters
- **jyutcitzi_font.phrase.dict.yaml** - dictionary containing Cantonese phrases, which are rendered using font-based Jyutcitzi characters
- **jyutcitzi_web.phrase.dict.yaml** - dictionary containing Cantonese phrases, which are rendered using web-based Jyutcitzi characters 
- **jyutcitzi.jyutcit_phrases.dict.yaml** - dictionary containing a selection of phrases from existing Jyutcitzi literature
- **mapping.txt** - a list containing the Unicode values for newly-created Jyutcitzi and 改革漢字 characters

Apart from these files, the keyboard also relies on jyut6ping3.dict.yaml and jyut6ping3.phrase.dict.yaml from RIME Cantonese, which is why that has to be installed.

## Keyboard Features
Like RIME Cantonese, the keyboard has the following useful features:
0. Hit CTRL + OPTION + ` to redeploy RIME if it bugs out. Restart the computer if necessary.
1. Hit F4 or CTRL + ` (the backward tick next to the escape button) to switch between RIME keyboards via the arrow and enter key.
2. Hitting the SHIFT or CAPS LOCK key allows one to switch between Latin (A) and Jyutping (中)
3. Tones is optional when typing, add tones as follows:  
   ![Tone marks in RIME](https://github.com/jyutcitzi/jyutcitzi-RIME/blob/1efad951f8ef6e2cbc36f05b85726a21e3a2f1c5/images/tone_marks.png)  
   The extended Jyutcitzi alphabet also contains two additional tone marks:  
   ![Extended tone marks in RIME](https://github.com/jyutcitzi/jyutcitzi-RIME/blob/4fc8bf49e4424a0743e854259ff2c454eed5a311/images/tone_marks_extended.png)  
   On the account of aesthetics, some will prefer the use of ' and " over ‒ and = for marking tones 1 and 4 when marking tones in Cantonese. To change this preference, please select setting 2 instead of setting 1 in the files jyutcitzi_font.schema.yaml and jyutcitzi_web.schema.yaml.

4. The single quote character ' can be used to separate characters in a string of Jyutping. This character is needed in order to disambiguate the way in which the keyboard splits the string of letters, e.g. use song'kyun instead of songk yun:  
![Apostrophe for separating](https://github.com/jyutcitzi/jyutcitzi-RIME/blob/194d5590b80284f298057cd7f67dbe43b7c151e2/images/apostrophe_for_separating.png)
5. The repeat character 々 is automatically used for known compounds:  
![Repeat glyph](https://github.com/jyutcitzi/jyutcitzi-RIME/blob/194d5590b80284f298057cd7f67dbe43b7c151e2/images/repeat_mark.png)
6. The Jyutcitzi keyboards also has the following key bindings:  
   Q ⇒  ̄，W ⇒  ́，E ⇒ \`，A ⇒ =，S ⇒  ̋，D ⇒ ﾞ，R⇒々
7. The Jyutcitzi keyboards appropriately provide both toneful and toneless Jyutcitzi as output options. To add pitch to other monosyllables with no toneful option manually use the key bindings!

Warning: Try not to type too many characters in one go, it'll lag the computer a lot!

## Frequently Asked Questions
Q: The keyboard stopped working!  
A: Try redeploying it under the language tab, or perhaps try restarting your computer.

Q: I can't type a specific monosyllable, e.g. schweis!  
A: This Jyutcitzi keyboard is meant to only cover monosyllabic combinations that are likely to be used in English and Cantonese. If you think it is really essential to add a certain monosyllable to the keyboard, feel free to suggest it by [opening a new issue](https://github.com/jyutcitzi/jyutcitzi-RIME/issues/new)!

Q: Where does the keyboard's lexicon come from?  
A: It directly comes from the lexicon used in RIME Cantonese (a version from Feb-Mar 2020 to be exact)

## Software Updates
### Version 2.0
1. Due to aesthetic issues with Suzhou numerals not fitting into the square box, Jyutcitzi now uses tone marks at the glyph's top-right corner instead when marking tones.
2. The repeat glyph 々 can be toned, e.g. Rv ⇒ 々 ̄:  
   ![Toneful repeat](https://github.com/jyutcitzi/jyutcitzi-RIME/blob/aee302bd087caba2e933d9f22a11b8455ace1e87/images/toneful_repeat.png)
3. A sufficient amount of initial consonant cluster-containing Jyutcitzis were added, such as “shwaang” (厶亾禾生), “fwoe” (夫禾居·) and “jyue” (央仒旡·):  
   ![shwaang fwoe jyue](https://github.com/jyutcitzi/jyutcitzi-RIME/blob/aee302bd087caba2e933d9f22a11b8455ace1e87/images/shwaang_fwoe_jyue.png)
4. Numerous tone-free combinations relating to consonant clusters were also added. Examples include “soecj” and “witcj” (English “search” and “which”):  
   ![soecj witcj](https://github.com/jyutcitzi/jyutcitzi-RIME/blob/aee302bd087caba2e933d9f22a11b8455ace1e87/images/soecj_witcj.png)
5. The keyboard also allows one to transcribe English, Mandarin, Japanese, Taiwanese Hokkien and Taiwanese Hakka in Jyutcitzi. To do this, the following novel components are added:  
a. 圭(⿰) for v- (used in Taiwanese Hakka and English)  
b. ㄖ (⿰) or the consonant cluster wl- (禾力,⿰) for English/Mandarin r-  
c. 止 for Mandarin -i and Early Cantonese -i  
d. 亇for Mandarin Pinyin -e and English shwa sound  
e. 艮 for Mandarin Pinyin -en  
f. ㄦ for Mandarin Pinyin er  
   ![Extended components](https://github.com/jyutcitzi/jyutcitzi-RIME/blob/aee302bd087caba2e933d9f22a11b8455ace1e87/images/extended_components.png)

### Version 1.1:
1. Added 尼 as an entry for 'ne1'
2. Fixed bug where typing 'best' in the font keyboard gave the font equivalent of 比旡·乃力·
3. Adopted ⺍ instead of \` for consonant or vowel only Jyutcitzi characters in the Jyutcitzi font
