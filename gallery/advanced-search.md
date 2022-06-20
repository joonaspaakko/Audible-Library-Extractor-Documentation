# Advanced search

The search has advanced functionality for making your searches more specific and you can even search for many different things at once. Odds are simple keywords are good enough for kmost users and you won’t need these, but they are there just in case.

## Search operators&#x20;

These "operators" are characters that serve specific function. Normally the space character is equal to **`and`**, so the search for `demon accords` translates to `contains 'demon' and 'accords'`. Although the search is quite forgiving and may return books that don't fit the criteria a 100%. The vertical bar **`|`** on the other hand is equal to **`or`**, so the search for `demon | accords` translates to `contains 'demon' or 'accords '`. For example, you could search for multiple authors by separating each name with a vertical bar. You can also nullify the **`and`** operator by wrapping the words in double quotes **`"`**. For example `"demon accords"` would translate to `contains 'demon accords'`.

{% hint style="info" %}
The microscope icon on the search bar allows you to specify where to search. I would say you probably don't need to change these much either, but if you're searching for authors, it might make sense to make that the only search scope to prevent false matches.&#x20;
{% endhint %}

### Quick example

Before looking at the full list of search operators, here's a quick recap and an example using the $ operator, which equates to "ends in" the supplied search query. It's always used as a suffix.

| Search query                   | Meaning                                                    |
| ------------------------------ | ---------------------------------------------------------- |
| **`book 1$`**                  | contains "book" **and** ends in "1"                        |
| **`"book 1"$`**                | ends in "book 1"                                           |
| **`theft "volume 1" \| npcs`** | contains "theft" **and** "volume 1" **or** contains "npcs" |

### All search operators

| Token                                                                                                                        | Match type                 | Description                                                                                                                                                   |
| ---------------------------------------------------------------------------------------------------------------------------- | -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [`monster`](https://joonaspaakko.github.io/my-audible-library/#/library?search=monster\&scope=title)                         | fuzzy-match                | Books that fuzzy match [`monster`](https://joonaspaakko.github.io/my-audible-library/#/library?search=monster\&scope=title)(not using any special characters) |
| [`=14`](https://joonaspaakko.github.io/my-audible-library/#/library?search=%253D14\&scope=title)                             | exact-match                | Books that are an exact match to [`14`](https://joonaspaakko.github.io/my-audible-library/#/library?search=%253D14\&scope=title)                              |
| [`'14`](https://joonaspaakko.github.io/my-audible-library/#/library?search=%2714\&scope=title%252Cblurb)                     | include-match              | Books that include [`14`](https://joonaspaakko.github.io/my-audible-library/#/library?search=%2714\&scope=title%252Cblurb)                                    |
| [`!14`](https://joonaspaakko.github.io/my-audible-library/#/library?search=%2114\&scope=title)                               | inverse-exact-match        | Books that do not include [`14`](https://joonaspaakko.github.io/my-audible-library/#/library?search=%2114\&scope=title)                                       |
| [`^fix`](https://joonaspaakko.github.io/my-audible-library/#/library?search=%255Efix\&scope=title)                           | prefix-exact-match         | Books that start with [`fix`](https://joonaspaakko.github.io/my-audible-library/#/library?search=%255Efix\&scope=title)                                       |
| [`!^the`](https://joonaspaakko.github.io/my-audible-library/#/library?scope=title\&search=%21%255Ethe)                       | inverse-prefix-exact-match | Books that do not start with [`the`](https://joonaspaakko.github.io/my-audible-library/#/library?scope=title\&search=%21%255Ethe)                             |
| [`"book 1"$`](https://joonaspaakko.github.io/my-audible-library/#/library?search=%2522book%25201%2522%2524\&scope=title)     | suffix-exact-match         | Books that end with [`book 1`](https://joonaspaakko.github.io/my-audible-library/#/library?search=%2522book%25201%2522%2524\&scope=title)                     |
| [`!"book 1"$`](https://joonaspaakko.github.io/my-audible-library/#/library?search=%21%2522book%25201%2522%2524\&scope=title) | inverse-suffix-exact-match | Books that do not end with [`book 1`](https://joonaspaakko.github.io/my-audible-library/#/library?search=%21%2522book%25201%2522%2524\&scope=title)           |

{% hint style="warning" %}
Most of these links above have been limited to use the scope `"title"`, because with some of these examples the default scopes were a little too generous with the results. The example for `'include` uses scopes `"title"` and `"blurb"` because it turns out that in my library the book 14 is the only one that has the number in the `title`, but I have a few books where it's in the `blurb`.
{% endhint %}

{% hint style="info" %}
You can find a link to this documentation page by hovering the magnifying glass icon in the gallery.

&#x20;<img src="../.gitbook/assets/gallery search icon.png" alt="" data-size="original">
{% endhint %}

## Advanced search example

The most useful feature in this context might be the or operator `|` (vertical bar), which allows you to search for multiple separate things at once. This can be very useful if you want to share a specific set of unrelated books from your library.&#x20;

`storm front​ ​|​ ​space team$​ ​|​ ​demon ​accords ​book 1 ​| ​^hunted` [...will return 4 books](https://joonaspaakko.github.io/my-audible-library/#/library?scope=title\&search=storm%2520front%2520%257C%2520space%2520team%2524%2520%257C%2520demon%2520accords%2520book%25201%2520%257C%2520%255Ehunted\&sortValues=true\&sort=title\&sortDir=asc).&#x20;

I deliberately made each search term specific enough to return 1 book each, but the results of this example may change in the future as my library changes. Of course, I could be using exact matches, but who has the time for that.

![](<../.gitbook/assets/Advanced search.png>)
