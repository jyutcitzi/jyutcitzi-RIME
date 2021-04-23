# jyutcitzi-RIME
RIME keyboard for realizing the Honzi-Jyutcitzi mixed script in Hong Kong Cantonese.

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
   f. Hit F4 to switch to either:  
      i. “粵切字 (禾旡·比\`·版)” (web version of the keyboard), or  
      ii. “粵切字 (夫干·天\`·版)” (font version of the keyboard),  
   g. Start typing!
   
   For Windows: To be Updated. Please contact us if you can help us extend this part of the README.

## File Descriptions
For those who want to know more about what the keyboard contains, here is a description of the keyboard-related files in this folder:
- default.custom.yaml - config file for specifying the list of RIME keyboards to use (i.e. RIME Cantonese and Jyutcitzi keyboard)
- jyutcitzi_font.schema.yaml - config file for the Jyutcitzi font keyboard jyutcitzi_web.schema.yaml - config file for the Jyutcitzi web keyboard 
- jyutcitzi_font.dict.yaml - main dictionary for the Jyutcitzi font keyboard, and contains a wide selection of monosyllables rendered using font-based Jyutcitzi characters
- jyutcitzi_web.dict.yaml - main dictionary for the Jyutcitzi web keyboard, and contains a wide selection of monosyllables rendered using web-based Jyutcitzi characters
- jyutcitzi_core.lettered.dict.yaml - dictionary containing the original list of latin- containing compounds from jyut6ping3.lettered.dict.yaml 
- jyutcitzi_font.lettered.dict.yaml - dictionary containing Latin-containing compounds, which are rendered using font-based Jyutcitzi characters
- jyutcitzi_web.lettered.dict.yaml - dictionary containing Latin-containing compounds, which are rendered using web-based Jyutcitzi characters 
- jyutcitzi_font.compound.dict.yaml - dictionary containing Honzi compounds, which are rendered using font-based Jyutcitzi characters 
- jyutcitzi_web.compound.dict.yaml - dictionary containing Honzi vocabulary, which are rendered using font-based Jyutcitzi characters
- jyutcitzi_font.phrase.dict.yaml - dictionary containing Cantonese phrases, which are rendered using font-based Jyutcitzi characters
- jyutcitzi_web.phrase.dict.yaml - dictionary containing Cantonese phrases, which are rendered using web-based Jyutcitzi characters 
- jyutcitzi.jyutcit_phrases.dict.yaml - dictionary containing a selection of phrases from existing Jyutcitzi literature
- mapping.txt - a list containing the Unicode values for newly-created Jyutcitzi and 改革漢字 characters

Apart from these files, the keyboard also relies on jyut6ping3.dict.yaml and jyut6ping3.phrase.dict.yaml from RIME Cantonese, which is why that has to be installed.
