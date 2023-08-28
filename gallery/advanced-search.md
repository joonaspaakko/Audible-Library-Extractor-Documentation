# Advanced search

The search has advanced functionality for making your searches more specific and you can even search for many different things at once. Odds are simple keywords are good enough for most users and you won’t need these, but they are there just in case.

Before I explain how operators work, I should mention that you can tighen the search scope from the microscope icon on the search bar.

> I would say you probably don't need to change the scope much either, but if you're searching for authors, it might make sense to make that the only search scope to prevent false matches.&#x20;

## Search operators&#x20;

These "operators" are characters that serve a specific function.&#x20;

#### AND operator

The space character is equal to **`and`**, so the search for&#x20;

```
demon accords
```

...translates to&#x20;

```
contains 'demon' and 'accords'
```

> Although the search is quite forgiving and may return books that don't fit the criteria a 100%. Either way the best matches are hoisted to the top.

You can also nullify the **`and`** operator by wrapping the words in double quotes **`"`**. This is basically the same as in Google search. It will then look for the exact match for a word or a sentence

```
demon accords
```

...would translate to&#x20;

```
contains 'demon accords'
```

#### OR operator

The vertical bar **`|`** is equal to **`or`**, so the search for

```
demon | accords
```

...translates to&#x20;

```
contains 'demon' or 'accords'
```

> Again, the search is quite forgiving and may return books that don't fit the criteria a 100%. Either way the best matches are hoisted to the top.

***

### Quick example

Before looking at the full list of search operators, here's a quick recap of what I've said so far about the **and** + **or** operators but this time I'm adding the **$** operator into the mix, which equates to "ends in" the supplied search query.

| Search query                    | Meaning                                                            |
| ------------------------------- | ------------------------------------------------------------------ |
| **`book 1$`**                   | contains "book" **and** ends in "1"                                |
| **`"book 1"$`**                 | ends in "book 1"                                                   |
| **`theft "volume 1"$ \| npcs`** | contains "theft" **and** ends in "volume 1" **or** contains "npcs" |

### All search operators

<table data-header-hidden><thead><tr><th width="175.3">Token</th><th width="162">Match type</th><th>Description</th></tr></thead><tbody><tr><td>Token</td><td>Match type</td><td>Description</td></tr><tr><td><a href="https://joonaspaakko.github.io/my-audible-library/#/library?search=monster&#x26;scope=title"><code>monster</code></a></td><td>fuzzy-match</td><td>Books that fuzzy match <a href="https://joonaspaakko.github.io/my-audible-library/#/library?search=monster&#x26;scope=title"><code>monster</code></a>(not using any special characters)</td></tr><tr><td><a href="https://joonaspaakko.github.io/my-audible-library/#/library?search=%253D14&#x26;scope=title"><code>=14</code></a></td><td>exact-match</td><td>Books that are an exact match to <a href="https://joonaspaakko.github.io/my-audible-library/#/library?search=%253D14&#x26;scope=title"><code>14</code></a></td></tr><tr><td><a href="https://joonaspaakko.github.io/my-audible-library/#/library?search=%2714&#x26;scope=title%252Cblurb"><code>'14</code></a></td><td>include-match</td><td>Books that include <a href="https://joonaspaakko.github.io/my-audible-library/#/library?search=%2714&#x26;scope=title%252Cblurb"><code>14</code></a></td></tr><tr><td><a href="https://joonaspaakko.github.io/my-audible-library/#/library?search=%2114&#x26;scope=title"><code>!14</code></a></td><td>inverse-exact-match</td><td>Books that do not include <a href="https://joonaspaakko.github.io/my-audible-library/#/library?search=%2114&#x26;scope=title"><code>14</code></a></td></tr><tr><td><a href="https://joonaspaakko.github.io/my-audible-library/#/library?search=%255Efix&#x26;scope=title"><code>^fix</code></a></td><td>prefix-exact-match</td><td>Books that start with <a href="https://joonaspaakko.github.io/my-audible-library/#/library?search=%255Efix&#x26;scope=title"><code>fix</code></a></td></tr><tr><td><a href="https://joonaspaakko.github.io/my-audible-library/#/library?scope=title&#x26;search=%21%255Ethe"><code>!^the</code></a></td><td>inverse-prefix-exact-match</td><td>Books that do not start with <a href="https://joonaspaakko.github.io/my-audible-library/#/library?scope=title&#x26;search=%21%255Ethe"><code>the</code></a></td></tr><tr><td><a href="https://joonaspaakko.github.io/my-audible-library/#/library?search=%2522book%25201%2522%2524&#x26;scope=title"><code>"book 1"$</code></a></td><td>suffix-exact-match</td><td>Books that end with <a href="https://joonaspaakko.github.io/my-audible-library/#/library?search=%2522book%25201%2522%2524&#x26;scope=title"><code>book 1</code></a></td></tr><tr><td><a href="https://joonaspaakko.github.io/my-audible-library/#/library?search=%21%2522book%25201%2522%2524&#x26;scope=title"><code>!"book 1"$</code></a></td><td>inverse-suffix-exact-match</td><td>Books that do not end with <a href="https://joonaspaakko.github.io/my-audible-library/#/library?search=%21%2522book%25201%2522%2524&#x26;scope=title"><code>book 1</code></a></td></tr></tbody></table>

Most of these links above have been limited to use the scope `"title"`, because with some of these examples the default scopes were a little too generous with the results. The example for `'include` uses scopes `"title"` and `"blurb"` because it turns out that in my library the book 14 is the only one that has the number in the `title`, but I have a few books where it's in the `blurb`.

## Somewhat advanced search example

A search query like this:

```
"Storm Front" | "demon accords" "Book 1"$ | ^hunted | The Grave Kingdom "book 1"$
```

...would return [these 4 books](https://joonaspaakko.github.io/my-audible-library/#/library?scope=title\&search=%2522Storm%2520Front%2522%2520%257C%2520%2522demon%2520accords%2522%2520%2522Book%25201%2522%2524%2520%257C%2520%255Ehunted%2520%257C%2520The%2520Grave%2520Kingdom%2520%2522book%25201%2522%2524\&sortValues=true\&sort=title\&sortDir=asc) from my library.

> I deliberately made each search term specific enough to return 1 book each, but the results of this example may change in the future as my library changes.
