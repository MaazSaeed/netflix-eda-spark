# Netflix Shows EDA Notebook

This Jupyter Notebook performs Exploratory Data Analysis (EDA) on Netflix shows using PySpark and Python libraries. It processes and visualizes data to uncover insights into Netflix's catalog.

# Process

# Step 1:
Command: "docker run --help"
This command displays the help information for the "docker run" command, which is used to start a new Docker container.
# Step 2:
Command: "docker run -it --name spark-container -p 8888:8888 -v 'C:\Users\Waaz:/home/jovyan/work' jupyter/pyspark-notebook"
This command starts a new Docker container using the "jupyter/pyspark-notebook" image. The key things it does:

"-it" runs the container in interactive mode with a terminal
"--name spark-container" gives the container a name
"-p 8888:8888" maps port 8888 on the host to port 8888 in the container
"-v 'C:\Users\Waaz:/home/jovyan/work'" mounts the "C:\Users\Waaz" directory on the host to the "/home/jovyan/work" directory in the container
"jupyter/pyspark-notebook" is the image used to create the container

# Step 3:
Command: "docker start spark-container"
This command starts the Docker container named "spark-container".

# To check running containers:
Command: "docker ps"


## File Contents
The notebook includes the following:

1. **Importing Libraries**
   - Python libraries used: `pyspark`, `pandas`, `numpy`, `matplotlib`, `seaborn`.

2. **Spark Initialization**
   - A Spark session is set up to handle distributed data processing.

3. **Data Processing**
   - Data is ingested, cleaned, and prepared for analysis using PySpark and Pandas.

4. **Data Visualization**
   - Visualizations are created using Matplotlib and Seaborn to provide insights into trends and distributions.

5. **Package Management**
   - Ensures required packages are installed (`kagglehub`, etc.).

## Key Features
- **PySpark Integration**: Efficient handling of large datasets.
- **Data Cleaning**: Prepares the dataset by handling missing values and ensuring consistency.
- **Visual Insights**: Graphical representation of data for better understanding.

## Outputs
The notebook generates:
- Summary statistics of the dataset.
- Graphs and plots illustrating data trends and distributions.
