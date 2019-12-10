# Big Data Programming - March Twitter data analysis local processing

Please follow these instructions in order to run the local processing
Jupyter Notebook to run - March2016_Twitter_Processing_Local.ipynb 

Open terminal on your linux/ubuntu OS and follow the following
If the system is Windows or Mac, Anaconda can be installed by loading the URL:
https://www.anaconda.com/distribution/
and downloading the Anaconda3.7 for your respective OS and follow the terminal commands from 'Creating a new environment'

## Installation Anaconda - Linux

```$
cd /tmp
curl -O https://repo.anaconda.com/archive/Anaconda3-2019.10-Linux-x86_64.sh
```
The download may take some time depending on your connection speed.

```$
bash Anaconda3-2019.10-Linux-x86_64.sh
```

Follow the further instructions to install Anaconda and verify the installation by running:
```$
conda info
```

##Creating a new environment
```$
conda create -n bdp python=3.7
```
This will create a new environment with name 'bdp' with Python version 3.7

##Activating new environment
```$
conda activate bdp
```
This will activate the new environment

##Installing the required packages
```$
conda install -c conda-forge spacy
```
```$
python -m spacy download en_core_web_md
```
```$
conda install -c conda-forge swifter
```
```$
pip install autocorrect
```
```$
pip install pandas
```
```$
pip install -U scikit-learn
```
```$
pip install seaborn
```
```$
pip install bokeh
```
```$
pip install numpy
```
```$
pip install matplotlib
```
```$
pip install tabulate
```
```$
pip install wordcloud
```
```$
pip install jupyter
```
```$
pip install pyspark
```

Now, copy the files which were created during the previous run to a new folder and the main code file. The folder from which the input files are originating are mentioned in the Jupyter Notebook. 

For example, for the input file for Misspelled words, take the file "part-00000-481943e0-3049-4c42-803a-93134747645e-c000.csv" from the output folder "Misspelled_words.csv"

Jupyter Notebook - March_2016_Twitter_Processing_Local.ipynb

##Running the local processing
```$
jupyter notebook
```
This will open a browser tab.
Locate the respective project folder and open the .ipynb file

Lastly, click on the 'Cell' option in the top toolbar and then click on 'Run all'.
Please wait for the code to process all data. This may take around 180 minutes to process.


