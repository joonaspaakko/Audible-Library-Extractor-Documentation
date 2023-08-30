# Saving standalone gallery

After you've extracted the data, you can view the gallery locally, but that is directly tied to the extension environment and your browser, meaning that you have to have the extension installed and data extracted to see it.&#x20;

However, you can save the gallery or it's data through the gallery page's <mark style="color:orange;">**"Extension tools"**</mark> menu item and access it from a mobile device. Or share the link with a friend who can then view your library and wishlist. I've outlined all the main methods below:

{% tabs %}
{% tab title="Standalone gallery (website)" %}
The best way to share your library would be to save the standalone gallery from **Extension tools > Save gallery website,** then upload the unpacked gallery files online as a website, which also allows you to use it on [a mobile device](../gallery/next-listen-mobile-use.md).&#x20;

> **You can get a library website running for free in Github** and you even get a reasonable domain name to go with it. It isn't overly complicated, but it does have quite a few steps.

From that point on, using the standalone gallery yourself or showing it to a friend is as simple as sending the website address. For example, here's [my Audible library in Github](https://joonaspaakko.github.io/my-audible-library/).&#x20;

> Of course, you can upload the files to your personal website too if you want.

{% content-ref url="uploading-to-github/" %}
[uploading-to-github](uploading-to-github/)
{% endcontent-ref %}
{% endtab %}

{% tab title="Google sheets" %}
From **Extension tools > CSV export (spreadsheet)** you can save a CSV file that is usable in any spreadsheet application. I tend to recommend Google Sheets because it's free and you can even share a public link to it.&#x20;

This is potentially simpler than sharing the standalone gallery since there are not as many steps in the process and the concept of uploading a website online is probably more alien to people compared to importing a document to Google Sheets.

{% content-ref url="../gallery/csv-export/" %}
[csv-export](../gallery/csv-export/)
{% endcontent-ref %}
{% endtab %}

{% tab title="Simple sharing (old school)" %}
> This method is no longer possible since v.0.2.9.

~~One option for sharing the gallery would be to send the stand-alone gallery as a zip file via email. The receiver can unpack the zip and open the `index.html` file in a browser to view the gallery locally. Double-clicking the file should open it in your default browser.~~
{% endtab %}
{% endtabs %}
