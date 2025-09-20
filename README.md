Here’s the README file for your project:

---

# **SH+ Migration Strategy Analysis**

This project analyzes the fleet of 3rd party (3P) devices for the SH+ platform to guide the migration strategy from AWS' AUC to IoTMI. The analysis clusters households based on the number of devices and manufacturers, providing insights for migration batching.

---

## **Requirements**

1. **Python**: Version 3.8 or later.
2. **CSV File**: The dataset required for the analysis is available in the Jira story: [SET-96889](https://telusvideoservices.atlassian.net/browse/SET-96889). Download the file and add it to the project directory.
3. **Browser**: A modern browser (e.g., Chrome, Firefox) to view the Jupyter Notebook interface.

---

## **Setup**

### **Step 1: Install Python**

- **macOS**:
  - Open the Terminal and install Python via Homebrew:
    ```bash
    brew install python
    ```
  - Verify the installation:
    ```bash
    python3 --version
    ```

- **Windows**:
  - Download Python from [python.org](https://www.python.org/downloads/).
  - Follow the installation instructions and ensure the "Add Python to PATH" option is checked during installation.

- **Linux**:
  - Use your package manager to install Python:
    ```bash
    sudo apt update
    sudo apt install python3
    ```

---

### **Step 2: Clone the Repository**

Clone this repository to your local machine:

```bash
git clone <repository-url>
cd <repository-directory>
```

---

### **Step 3: Set Up a Virtual Environment**

Create and activate a virtual environment to isolate dependencies:

```bash
python3 -m venv venv
source venv/bin/activate  # On Windows, use `venv\\Scripts\\activate`
```

---

### **Step 4: Install Dependencies**

Install the required Python libraries:

```bash
pip install -r requirements.txt
```

The `requirements.txt` file includes:

```
pandas
matplotlib
seaborn
scikit-learn
notebook
```

---

### **Step 5: Add the CSV File**

Download the CSV file from the Jira story [SET-96889](https://telusvideoservices.atlassian.net/browse/SET-96889) and place it in the project directory. Ensure the file is named `asset_data_18092025.csv` to match the notebook's code.

---

### **Step 6: Run the Jupyter Notebook**

Launch Jupyter Notebook:

```bash
jupyter notebook
```

This will open the Jupyter interface in your default web browser. If it does not open automatically, copy and paste the URL displayed in the terminal (e.g., `http://localhost:8888`) into your browser.

---

### **Step 7: Open and Run the Notebook**

1. In the Jupyter interface, navigate to the `shplus_assets_20250918.ipynb` file and click to open it.
2. Run the notebook cells sequentially:
   - Use **Shift + Enter** to execute each cell.
3. The notebook will generate visualizations and insights based on the CSV data.

---

### **Step 8: Visualize the Results**

- The notebook produces the following visualizations:
  - **Devices per Manufacturer**: A bar chart showing the number of devices for each 3P manufacturer.
  - **Households with Single Manufacturer**: A bar chart showing households that have devices from only one 3P manufacturer.
  - **Clusters of Households**: A bar chart showing the clustering of households based on the number of devices.

These visualizations will help guide the migration strategy by identifying logical batches for migration.

---

## **Contributing**

Feedback is welcome!

juan.gramajo@telus.com
