# PhotoManager
Project Overview:  

Here are updated client requirements:

The user wants to be able to manage a set of tags independently from any
images. This tag set should persist through a quit and restart. The user
doesn't want to type the `@` symbol, although it should appear in tagged image
filenames.

The user wants to be able to choose a "root" directory and see a list of images
anywhere under that directory. Images in that directory may include tags that
aren't in the tag set. Any such tags should be automatically added to the tag
set.

The user wants to be able to select an image and view it. The absolute path to
that image file should be visible in the UI.

When viewing an image, the user can select multiple tags at once and apply them
to the current image. The user can also remove tags from the image.

Whenever an image is tagged the application will rename the image file to
include the tags, each prefixed with the "@" character. For example, if the
user has tagged an image with "Aunt June" and "Samantha", then the file will be
renamed to include "@Aunt June @Samantha". The user should also be able to open
(directly in their OS's file viewer) the directory containing the current image
file.

The user should be able to move a file to another directory under the "root" directory. (It's okay if your program works when the target directory is not under the "root" directory, but your program doesn't need to be able to handle that if you prefer.)

The user wants to be able to view and revert to older file names for the current image. Provided that an image has not been manually moved or renamed using the OS, the user can view all the names that a file has had. This should persist through a quit and restart.

The user wants a log of all renaming ever done to all files (old name, new name, and timestamp), and this log should be viewable by the application.

When the program is first run, it should create any configuration files that it
needs, and if they are deleted it should recreate them the next time it is run.
