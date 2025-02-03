# Installation

| Platforms                                                                                                                                                                                                  | Info                                                                                                            |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| <img src="../.gitbook/assets/chrome.png" alt="" data-size="line">  **Install in** [**Chrome**](https://chrome.google.com/webstore/detail/audible-library-extractor/deifcolkciolkllaikijldnjeloeaall)       |                                                                                                                 |
| <img src="../.gitbook/assets/edge.png" alt="" data-size="line">  **Install in** [**Microsoft Edge**](https://chrome.google.com/webstore/detail/audible-library-extractor/deifcolkciolkllaikijldnjeloeaall) | Installs the Chrome extension: [**Instructions**](edge-installation-instructions.md)                            |
| <img src="../.gitbook/assets/brave.png" alt="" data-size="line"> **Install in** [**Brave**](https://chrome.google.com/webstore/detail/audible-library-extractor/deifcolkciolkllaikijldnjeloeaall)          | Installs the Chrome extension: just click "**Add to Brave**"                                                    |
| <img src="../.gitbook/assets/opera.png" alt="" data-size="line">  **Install in** [**Opera**](https://chrome.google.com/webstore/detail/audible-library-extractor/deifcolkciolkllaikijldnjeloeaall)         | Installs the Chrome extension: just click "**Add to Opera**"                                                    |
| <img src="../.gitbook/assets/firefox.png" alt="" data-size="line">  **Install in** [**Firefox**](https://addons.mozilla.org/en-US/firefox/addon/audible-library-extractor/)                                | ⚠️ For now this is stuck in v.0.2.8, which is broken. Will be updated once the build tools start supporting it. |

> The extension should work in any Chromium based browser.&#x20;

{% content-ref url="../how-to-use-the-extension.md" %}
[how-to-use-the-extension.md](../how-to-use-the-extension.md)
{% endcontent-ref %}

{% content-ref url="../sharing/saving-gallery-locally.md" %}
[saving-gallery-locally.md](../sharing/saving-gallery-locally.md)
{% endcontent-ref %}

{% content-ref url="../sharing/uploading-to-github/" %}
[uploading-to-github](../sharing/uploading-to-github/)
{% endcontent-ref %}

{% hint style="warning" %}
You can find [development releases in Github](https://github.com/joonaspaakko/audible-library-extractor#how-to-install-developement-releases), but you shouldn't install them unless you really have to. One such reason might be that Chrome Web Store releases aren't as quick as Github releases and the extraction can very easily stop working all of a sudden.
{% endhint %}

{% hint style="info" %}
#### Experimental use case

The Chrome extension can also be installed in the **Android** browser [Kiwi](https://kiwibrowser.com/). _This is unfortunately not possible on IOS._ The potential benefit of installing the extension straight on a mobile device is that you can get more or less instant access to the gallery on your mobile device without having to upload it online. However, if you want to show your library gallery to anyone else through a public link, you'd still have to upload it anyway.

With the one-time test that I've performed, there doesn't seem to be much to it:

1. The extraction could be too much for some Android devices as it is quite a heavy process...
2. You need to force Kiwi to view the site in desktop mode because Audible's library is not visible on the mobile website for some reason. You should find it in the 3 dot menu at the top right corner of the browser.
3. You need to keep your phone screen on during the extraction process in order to keep it going. If your screen goes to sleep, it won't do anything catastrophic, it will just pretty quickly slow the process down and not long after stop it entirely. It should pick up where it left off if you open it again.
4. You should probably bookmark the gallery page to get back to it easier. The other way to get back to the gallery later would be to go to your library in audible → open audible library extractor → click the "Open gallery" button.
5. Saving to the home screen doesn't seem to work on this extension gallery page. \
   The uploaded standalone gallery can be saved to the home screen. If you extract the gallery on a desktop computer, the standalone gallery upload/update process to Github is pretty fast and effortless after you've done it a few times.
{% endhint %}

