# PyQt Image Annotation Tool

This app is used to label images in a given directory.
Labeled images can be moved or copied into sub-directories, which are named as assigned labels.
The app is just a single Python script with GUI.

![PyQt Image Annotation Tool GUI](https://i.stack.imgur.com/iihhf.png)

## What can this app do
For example you have folder ./data/images/ with a lot of images and you need to assign some
label(s) to these images.

- it can assign multiple labels to one image
- it allows you to choose number and names of your labels
- it can move/copy images to folders that are named as desired labels.
- it can generate .csv file with assigned labels.
- it can generate .xlsx file with assigned labels.
- all settings are handled via GUI

## Installation and usage

1. Clone the project:
    ```bash
    git clone https://github.com/FilipAnjou/PyQt-image-annotation-tool.git
    ```

2. Enter the directory and install the dependencies (you might need to use `pip3` instead of `pip`):
    ```bash
    cd PyQt-image-annotation-tool
    pip install -r requirements.txt
    ```
3. Run the app (use `python3` for Python 3)
   ```bash
    python main.py
    ```

## Keyboard shortcuts

- `N` (or `d`): Next image
- `P` (or `a`): Previous image
- 1-9: Select label
- `R`: Show random unlabeled image
- `esc`: Clear labels of currently shown image

## TODO

- [x] Use `a` and `d` to switch between images (`N` and `P` are awkward)
- [x] Skip to first un-labeled on startup (assumes no image has been skipped)
- [ ] Keep labels from previous image 
- [x] Shuffle (using the `r` key)
- [ ] More (and better) keybinds
- [x] Button for clearing all labels from an image (using the `esc` key)
- [ ] Only allow one active label for each lane. Selecting a new one should remove the other

