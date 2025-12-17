This project can be run in Google Colab or in a local Python 3.8+ environment. No external datasets are required because all phantoms are generated programmatically.

The required packages are numpy, matplotlib, scikit-image, and PyQt5 (PyQt5 is only needed if running the GUI). These can be installed with:

pip install numpy matplotlib scikit-image PyQt5

To run the project in Google Colab, upload the Virtual\_CT\_Scanner.ipynb file and run all cells in order. The notebook will automatically generate the circular, rectangular, and head phantoms, produce sinograms, reconstruct the images, compute difference maps, generate signal intensity profiles, and calculate the image quality metrics (MSE, RMSE, MAE, SSIM). It will also run the acquisition parameter studies.

To run the GUI locally, open a terminal in the project directory and run the colab.

The GUI allows selecting a phantom, adjusting acquisition parameters such as projections, detectors, spacing, and noise, and then running the scan. It displays the phantom, sinogram, reconstructed image, difference image, signal intensity profile, and the parameters used.

This runs the full phantom-to-reconstruction pipeline and displays all results.

No external databases or repositories are required. The project does not involve machine learning or AI training, so no training or model-loading instructions are needed.

Testing and evaluation are performed automatically. When the code is run, it computes MSE, RMSE, MAE, and SSIM to compare the reconstructed image with the phantom. These, along with the plots and acquisition parameter outputs, appear automatically.

To ensure the project is fully reproducible, install the required packages, open the Colab notebook or run the GUI or scanner script, and follow the steps above. All code dependencies are self-contained, and no additional configuration is needed.

