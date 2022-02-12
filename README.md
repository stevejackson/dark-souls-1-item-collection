# Dark Souls 1 Japanese Item Collection

All Dark Souls 1 Items, in Japanese & English, as an Anki deck. Intended usage is for learning Japanese, although it also functions as a way to compare localizations or easily search item descriptions for text.

This repository houses the latest card templates used for that anki deck.

TODO: add link to the anki deck on ankiweb.net

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
5. Anki: File -> Export -> Anki Deck page -- do this again, but from the new profile, now that the cards have been cleaned up.

## How to Use the Anki deck for studying Japanese

### Difficulty level

I recommend that you can at least roughly understand N4 grammar before spending a lot of time on this. These item descriptions are pretty consistent with the types of grammar they use past the N4 level though, so once you get the hang of it, the biggest challenge will be likely be the vocabulary.

In general, I found that many words are repeated and re-used throughout these items, which helped with reinforcing their meaning.

### Before using the deck

There are quite a few items that are extremely similar to each other, namely armour sets. I have tagged items like this that aren't really worth learning as `nearduplicate`. I recommend going into the Anki card browser, searching for `tag:nearduplicate`, selecting all of these cards, and suspending them (right click -> Toggle Suspend.)

### How to learn & review cards

Here is what I would personally recommend for the somewhat daunting task of using this deck. Since it's not broken up into single sentences, or one vocab word per card, each card will definitely take a lot more work than a normal Anki card. Because of that, I don't treat them like normal, quick-to-review Anki cards.

* **I wouldn't recommend learning each Anki card in perpetuity**. These cards are long to review, and it would get quite aggravating. I would advise choosing an interval, and essentially once cards reach that interval, suspending them. Go to Anki Browser, right click on the columns and select "Interval" to see what your cards intervals are. I essentially go into the card browser every couple of days and suspend cards over 14 days. That means I'm learning the card well enough to remember it for 14 days, but I have no need to remember it forever.
  * There's an addon which may do this for you automatically, but I have not tried it: https://ankiweb.net/shared/info/1666520655
* **Use a quickly searchable dictionary of some sort while learning these cards**. You'll be looking up a lot of new vocabulary and this should be very convenient. Here are the methods I'm aware of:
  * Use ankiweb.net to review cards in this deck instead of another app. The interface is uglier, but it means you can use the Yomichan browser extension, or 10ten, etc while reviewing cards. That makes word lookups completely smooth. See below for some customization I've made to the ankiweb.net UI to be slightly better.
  * Use the Migaku Dictionary addon for Anki, which adds a dictionary within Anki you can use with a hotkey (ctrl+s while selecting the word to lookup, I think?)
  * Use the "Web Browser" addon for Anki, which adds a browser within Anki. Using a hotkey you setup, it will search the selected text on any website or dictionary website you choose. https://ankiweb.net/shared/info/864545277
* I have had a lot more success using monolingual dictionaries for these item descriptions. English language dictionaries miss a lot of valid pronunciations and words that are in these items, so you'll be misled if relying on those definitions alone. This site has good advice on how to do so (I've set them up within Yomichan): https://learnjapanese.moe/monolingual/

* You can hover over words even when on the front of a card to see the furigana.

### Customize ankiweb.net for reviewing

As mentioned above, I prefer to use ankiweb.net while reviewing cards in this deck, since it allows me to use Yomichan for lookups. It's still much uglier than the native Anki application, but I haven't put more effort into styling it better. Using yomichan is just too good to pass up.

I use the Stylebot chrome addon with this stylesheet:

```
body {
    background-color: black;
}

div#qa_box {
    min-width: 1400px;
    min-height: 1200px;
}
```

Set to `URLs on the domain`: `ankiuser.net`

## FAQ

TODO: is the pronunciation/furigana correct for X word?
TODO: mobile support
TODO: the alternating backgrounds annoy me

## How did I make this?

### Furigana

TODO

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
