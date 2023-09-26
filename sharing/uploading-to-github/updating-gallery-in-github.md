---
description: If you have already uploaded the gallery once and want to update...
---

# Updating gallery in Github

### Step 0 - Update library data

If you haveen't already, go back to the Audible website and in your library initiate a new extraction.

> When you've extracted data once, it does a shorter partially extraction.

### Step 1 - Save the stand-alone gallery

Save `ALE-gallery.zip` locally from the gallery menu "Extension tools > Save standalone gallery".

### Step 2 - Replace old files in the project folder

You can find the project folder easily through the Github Desktop application. **Remove all files inside the project folder** and then **put the new files in**.

![](<../../.gitbook/assets/replace old files.gif>)

> If the project is not active in the Github Desktop client, you can open projects from the dropdown in the top left. Then on the right, you’ll find a button that will likely say `Show in Finder` (Mac) or `Show in Explorer` (Windows) click that, [like you did when you first created the project](./#step-4-add-gallery-files-to-the-project-folder) (`repository`).

{% hint style="danger" %}
The project folder contains hidden files that you shouldn't remove or misplace. If you don't see a folder called`.git` then don't worry about it. If you do see it, don't remove it.



> If you do, it's not the end of the world. Either bring it back from the trash or you can also redownload (`clone`) the project using the Github Desktop client, it is uploaded online after all. Just remove the project (`repository`) folder and from the top menu: `File > Clone repository`&#x20;
{% endhint %}

### Step 3 - Save changes

Back in Github desktop app **add a summary** and **save changes** (`commit`).

![](<../../.gitbook/assets/update - save changes.png>)

### Step 4 - Upload to Github

Upload by clicking the `Push origin` button.

{% hint style="warning" %}
It may take a few minutes for the changes to show up after Github Desktop is done uploading the files. If you don't see any expected changes, you can check the deployment status in the website on the "Actions" page. [READ MORE HERE](double-check-if-site-is-online.md).
{% endhint %}

![](<../../.gitbook/assets/update - upload.png>)

