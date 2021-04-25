# jyutcitzi-RIME
RIME keyboard for realizing the Honzi-Jyutcitzi mixed script in Hong Kong Cantonese.

Thanks for supporting this Jyutcitzi keyboard and font project! The following sections contains the installation instruction for Mac and Windows, as well as some words on how to use the keyboard itself, and concludes with a FAQ section.

## Installation Instructions
1. Install RIME ([Squirrel](https://github.com/rime/squirrel) for Mac, [Weasel](https://github.com/rime/weasel) for Windows)

2. Install [RIME Cantonese](https://github.com/rime/rime-cantonese)  
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
- **jyutcitzi_font.schema.yaml** - config file for the Jyutcitzi font keyboard jyutcitzi_web.schema.yaml - config file for the Jyutcitzi web keyboard 
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
   
The extended Jyutcitzi alphabet also contains two additional tone marks: V for 7:


On the account of aesthetics, some will prefer the use of ' and " over ‒ and = for marking tones 1 and 4 when marking tones in Cantonese. To change this preference, please select setting 2 instead of setting 1 in the files jyutcitzi_font.schema.yaml and jyutcitzi_web.schema.yaml.

4. The single quote character ' can be used to separate characters in a string of Jyutping. This character is needed in order to disambiguate the way in which the keyboard splits the string of letters.
e.g. song'kyun ⇒ , instead of songk yun, which gives 
5. The repeat character 々 is automatically used for known compounds
e.g. wong gam gam ⇒ 
6. The Jyutcitzi keyboards also has the following key bindings:
Q⇒ ̄，W⇒ ́，E⇒`，A⇒=，S⇒ ̋，D⇒゙，R⇒々
7. The Jyutcitzi keyboards appropriately provide both toneful and toneless Jyutcitzi as output options. To add pitch to other monosyllables with no toneful option manually use the key bindings!
Warning: Try not to type too many characters in one go, it'll lag the computer a lot!
