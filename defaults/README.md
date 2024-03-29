# Anki Default Settings

## Settings

### General Options

**Scheduling**

- v3 Scheduler : yes
- Next day starts at : 5
- Learn ahead limit : 0

### Deck Options

**Daily limits**

- New cards/day\* : 7 / 999 (Subdeck / Superdeck)
- Maximum reviews/day : 9999

**New card**

- Learning steps : 3m 1h 6h 2d 4d 7d
- Graduating interval : 12
- Easy interval : 7
- Insertion order : Sequential (with Scheduler v3 set with 'Display Order')

**Lapses**

- Relearning steps : 3m 6h 2d 7d
- Minimum interval : 12
- Leech threshold : 3
- Leech action : Tag Only

**Display Order**

- New card gather order : Deck
- New card sort order : Order gatheres
- New/review order : Show before reviews
- Interday learning/review order : Mix with reviews
- Review sort order : Due date, then random

**Burying**

- Bury new siblings : yes
- Bury review siblings : yes
- Bury interday learning siblings : yes

**Advanced**

- Maximum interval : 36500
- Starting ease : 2.50
- Easy bonus : 1.30
- Interval modifier : 0.85
- New interval : 0.20

### Subdecks

Different decks of a subject matter can be organized as subdecks. This open the
possibility for interleaving in review process by setting the `Display order`
option `Review sort order : Random`.

This comes with some caveats. From the [Anki Manual](https://docs.ankiweb.net/deck-options.html):

```
If your deck has subdecks, each deck can optionally be assigned a different preset.
When Anki shows a card, it will check which subdeck the card is in, and use the
options for that deck. [But]:

The display order options in the v3 scheduler are taken from the deck you select
to study, not the deck of the current card.
```

## Add-ons

- [Advanced Browser](https://ankiweb.net/shared/info/874215009) (874215009)
- [Colorful Tags (+ Hierarchical Tags)](https://ankiweb.net/shared/info/594329229) (594329229)
- [Review Heatmap](https://ankiweb.net/shared/info/1771074083) (1771074083)
- [More Decks Stats and Time Left](https://ankiweb.net/shared/info/1556734708) (1556734708)
- [True Retention](https://ankiweb.net/shared/info/613684242) (613684242)
  - True Retention opens with `Shift + Click` on `Stats`
- [Anki Simulator](https://ankiweb.net/shared/info/817108664) (817108664)

## Tips and Tricks

### Searching

Using the [searching features](https://docs.ankiweb.net/searching.html) provided by Anki can be useful in many
situations:

- `is:suspended` : Filter for suspended cards
- `prop:ivl>=366` : Filter for cards with an interval longer than one year to retire mature cards.
- `added:7` : Filter for cards which were added in the 7 days.

### Filter and relearn, refactor or delete 'hard' cards

Some cards may be harder to memorize than others. Since time and attention is a limited resource
it may be a good idea to filter for those cards and take measures to reduce time spent on those cards.

#### Filter

**Lapses / Leeches**

Lapses in combination with the `Leech threshold` are Anki's build in mechanism to detect 'hard' cards. Cards
which gone through relearning more often then the `Leech threshold` are getting tagged.

For more information: [Anki Documentation - Leeches](https://docs.ankiweb.net/leeches.html)

**Advanced Browser**

The [Advanced Browser](https://ankiweb.net/shared/info/874215009) Add-on has some more advanced features to
filter for hard cards:

- `Percent Correct`
- `Time (Total)`
- `Time (Average)`

#### Dealing with 'hard' cards

There are different strategies to deal with hard cards:

**Suspend**

You are missing context or the card is simple to advanced for the current point in time. Suspend the card and
come back to it at a late point in time.

**Relearn**

Maybe you have started a card before thoroughly understanding the subject matter. After revisiting the subject
matter reset the card since the ease of card remains low otherwise, and you will see the card more often then
intended.

**Refactor**

The structure of the card makes it hard to remember. Refactor the card to make it more atomic.

**Delete**

The card has no relevance to you and/or other strategies yielded no results. Delete the card!

## References

- [Anki Manual](https://docs.ankiweb.net/)
- [Effective learning: Twenty rules of formulating knowledge](https://www.supermemo.com/en/blog/twenty-rules-of-formulating-knowledge)
- [Effective spaced repetition](https://borretti.me/article/effective-spaced-repetition)
- [Anki scripting](https://www.juliensobczak.com/write/2016/12/26/anki-scripting.html)
