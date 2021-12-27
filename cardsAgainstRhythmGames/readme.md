# json5 basic template  

Sample code below
```
{
  "name": "Pack Name",
  "language": "en-US",
  "author": "Your name",
  "calls": [
    [
      [
        "Black card text with one blank ",
        {}
      ]
    ],
    [
      [
        "Black card text with ",
        {}
      ],
      [
        "More than one blank",
        {}
      ]
    ]
  ],
  "responses": [
    "white card text",
    "another white card text"
    ]
}
```

## Some key notes on syntax

On black cards, each there's a pair of [] for a card, but inside of those there's a pair of [] for each string, or text in quotes.

```
[ #bracket for the card
      [ #bracket for the string
        "Black card text with one blank ", # the string
        {} # the blank itself
      ]
],
```

If there's another card afterwards, the last [] needs a comma. Similarly, if there's more that one string on a card, the [] for the string needs a comma too. 
```
[ # bracket for card
      [ #bracket for first string
        "Black card text with ",
        {}
      ], # note the comma
      [ # bracket for second string
        "More than one blank",
        {}
      ]
]
```

Lastly, I highly reccommend using an editor that can handle syntax highlighting. The lazy option is https://jsoneditoronline.org. It'll let you know real quick if you miss a [] or comma
