# book-covers
Make a grid of postage-size book cover images to track kids' reading progress!

![](doc/example.png)

# Dependencies
- Working installation of Anaconda / miniconda

# Setup
1. Clone this repository

    ```bash
    git clone https://github.com/matthewgiarra/book-covers
    ```

2. Build the conda environment (which will be named `book-covers`)

    ```bash
    cd book-covers
    conda env create -f environment.yml  
    ```

3. Activate the conda environment

    ```bash
    conda activate book-covers
    ```

# Usage

1. Make a multi-page PDF whose pages are images of book covers. See [tips](#tips) for an easy way to do this. 


2. Open `book-covers.ipynb` in a jupyter notebook

     ```bash
    jupyter notebook book-covers.ipynb
    ```

3. In `book-covers.ipynb`, modify the line `pdf_file_path = covers.pdf` to point to the PDF you saved in step 1.
4. Run the notebook. This will save the grid-of-images figures in the `outputs/grids` directory, and the individual cover images in `outputs/jpg`. The figures that get saved should look something like the image above.

# Tips

- If the resolution of the figures saved to `outputs/grids` is insufficient, you might have better luck saving the figures by dragging-and-dropping them from the notebook window to your file browser.
- To change the sizes of the cover images in the grid, adjust the number of rows and columns by modifying the `plt_rows` and `plt_cols` variables in `book-covers.ipynb`. The cover images will scale so that the `plt_rows`-by-`plt_cols` grid fills the page, e.g., specifying fewer rows/columns will make the individual cover images larger, and more rows/columns will make them smaller. 

## Scanning book covers
The *scan documents* feature in the iPhone *Notes* app is one option for quickly scanning lots of book covers into a single consolidated PDF. The video below shows an example. Once you've saved the scans in the iPhone *Notes* app, you can export the whole thing as a PDF via the corresponding *Notes* app on MacOS.  

![output](https://user-images.githubusercontent.com/6032986/183572080-c3cf0d2c-d5ae-4426-baad-5b9c04a51cc3.gif)



