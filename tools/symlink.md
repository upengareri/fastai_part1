### Symlink
---

A symlink or symbolic link is a shotcut path that points to the original path.

#### Why use it?
Let's say we create a project in our local machine which requires use of huge dataset.
In that case we can create a symlink inside our project folder and keep the original dataset
in external drive. This maintains the structure of the project while keeping the hassles of storage away.

#### How to use?
	ln -s [actual location] [new location]

***Example:***
	ln -s /Volumes/external_drive/short_folder /Users/username/Desktop/	

This will create a soft link of short_folder in Desktop.

---
This kind of trick is mostly helpful in my case when I am creating projects in machine learning and I have huge dataset to run but I don’t want to keep the dataset in my local machine (yeah, you got me - 121GB storage). In those cases, I create a shortcut from my project to the actual location of dataset stored in external disk.

_Note_: to get the location of any folder, we can also drag that folder to the terminal which shows the exact path of the folder

_Note_: if the name of the folder has space or special characters, we can simply put the path under quotation. For example 

	ln -s “/Users/username/Desktop/folder name” “/Users/username/Downloads/another folder/”

_Note_: To delete the symlink, simply move it to trash.
