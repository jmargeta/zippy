# Zippy

Zippy is a simple, lightweight, and quick image annotation tool
for creation of image classification groundtruth.
It is built using [feh](https://feh.finalrewind.org/) -
the fenomenal image viewer and cataloguer.

The decisions to take are assign label 1, 2 or skip until
all images are exhausted or program is quit manually.


# Installation

 - install [feh](https://feh.finalrewind.org/)
 - copy zippy somewhere into the PATH


# Usage

Run Zippy as:

```bash
zippy path_to_images
```

Zippy will traverse the path recursively, randomize the image order.


## Outputs

### **Labels.txt**

full paths and assigned labels

#### Example:

```
/data/eagle.jpg,1
/data/dog.jpg,2
/data/colibri.png,1
/data/albatros.jpg,1
/data/camel.jpg,2
/data/deer.png,2
…
```

### **skipped.txt**

full paths to skipped files

#### Examples
```
/data/trout.png
/data/sardine.jpg
```


## Keyboard shortcuts

 - Enter - skips the image and adds to skipped.txt
 - 1 - assigns label 1 and adds the record to labels.txt
 - 2 - assigns label 2 and adds the record to labels.txt
 - q - quit zippy
 - see feh's manual for the rest



# PRs welcome
 - resume
 - input labels as arguments
 - active training loop
 - allow label correction
 - …
