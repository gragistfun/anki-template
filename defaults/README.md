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

- Learning steps : 15m 1h 6h 1d 2d 4d 7d
- Graduating interval : 12
- Easy interval : 7
- Insertion order : Sequential (with Scheduler v3 set with 'Display Order')

**Lapses**

- Relearning steps : 15m 4h 2d 7d
- Minimum interval : 12
- Leech threshold : 5
- Leech action : Tag Only

**Display Order**

- New card gather order : Deck
- New card sort order\* : Order gatheres / Card type, then random (ordered / shuffled)
- New/review order : Show before reviews
- Interday learning/review order : Mix with reviews
- Review sort order : Due date, then random

**Burying**

- Bury new siblings : yes
- Bury review siblings : yes

**Advanced**

- Maximum interval : 36500
- Starting ease : 2.50
- Easy bonus : 1.30
- Interval modifier : 0.85
- New interval : 0.20

### Subdecks

Different decks of a subject matter can be organized as subdecks. This open the
possibility for interleaving in review process by setting the `Display order`
option `Review sort order : Due date, then random`.

This comes with some caveats. From the [Anki Manual](https://docs.ankiweb.net/deck-options.html):

```
If your deck has subdecks, each deck can optionally be assigned a different preset.
When Anki shows a card, it will check which subdeck the card is in, and use the
options for that deck. [But]:

The display order options in the v3 scheduler are taken from the deck you select
to study, not the deck of the current card.
```

Sometimes it may be desirable to have different `Display order` options for different
subdecks, especially for new cards. Some decks come with a specific order
(`New card sort order : Order gatheres`), while others a better learned shuffled
(`New card sort order : Card type, then random`).
By setting `New/review order : Show before reviews` to the targeted deck and
learning the new cards individually is it still possible to learn the cards in order.
To differentiate it may be a good idea to mark those decks, for example `Example Deck*`.

## Add-ons

- [Advanced Browser](https://ankiweb.net/shared/info/874215009) (874215009)
- [Colorful Tags (+ Hierarchical Tags)](https://ankiweb.net/shared/info/594329229) (594329229)
- [Review Heatmap](https://ankiweb.net/shared/info/1771074083) (1771074083)
- [More Decks Stats and Time Left](https://ankiweb.net/shared/info/1556734708) (1556734708)
- [True Retention](https://ankiweb.net/shared/info/613684242) (613684242)
  - True Retention opens with `Shift + Click` on `Stats`
- [Anki Simulator](https://ankiweb.net/shared/info/817108664) (817108664)

## References

[Anki Manual](https://docs.ankiweb.net/)

[Effective learning: Twenty rules of formulating knowledge](https://www.supermemo.com/en/blog/twenty-rules-of-formulating-knowledge)
