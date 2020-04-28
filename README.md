# anki-layouts
HTML and CSS for my Anki notes.

I am pretty happy with the layouts that I've come up with for my Anki cards. Others have expressed similar approval, so I figured I would share them (and back them up) in a repo.

They are a work in progress.

**All cards use the same CSS.**

## Examples

### Example Reverse Card with Image

![example-with-image](example-with-image.png?raw=true "Example with Image")

### Example with Hint

![example-with-hint](example-with-hint.png?raw=true "Example with Hint")

Note, you click the hint to display it.

### Example with Extra

![example-with-extra](example-with-extra.png?raw=true "Example with Extra")

Shows how I use the extra fields to display kanji readings.

## Fields

Aside from the Anki default fields (Front, Back, Cloze), all card types use the same 8 fields.

1. Topic
2. Source
3. Extra1
4. Extra2
5. Extra3
6. Audio
7. Image
8. Hint

### Topic
'Topic' is useful for immediately determining what a card is about. For example,

1. A card says "Put your raincoat on."  What am I supposed to do with this? If the topic is "Spanish", it's obvious that I need to translate the sentence.
2. "What does :vsp do?" I could add "In Vim, ..." to all my Vim cards, but I've found it's much better to just set the topic - "Vim".

Before having a `Topic` field, I had cards for Spanish, Japanese, etc. to indicate what I needed to do with a card**. Having this field has greatly cleaned up my cards.

** Note, I use the "single deck" approach that most Vim power users recommend.

### Source

It's a good idea to source your cards, so that you can always go back.

This field is more utilitarian than something you really need to see each time.  Thus, it's displayed at the bottom in small font.

### Extra1, Extra2, Extra3

If you have additional information you want to include about a card but don't want it on the front, put it here.

Due to the [Minimum Information Principle](https://supermemo.guru/wiki/Minimum_information_principle), you want to keep your cards _as simple as possible_  - strive to eliminate any extra clauses, adverbs, etc, and **put extra information in the extra fields**.

For example,

* Elaboration on the topic
* Examples of the topic
* Clarification of terms
* Readings for Japanese Kanji

These fields are displayed below the answer field.  They are in small font since they are less important than the answer, itself.

### Audio

If you didn't know, you can record your own voice directly in the Anki app in addition to linking audio files. Some people do really well _hearing_ the answer in addition to reading it.  Consider adding audio to your cards.

The play button is currently not displayed (didn't want more clutter), but I might need to add this back for use on AnkiDroid.

### Image

Copy a link or drag-and-drop an image into this field in the Anki editor. Some people do really well having visual cues in addition to the answer. It's also one of the [twenty rules of formulating knowledge](http://super-memory.com/articles/20rules.htm). Consider adding images to your cards.

Image is displayed below the extra notes, centered and scaled.

### Hint

Anki has built in [support for hint fields](https://docs.ankiweb.net/#/templates/fields?id=hint-fields). To use, preface your field (in this case `Hint`) with `hint`. See [here](https://github.com/dempe/anki-layouts/blob/master/basic-front.html#L5).

I use this field for various mnemonics - personal stories about a card, "king phillip came over..." type things, etc.

I rarely use this field. If your card is too difficult, try to simplify it by removing extraneous information or splitting it up into multiple cards.

## Usage

Import the included [sample deck](sample-deck.apkg) into Anki. This contains the three card types - basic, reversed, and cloze, and will give you the corresponding styles. (Note they are prefaced with "0-" to make them easier to find in the list).
