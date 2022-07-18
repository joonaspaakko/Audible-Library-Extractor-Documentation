# Goodreads import

Goodreads requires that all books you import have a ISBN, so during the CSV export all books without them will be excluded. You can do ISBN extraction even after you've already extracted your library. When you fetch ISBNs, the extension tries to match the books in your library with ISBN numbers from the Google Books API.&#x20;

> Here's [my library](https://www.goodreads.com/review/list/105056505-joonas?ref=nav\_mybooks\&shelf=audible) imported into goodreads, though admittedly I haven't updatTed in a long time.

### Steps:

1. Fetch ISBN numbers _(if you haven't already)_&#x20;
   1. You can fetch ISBNs by doing a new extraction. Just make sure to check (select) the 4th item in the extraction settings before clicking the big blue ”Extract Selected Items” button, as you can briefly see in [the desktop usage video](https://youtu.be/LqplX-z-m0s?t=9\&autoplay=0). The linked video should start around 9 seconds in to the video where where the extraction settings are visible.
2. Export the CSV file through the gallery by clicking the floppy disk icon on the top menu.
   1. This opens up a modal window that first talks about saving the gallery locally and then below that you’ll find the CSV export.
   2. Pick these settings when exporting:
      1. Data source: Library
      2. Compatibility: Goodreads
   3. Click download
3. Import he downloaded file to Goodreads from this page: [https://www.goodreads.com/review/import](https://www.goodreads.com/review/import)&#x20;
   1. You can also find your way to the Goodreads import page from `Goodreads.com > My books` from the left sidebar.&#x20;

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
