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

1. Make a multi-page PDF whose pages are images of book covers. 
2. Open `book-covers.ipynb` in a jupyter notebook

     ```bash
    jupyter notebook book-covers.ipynb
    ```

3. In `book-covers.ipynb`, modify the line `pdf_file_path = covers.pdf` to point to the PDF you saved in step 1.
4. Run the notebook. This will save the grid-of-images figures in the `outputs/grids` directory, and the individual cover images in `outputs/jpg`. The figures that get saved should look something like the image above.

5. If the resolution of the figures saved to `outputs/grids` is insufficient, you might have better luck saving the figures by dragging-and-dropping them from the notebook window to your file browser.


