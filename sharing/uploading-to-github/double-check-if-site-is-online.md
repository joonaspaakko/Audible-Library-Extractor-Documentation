# Check if changes are online

After you upload or update the gallery to Github it may take a few minutes or even longer than that to show up online. To check the current status follow these steps.

### Step 1 - Going to the repository in Github.com

You can easily get to your repository page in [Github.com](https://github.com/) from the Github Desktop client.

![](../../.gitbook/assets/ale-github-pages-environments-0.png)

### Step 2 - Check build status&#x20;

Open the Actions page and see if the status looks ok.

{% hint style="danger" %}
If the top most deployment doesn't have a checkmark [check this video below](double-check-if-site-is-online.md#force-page-to-re-deploy-video) to see how you can force Github to try to rebuild the page.
{% endhint %}

![Checkmark means it should be online...](../../.gitbook/assets/githubpages-check-build-status.png)

You can open the website by first opening the next page by clicking the title next to the checkmark :white\_check\_mark: `pages build and deployment`and then click the link:

![](../../.gitbook/assets/githubpages-open.png)



### Force page to re-deploy (video)

Sometimes a page build can fail for no apparent reason or just never finish. If that happens, you can force Github to re-deploy the website by disabling and immediately enabling "Github pages". See the video below. If you don't have the "Actions" tab it should still work if you do the first part of the video up to 0:30.

{% hint style="warning" %}
If the deployment looks to be in `queue` or `progress` try canceling it first.
{% endhint %}

![](../../.gitbook/assets/githubpages-open-cancel.png)

{% embed url="https://youtu.be/d5tDx-CIvo8" %}
Video has no audio
{% endembed %}
