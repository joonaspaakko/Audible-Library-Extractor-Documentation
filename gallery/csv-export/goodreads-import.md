# Goodreads import

To import to Goodreads, you first have to export the data as a CSV file. Depending on your CSV export settings, books with no ISBN or ASIN will be excluded. Then you open the import page in Goodreads and upload the file there.&#x20;

You can do ISBN extraction even after you've already extracted your library. When you fetch ISBNs, the extension tries to match the books in your library with ISBN numbers from the Google Books API. You can also import books with ASIN, which gives you an exact match for an Audible audiobook, but according to my testing you also get less matches if you don't include any ISBN's.

> Here's [my library](https://www.goodreads.com/review/list/105056505-joonas?ref=nav\_mybooks\&shelf=audible) imported into goodreads. I don't really maintain it...

### Step 0 (optional):

Fetch ISBN numbers, unless you wish to import using ASIN only. You can fetch ISBNs by doing a new extraction through your Audible Library page, just like you did the first time you extracted the data, just make sure to choose to extract ISBN.

{% hint style="warning" %}
ASIN import is not necessarily recommended for people who have already imported books to Goodreads using ISBNs, because it will likely create a whole lot of duplicate entries and those can be difficult to clean up.
{% endhint %}

{% hint style="info" %}
Exporting with these "Goodreads identifier" settings :white\_check\_mark: isbn :white\_check\_mark: asin :white\_check\_mark: merge  has the potential to give you the most matches with the least amount of duplicates. Unchecking merge will likely give you so many duplicates you'll give up on trying to remove them.
{% endhint %}

### Step 1:

Export your library data as a CSV file

> Pick these settings when exporting => **Data source**: Library **Compatibility**: Goodreads

{% embed url="https://youtu.be/F3GTXB1hj1k" %}
NOTE: THIS IS A GENERAL VIDEO ABOUT EXPORTING CSV! \
Pick the appropriate export settings as stated above the video.
{% endembed %}

### Step 3:

Import the downloaded file to Goodreads. You can use this direct link: [https://www.goodreads.com/review/import](https://www.goodreads.com/review/import)&#x20;

> Or you you can also find your way to the Goodreads import page from `Goodreads.com > My books` from the left sidebar.&#x20;

### Good to know!

Importing this file will create a bunch of shelves from the categories. The two constant values for the shelves are `audible` and `audiobook`. Other shelves it creates are generated from categories and book status: not started (to-read), started (currently-reading), finished (read).

{% hint style="success" %}
If you've refreshed extracted library data after the last import by doing a new extraction, exporting a new Goodreads CSV, and importing it again updates the to-read, currently-reading, and read shelves in Goodreads as long as there were changes from last time.&#x20;
{% endhint %}

### Warnings

> Perhaps even gooder to know...

* It may be difficult to undo an import so if your Goodreads library is your temple, be cautious when importing and maybe try importing one or a few rows first as a test.
* Continuing with the last point, this export / import may produce some or many duplicates and while Goodreads has a tool for resolving duplicates, it's extremely manual. So much so that if you have like a 100 duplicate book entries, you'll be spending the rest of your day resolving them... If you care enough to do so.
* The ISBN import is somewhat unreliable as it's matching audiobooks with books from the Google books api, which so far hasn't returned a single entry for an audiobook to my knowledge. Importantly, to get the most out of it, it doesn't require an exact match, so you are quite likely to get a few wrong entries.

### Why not use Goodreads API for the matching?

There's no doubt that fetching them using the Goodreads API would result in more accurate matches and fewer books without any matches but unfortunately:

> As of December 8th 2020, Goodreads no longer issues new developer keys for our public developer API and plans to retire the current version of these tools. You can find more information [here](https://help.goodreads.com/s/article/Does-Goodreads-support-the-use-of-APIs).&#x20;
