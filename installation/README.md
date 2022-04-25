# Installation

| Platforms                                                                                                                                                                                                          | Info                                                                                  |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------- |
| ****<img src="../.gitbook/assets/firefox.png" alt="" data-size="line">  **Install in** [**Firefox**](https://addons.mozilla.org/en-US/firefox/addon/audible-library-extractor/)****                                |                                                                                       |
| ****<img src="../.gitbook/assets/chrome.png" alt="" data-size="line">  **Install in** [**Chrome**](https://chrome.google.com/webstore/detail/audible-library-extractor/deifcolkciolkllaikijldnjeloeaall)****       |                                                                                       |
| ****<img src="../.gitbook/assets/edge.png" alt="" data-size="line">  **Install in** [**Microsoft Edge**](https://chrome.google.com/webstore/detail/audible-library-extractor/deifcolkciolkllaikijldnjeloeaall)**** | Installs the Chrome extension: [**Instructions**](edge-installation-instructions.md)  |
| ****<img src="../.gitbook/assets/brave.png" alt="" data-size="line"> **Install in** [**Brave**](https://chrome.google.com/webstore/detail/audible-library-extractor/deifcolkciolkllaikijldnjeloeaall)****          | Installs the Chrome extension: just click "**Add to Brave**"                          |
| ****<img src="../.gitbook/assets/opera.png" alt="" data-size="line">  **Install in** [**Opera**](https://chrome.google.com/webstore/detail/audible-library-extractor/deifcolkciolkllaikijldnjeloeaall)****         | Installs the Chrome extension: just click "**Add to Opera**"                          |

{% content-ref url="../how-to-use-the-extension.md" %}
[how-to-use-the-extension.md](../how-to-use-the-extension.md)
{% endcontent-ref %}

{% content-ref url="../sharing/saving-gallery-locally.md" %}
[saving-gallery-locally.md](../sharing/saving-gallery-locally.md)
{% endcontent-ref %}

{% content-ref url="../sharing/uploading-to-github/" %}
[uploading-to-github](../sharing/uploading-to-github/)
{% endcontent-ref %}

> You can find [development releases in Github](https://github.com/joonaspaakko/audible-library-extractor#how-to-install-developement-releases), but I don't recommend installing them for various reasons. For one, the extension marketplace versions retain previously extracted data when you update the extension. Firefox is particularly difficult with dev releases because it only installs them temporarily.

{% hint style="info" %}
#### Experimental use case

The Chrome extension can also be installed on the **Android** browser [Kiwi](https://kiwibrowser.com). This is unfortunately not possible on IOS. The potential benefit of installing the extension straight on a mobile device is that you can get more or less instant access to the gallery on your mobile device without having to upload it online. Though if you want to show your library gallery to anyone else through a public link, you'd still have to upload it anyways.

With the one time test that I've performed, there doesn't seem to be much to it:

1. The extraction could be too much for some Android devices as it is quite a heavy process...
2. You need to force Kiwi to view the site in the desktop mode because Audible's library is not visible on the mobile website for some reason. You should find it in the 3 dot menu at the top right corner of the browser.
3.  You need to keep your phone screen on during the extraction process in order to keep it going.&#x20;

    If your screen goes to sleep, it won't do anything catastrophic, it will just pretty quickly slow the process down and not long after stop it entirely. If you open it again, it should pick up where it left off.
4. You should probably bookmark the gallery page to get back to it easier. It's not necessary, but the other way to get back to the gallery later would be to go to your library in audible → open audible library extractor → click the "Open gallery" button.
5.  Saving to the home screen doesn't seem to work on this extension gallery page. The uploaded standalone gallery can be saved to the home screen.

    If you extract the gallery on a desktop computer, the standalone gallery upload / update process to Github is pretty fast and effortless after you've done it a few times.
{% endhint %}

