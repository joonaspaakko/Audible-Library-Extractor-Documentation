# CSV export

You can export your gallery or parts of it as a CSV file from the top right corner under the menu item "Extension tools".&#x20;

> CSV is a generic file format for tabular data supported by all spreadsheet applications.

{% embed url="https://youtu.be/F3GTXB1hj1k" %}

{% hint style="warning" %}
In some cases the file is saved with the extension `.txt instead of` .csv. This is a known [issue](https://github.com/joonaspaakko/audible-library-extractor/issues/55) and not a big deal since all spreadsheet applications should open/import the file just fine with either extension.&#x20;

> The only issue is that your operating system likely won't recognize the correct default application for CSV files. If that is an wissue for you, you can just manually rename the file  from `.txt` to → `.csv` and that's it.
{% endhint %}

## CSV Compatibility

Pick **raw data** if you're not importing to Google Sheets or Goodreads. You can also use Raw data in Google Sheets if you don't like the clickable links and icons.

<table data-header-hidden><thead><tr><th width="326">Compatibility</th><th>Description</th></tr></thead><tbody><tr><td>Compatibility</td><td>Description</td></tr><tr><td><strong>Google Sheets</strong> </td><td>Uses formulas to add useful icon links to the front of the spreadsheet. <a href="https://docs.google.com/spreadsheets/d/1clOlIEPB_7Ukrq4Don-ANQg201iwRGy8EYFPvQM7DJA/edit?usp=sharing">My library</a> in Google Sheets. This format is preferred for Google Sheets but you can also use Raw data if the icon links aren't your thing. Check the import instructions <a href="google-sheets-import.md">here</a>.</td></tr><tr><td><strong>Goodreads</strong></td><td>Exports all books with ISBN numbers in a Goodreads compatible format. Bookshelves are generated automatically from the book categories and status: not started (to-read), started (currently-reading), finished (read). <a href="https://www.goodreads.com/review/list/105056505-joonas?ref=nav_mybooks&#x26;shelf=audible">My audible books</a> in Goodreads. Check the import instructions <a href="goodreads-import.md">here</a>.</td></tr><tr><td><strong>Raw data</strong></td><td>This one doesn't have any formulas and as such works in any application, like Libre Office, Numbers, Excel, Google Sheets, etc. </td></tr></tbody></table>

{% hint style="success" %}
Just a reminder that the gallery has a [spreadsheet view mode](../spreadsheet-view.md) that could potentially give you what you want with less effort if all you want from an actual spreadsheet application is to view the data in that format. The spreadsheet view is read-only, but it does have the same exact search, filter, and sorting methods as the grid view.
{% endhint %}
