
# TSP Transformer

### Overview
This project adapts the Transformer model to solve the Traveling Salesman Problem (TSP). It is designed to be run on Google Colab, making setup straightforward and leveraging Colab’s GPU for efficient processing.

### Description
The project is based on *"The Transformer Network for the Traveling Salesman Problem"* by Xavier Bresson and Thomas Laurent.

- **Source Paper**: [The Transformer Network for the Traveling Salesman Problem](https://arxiv.org/pdf/2103.03012.pdf)

### Main Contribution

| Folder Name                      | Description                                                                                       |
|----------------------------------|---------------------------------------------------------------------------------------------------|
| `experiment_TSP50.ipynb`         | Main use for experiments and results analysis on the parameters optimisation |
| `visualization_TSP50.ipynb`      | For testing the current checkpoint trained model of TSP50 
| `visualization_TSP100.ipynb`     | For testing the current checkpoint trained model of TSP100 

### Getting Started

To set up and run this project in Google Colab, follow these steps:

#### Step 1: Download the Project Files
1. Download the entire `TSP_Transformer` folder as a ZIP file from the repository or using the download option on GitHub.
2. Extract the ZIP file to a location on your computer.

#### Step 2: Upload the Files to Google Drive
1. Open [Google Drive](https://drive.google.com/) in your browser.
2. Upload the extracted `TSP_Transformer` folder to the root of your Google Drive.

#### Step 3: Open the Jupyter Notebook in Google Colab
1. Navigate to the `TSP_Transformer` folder in Google Drive.
2. Locate the Jupyter Notebook (`.ipynb` file) you want to run (e.g., `visualization_TSP50.ipynb`).
3. Right-click on the notebook file, select **Open with**, and choose **Google Colab**.

#### Step 4: Connect Google Colab to Google Drive
1. In Google Colab, run the first code cell in the notebook to mount your Google Drive:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```
2. This step will grant Colab access to your Google Drive files, allowing it to read the project files from the `TSP_Transformer` folder.

#### Step 5: Follow Notebook Instructions
Each notebook contains sequential instructions to:
- Set up the environment
- Train the Transformer model on TSP data if using new imported data
- Test model performance and visualize results if using existing checkpoints

Proceed through the cells in the notebook, following the prompts to complete each step.

### Project Structure

| Folder Name                      | Description                                                                                       |
|----------------------------------|---------------------------------------------------------------------------------------------------|
| `.git`                           | Includes file configurations for git repository. |
| `checkpoint`                     | Contains two .pkl files of trained models checkpoints of TSP50 and TSP100                                         |
| `data`                           | Dataset that has been converted int .pkl format.                                                          |
| `dataset`                        | Raw dataset in standard TSPLIB format.                                    |
| `experiment`                     | Includes code for prameters analysis, and testing TSP50 and TSP100 performance. |
| `pic`                            | Picture folder. |
| `pyconcorde`                     | Pyconcorde library. |
| `testing`                        | Testing and visualisation notebook for TSP50 and TSP100. |
| `tools`                          | Tools to visualise .pkl TSP data. |
| `training`                       | Training notebook for .pkl TSP data format and will generate checkpoints. |


### Results and Usage

The notebooks include:
1. **Training**: Step-by-step instructions to train models on datasets like TSP50 or TSP100.
2. **Testing**: Optimality gap analysis and performance evaluations.
3. **Visualization**: View generated TSP paths for both TSP50 and TSP100.

### License
This project is licensed under the MIT License.
