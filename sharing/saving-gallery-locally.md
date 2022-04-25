# Saving gallery locally

Technically after you've extracted the metadata, a version of the gallery is accessible locally, but that is directly tied to the extension environment and your browser, so you have to have the extension installed and data extracted to see it. However, the gallery can be saved as a stand-alone gallery by clicking the floppy disk icon 💾 at the top of the extension’s gallery page.

{% tabs %}
{% tab title="Advanced sharing (link sharing)" %}
The best way to share your library would be to upload the unpacked gallery files online as a website, which also allows you to use it on a mobile device. **You can get a library website running for free in Github** and you even get a reasonable domain name to go with it, but that said it does have quite a few steps. Sharing the gallery from that point on is as simple as sending someone the address. For example, here's [my Audible library in Github](https://joonaspaakko.github.io/my-audible-library/).&#x20;

After you've done it once, updating the website is way simpler now that you have an account, a repository, and Github Desktop installed.

> Of course, you can upload the files to your personal website too if you want.

{% content-ref url="uploading-to-github/" %}
[uploading-to-github](uploading-to-github/)
{% endcontent-ref %}
{% endtab %}

{% tab title="Google sheets" %}
You can also save a CSV file in that same modal window. This CSV file could be imported to Google Sheets, which is potentially a slightly easier way to share your library or wishlist or a filtered section of your library with a public link.

{% content-ref url="../gallery/csv-export/" %}
[csv-export](../gallery/csv-export/)
{% endcontent-ref %}
{% endtab %}

{% tab title="Simple sharing (old school)" %}
One option for sharing the gallery would be to send the saved zip file via email. The receiver can unpack the zip and open the `index.html` file in a browser to view the gallery locally. Double clicking the file should open it in your default browser.
{% endtab %}
{% endtabs %}

![](<../.gitbook/assets/Saving gallery locally.jpg>)

{% hint style="warning" %}
This icon is only available in the extension gallery and not the stand-alone gallery.
{% endhint %}
