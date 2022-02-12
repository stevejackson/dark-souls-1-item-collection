# Dark Souls 1 Japanese Item Collection

All Dark Souls 1 Items, in Japanese & English, as an Anki deck. Intended usage is for learning Japanese, although it also functions as a way to compare localizations or easily search item descriptions for text.

This repository houses the latest card templates used for that anki deck.

## Example card

### Front
![Front side](/example_images/DarkBead_Front.png)

### Back
![Back side](/example_images/DarkBead_Back.png)

## How to Re-export & Share deck

1. Anki: File -> Export -> Anki Deck Package
  - Include: Dark Souls 1 Items
  - Disable "Include scheduling information"
  - Enable "Include media"
2. Anki: File -> Switch Profile, use a separate profile
3. Anki: File -> Import; import the deck exported above
4. In this new profile, remove the tags `personaltointerval` and `personalskip` for all cards

## How to Use the Anki deck for studying Japanese

TODO: explain how to suspend the nearduplicates
TODO: explain early-retiring cards

## FAQ

TODO: the alternating backgrounds annoy me

## How did I make this?

### Screenshots

I used an application called "Greenshot". I set a hotkey for the "Capture window" setting. 

I ran Dark Souls 1: Remastered in 1920x1080 Windowed mode, and used the inventory screen (*not* the equip screen) and captured the screenshot from there.

Afterwards, I processed those screenshots with an Irfanview script and then dragged the result into the appropriate Anki card manually.

```
cd "C:\Program Files\IrfanView"
i_view64.exe "D:\Dropbox\Video Game Anki Decks\Dark Souls 1 Project\To Process\*.png" /crop=(145,220,1095,765,0) /convert="D:\Dropbox\Video Game Anki Decks\Dark Souls 1 Project\Converted\*.png"
```

## Credits & Thanks

TODO fromsoft
TODO gamegengo
TODO dark souls item spreadsheet source
TODO zetsuken
TODO that blog post with lots of words
