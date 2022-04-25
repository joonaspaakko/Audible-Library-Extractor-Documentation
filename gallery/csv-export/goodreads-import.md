# Goodreads import

Goodreads requires that all books you import have a ISBN, so during the CSV export all books without them will be excluded. You can do ISBN extraction even after you've already extracted your library. When you fetch ISBNs, the extension tries to match the books in your library with ISBN numbers from the Google Books API.&#x20;

> Here's [my library](https://www.goodreads.com/review/list/105056505-joonas?ref=nav\_mybooks\&shelf=audible) imported into goodreads, though admittedly I haven't updatTed in a long time.

### Steps:

1. Fetch ISBN numbers _(if you haven't already)_&#x20;
2. Export the CSV file using
   1. Data source: Library
   2. Compatibility: Goodreads
3. Import this CSV file to Goodreads from [https://www.goodreads.com/review/import](https://www.goodreads.com/review/import)

> You can also find your way to the import page from `Goodreads.com > My books` from the left sidebar.&#x20;

### Good to know!

Importing this file will create a bunch of shelves from the categories. The two constant values in the shelves are `audible` and `audiobook`. Other shelves it creates are generated from `categories` and book status: not started (`to-read`), started (`currently-reading`), finished (`read`).

Assuming you've refreshed extracted library data after the last import, creating a new Goodreads csv and importing again updates the to-read, currently-reading, read shelves in Goodreads as long as there were changes from last time.&#x20;

{% hint style="danger" %}
It may be difficult to undo an import so if your Goodreads library is your temple, be cautious when importing and maybe try importing one or a few rows first as a test.
{% endhint %}

{% hint style="warning" %}
**Be aware** this feature is somewhat unreliable, as the ISBN fetching is far from perfect. During the ISBN fetching, it's matching books with audiobooks, so to get the most out of it, the extension doesn't demand an exact match and it sometimes causes a false match. You will most likely get at least a few false matches.
{% endhint %}

{% hint style="info" %}
#### Why is the extension fetching ISB numbers from Google Books API and not Goodreads API?

There's no doubt that fetching them using the Goodreads API would result in more accurate matches and fewer books without any matches but unfortunately:

> As of December 8th 2020, Goodreads no longer issues new developer keys for our public developer API and plans to retire the current version of these tools. You can find more information [here](https://help.goodreads.com/s/article/Does-Goodreads-support-the-use-of-APIs).&#x20;
{% endhint %}
