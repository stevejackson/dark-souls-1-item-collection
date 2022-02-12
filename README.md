# Dark Souls 1 Japanese Item Collection

All 682 Dark Souls 1 Items, in Japanese (with Furigana) & English, as an Anki deck. Intended usage is for learning Japanese, although it also functions as a way to compare localizations or easily search item descriptions for text.

This repository houses the latest card templates used for that anki deck.

**The latest version can be downloaded here**: https://www.dropbox.com/s/7d7luhuf83dawl1/2022_02_11.03_Dark%20Souls%201%20Items.apkg?dl=0

## Example card

### Front
![Front side](/example_images/DarkBead1.png)

### Back
![Back side 1](/example_images/DarkBead2.png)
![Back side 2](/example_images/DarkBead3.png)

### Another example
![Back side 1](/example_images/AuralDecoy1.png)

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

As mentioned above, I prefer to use ankiweb.net while reviewing cards in this deck, since it allows me to use Yomichan for lookups. It's uglier than the native Anki application, so I made a quick script to at least make the screen less white, and a bit less cramped, but I haven't put more effort into styling it better. It's still quite awful - could be fixed with a bit more time.

Using yomichan is just too good to pass up.

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

### Is the pronunciation/furigana correct for X word?

tl;dr: Probably! But there could also be other valid readings.

The biggest challenge of this project was ensuring the furigana readings were correct. I put a LOT of time into it. There could be a few mistakes left, of course. But I gathered a lot of the readings by listening to a native Japanese speaker read item descriptions, and spent a lot of time googling other items and seeing how native speakers chose to pronounce those.

There are lots of words invented solely for Dark Souls by the writers, and Japanese speakers don't strictly follow the general guidelines of when to use on'yomi and kun'yumi, so you'll hear them using lots of different pronunciations.

### This doesn't work on AnkiDroid, Anki iOS, etc.

Because I don't personally use these, I have not spent time adding mobile support for the layout. It shouldn't be that hard to edit the layout to support mobile, so if someone wants to do it, please feel free to share. But it seems hard to handle the process of doing dictionary lookups from mobile, so it wouldn't be ideal to review there.

### Can I disable the changing background images?

Yes. In the Anki browser, select any card from this deck. Click "Cards" to open the card template editor. On the `Front Template`, scroll until you find `percentOfTimeToChooseRandomBackground` and change the value from `100` to `0`. Or, change it to `50` if you only want a new background on `50%` of the cards, etc.

### What is the English text from?

The English text is the item description from the English copy of the game. It is **not** a 1:1 translation of the Japanese. Like all games, it has been localized, so you'll often notice they don't exactly line up.

Most of the time, I grabbed the English text from https://darksouls.fandom.com/, as it seemed to have the best formatted version. Some of the other English descriptions will come from the text extracted from the game using the TextVessel tool.

## How did I make this?

### Furigana

Far and away, the most time consuming part of this project was ensuring that the furigana was correct. So many words in these item descriptions are open to interpretation as to what their pronunciation is, or at least would differ from what's obvious in the dictionary. I spent a *lot* of time and effort making sure the furigana is as accurate as possible.

First, I used the Anki addon "Japanese Support" to auto-generate some furigana. This usually has quite a few errors even with more common Japanese text, so I had to manually fix those errors. Then, for more Souls-related or weapon-related jargon, I had to scour the internet for answers.

- I'd watch native Japanese speakers playing the game
- Look at native Japanese dictionaries
- Utilize google searches like `ダークソウル 打刀`, `ダークソウル 打刀　読み方`
- A more advanced google search like `"打刀" "うちがたな"` will force results that contain both of those terms, which is very useful for seeing if any native speakers have written the kana out that you're guessing is correct. Oftentimes you'll come across Japanese that are also asking how to pronounce something, dictionaries or other sites providing the kana for pronunciation, etc.

### Screenshots

I used an application called "Greenshot". I set a hotkey for the "Capture window" setting. 

I ran Dark Souls 1: Remastered in 1920x1080 Windowed mode, and used the inventory screen (*not* the equip screen) and captured the screenshot from there.

Afterwards, I processed those screenshots with an Irfanview script and then dragged the result into the appropriate Anki card manually.

```
cd "C:\Program Files\IrfanView"
i_view64.exe "D:\Dropbox\Video Game Anki Decks\Dark Souls 1 Project\To Process\*.png" /crop=(145,220,1095,765,0) /convert="D:\Dropbox\Video Game Anki Decks\Dark Souls 1 Project\Converted\*.png"
```

It took around ~4 playthroughs to gather all the items!

## How to Re-export & Share deck

1. Anki: On the Dark Souls 1 Item Deck, right click, click Export
  - Disable "Include scheduling information"
  - Enable "Include media"
2. Anki: File -> Switch Profile, use a separate profile
3. Anki: File -> Import; import the deck exported above
4. In this new profile, remove the tags `personaltointerval` and `personalskip` for all cards
5. Move the deck up out of its tree organization to top level, so it doesn't include that structure in the export.
6. Anki: On the Dark Souls 1 Item Deck, right click, click Export -- do this again, but from the new profile, now that the cards have been cleaned up.

## Credits & Thanks

- FromSoftware
- u/kymojo & MeowMaritus for the spreadsheet containing Japanese/English
- https://www.youtube.com/playlist?list=PLrbvbc7Y4NFG8GtwJq8MK7eztzV0ZEM36
- 絶険、あるいは逃げられぬHDチャンネル: A Japanese youtuber that did a playthrough of Dark Souls 1 while reading out many item descriptions.
- This blog post which was quite helpful with a lot of Dark Souls-specific language that native speakers might not know how to read: https://bukimara.link/%E3%82%BD%E3%82%A6%E3%83%AB%E3%82%B7%E3%83%AA%E3%83%BC%E3%82%BA%E6%BC%A2%E5%AD%97%E3%81%AE%E8%AA%AD%E3%81%BF%E6%96%B9%E3%81%BE%E3%81%A8%E3%82%81
