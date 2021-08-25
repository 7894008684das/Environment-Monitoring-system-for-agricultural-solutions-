Create Conda Environment

This command will use the yam file to install all dependices which are 
installed using pip and conda package and it uses python version 3.7.10


##First Approach


###### Create conda environment 
```bash 
conda env create --file = requirements.yaml
```
###### Activate conda environment
```bash 
conda activate esa 
```
<hr>

##Second Approach

###### Create conda environment 
```bash 
conda create --name esa python=3.7.10
```
###### Activate conda environment 
```bash 
conda activate esa
```
<hr>

## Installing FBprophet model 

#### To install fbprophet one must first install Pystan which is a library that helps in running Fbprophet with ease. To install Pystan just open you Command Prompt or Anaconda Prompt and then type:
```bash
pip install pystan
```

#### Wait for the installation to finish.

#### 2. Once Pystan is successfully downloaded, the next step is to install Fbprophet either by pip or conda. Under the same Command Prompt just type:

```bash 

pip install fbprophet

```
#### or,
```bash 

conda install -c conda-forge fbprophet

```
#### Install requirements.txt 
```bash

pip isntall requirements.txt 

```


Once your environment is ready.
<hr>

## Run the project


#### Run the api server  
```bash

python main.py

```
####Now open url : http://127.0.0.1:8000/docs

###API Info :
`
Run ETL API 
`
Once the data fetched is from mongodb.
`
RUN Train APi 
`
On the basis of model accuracy copy the models to the <b>WebApp/Models</b> folder and
copy data from preprocessed folder to <b>WebApp/Data</b>.



#### Run the Dash server  
Change directory to WebApp and run the command 
```bash

python app.py

```
<hr>

##Project Documentation  :

The project documentation contains all the modules and method info in web format.The documentation can be accessed from :

`
Documentation/Document Guide/index.html
`