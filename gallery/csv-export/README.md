---
description: >-
  CSV is a generic file format for tabular data supported by all spreadsheet
  applications.
---

# CSV export

You can export your gallery or parts of it as a CSV file from the top right corner of the gallery by clicking the floppy disk icon 💾.

{% hint style="warning" %}
In some cases the file is saved with the extension `.txt instead of` .csv. This is a known [issue](https://github.com/joonaspaakko/audible-library-extractor/issues/55) and not a big deal since all spreadsheet applications should open/import the file just with either extension.&#x20;

> The only issue is that your operating system likely won't recognize the correct default application for CSV files. If that is an issue for you, you can just manually rename the file  from `.txt` to → `.csv` and that's it.
{% endhint %}

![](<../../.gitbook/assets/Saving gallery locally.jpg>)

## CSV Compatibility

Pick **raw data** if you're not importing to Google Sheets or Goodreads. You can also use Raw data in Google Sheets if you don't like the clickable icons.

| Compatibility      | Description                                                                                                                                                                                                                                                                                                                                                                                             |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Google Sheets**  | Uses formulas to add useful icon links to the front of the spreadsheet. [My library](https://docs.google.com/spreadsheets/d/1clOlIEPB\_7Ukrq4Don-ANQg201iwRGy8EYFPvQM7DJA/edit?usp=sharing) in Google Sheets. This format is preferred for Google Sheets but you can also use Raw data if the icon links aren't your thing. Check the import instructions [here](google-sheets-import.md).              |
| **Goodreads**      | Exports books with ISBN numbers in a Goodreads compatible format. Bookshelves are generated automatically from the book categories and status: not started (to-read), started (currently-reading), finished (read). [My audible books](https://www.goodreads.com/review/list/105056505-joonas?ref=nav\_mybooks\&shelf=audible) in Goodreads. Check the import instructions [here](goodreads-import.md). |
| **Raw data**       | This one doesn't have any formulas and as such works in any application, like Libre Office, Numbers, Excel, Google Sheets, etc.                                                                                                                                                                                                                                                                         |

{% hint style="danger" %}
Just a reminder that the gallery has a [spreadsheet view mode](../spreadsheet-view.md) that could potentially give you what you want with less effort, if all you want from an actual spreadsheet application is to view it and not to edit it manually or run any kind of formulas etc...
{% endhint %}
