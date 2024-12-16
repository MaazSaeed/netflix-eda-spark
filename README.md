# Netflix Shows EDA Notebook

This notebook performs Exploratory Data Analysis (EDA) on Netflix shows using PySpark and Python. It processes and visualizes data to uncover insights into Netflix's catalog.

## Process  

### Step 1: Start the Jupyter Notebook Container  
Run the following command:  
```bash
docker run -it --name spark-container -p 8888:8888 -v "C:\Users\Waaz:/home/jovyan/work" jupyter/pyspark-notebook
```  
**Explanation:**  
- `-it`: Runs the container in interactive mode with a terminal.  
- `--name spark-container`: Names the container as "spark-container".  
- `-p 8888:8888`: Maps port 8888 on computer to port 8888 in the container.  
- `-v "C:\Users\Waaz:/home/jovyan/work"`: Mounts the folder `C:\Users\Waaz` on your computer to the directory `/home/jovyan/work` inside the container.  
- `jupyter/pyspark-notebook`: Specifies the image to use for the container.

### Step 3: Start the Container  
To start the container, use the following command:  
```bash
docker start spark-container
```  

### Check Running Containers  
To check active containers, use the following command:  
```bash
docker ps
```  

## Notebook Contents  

### 1. Importing Libraries  
The notebook uses the following Python libraries:  
- `pyspark`  
- `pandas`  
- `numpy`  
- `matplotlib`  
- `seaborn`  

### 2. Spark Initialization  
A Spark session is set up to handle distributed data processing.

### 3. Data Processing  
Data is:  
- Loaded and cleaned using PySpark and Pandas.  
- Prepared for analysis by handling missing values and ensuring consistency.

### 4. Data Visualization  
Visualizations are created using Matplotlib and Seaborn to reveal trends and distributions in the dataset.

### 5. Package Management  
The notebook ensures all required packages, such as `kagglehub`, are installed.

## Key Features  

- **PySpark Integration**: Efficiently processes large datasets.  
- **Data Cleaning**: Handles missing values and ensures consistency.  
- **Visual Insights**: Provides graphical representations for easy interpretation of data.

## Outputs  

The notebook generates the following outputs:  
- Summary statistics of the dataset.  
- Visualizations that display trends and distributions in the data.
