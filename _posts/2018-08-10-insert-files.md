---
layout: post
title: Inserting Files into Markdown Pages
subtitle: Using github.com interface
tags: [help, website]
---

## Inserting Files into Markdown

Adding your own images or file into a markdown page takes a few steps:

1. Upload the image or files to github repository
2. Add link to page with path to the file

Note: These instructions focus on adding files and images using the github.com editor interface. Experienced users should clone the repository and make the changes on their local version.

### Creating a new folder

All module files and images should be stored in [`/assets/`](https://github.com/MarineGEO/marinegeo.github.io/tree/master/assets) folder.

Each module should have it's own subfolder. In order to create a new folder, we will have to create a temporary file (git doesn't store empty folders). Click the `Create new file` button, enter in the new folder name followed by a forward slash `/` and a temporary file name in the `Name your file...` box. Finally, commit the new file.

![Create New folder github](/assets/blog/2018-08-10-insert-files/createFolder.mov.gif)


### Uploading an asset

Navigate to the folder where you want to upload the asset (image, pdf, etc). Click the `Upload Files` button and drag files that you want to add. After the files are uploaded, commit the changes and include a commit message describing the files that were added.

![Upload an asset](/assets/blog/2018-08-10-insert-files/uploadImage.mov.gif)
