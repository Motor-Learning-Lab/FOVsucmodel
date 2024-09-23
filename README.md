# FOV adaptation model
The code of FOV adaptation model

# environment.yml 
The environment you need to run all the process the important libraries are
PyMC (5.12.0)
Ariviz (0.18.0)
numpy
pandas
matplotlib
seaborn

# Usage 
  ## If you just want to see the Bayesian analysis process
   ### Make sure that output plots folders are all right for you
        After you prepare the Python environment and modify the output file 
   ### Make sure you can connect to the internet (figshare) and run the model ipynb files  
      1. In the successpersession folder, run ESTgamma.ipynb. Input is the model_session_final.csv which should be automatically downloaded to the corresponding folder. You can also got to https://figshare.com/articles/dataset/Data_of_the_Bayesian_model/27061012 and download the data mmanually. The whole process of the Baysian analysis is included in the file. 
      2.Similarly, In the angularerror folder, run fovdisD2.ipynb. Input is the model_trial_final.csv which should be automatically downloaded to the corresponding folder.
      3.Similarly, In the distancetravelled folder, run fovM4D2.ipynb. Input is the model_trial_final.csv which should be automatically downloaded to the corresponding folder.
  ## if you are willing to go through all the process
  ## Make sure that raw data and plots folders are all right 
    Search for all the store addresses in the ipynb, replace them with your own adress.
   ## Run the ipynb files in the preprocessandtrace folder
   ### Run rawdata.ipynb
        The input is the raw data form FOV which is the data from each trial of each fish in one session of one stage.You will get the preprocessed dataframes which are ready to plot the trace plots for each fish in each session. 
   ### Run rawdataplots.ipynb
        The input is the combined preprocessed dataframes. Output is the trace plots of each fish in each session of all the stages (except Final stage(ReWashout)). You have options to choose which exact trial you want to plot by changing the input into the extact fish ,session and trial id.
   ### Run the Forposter.ipynb
        The input is the combined preprocessed dataframes. Output is the trace plots of each fish in each session of Final stage. The figurestyle is forposter.
   ## Run the ipynb files in the measures folder
   ### Run Rawdata.ipynb
        The input is the raw data form FOV which is the data from each trial of each fish in one session of one stage.You will get the preprocessed dataframes which are defined as different measures for measuring the performance of the FOV task. 
   ### Run Patchdata.ipynb
        The input is the preprocessed dataframes and this is forcaluculating some complex measures inclding some measures we did not show in the paper.
   ### Run Measureplot.ipynb and Ameasureplot.ipynb (Optinal)
        You can check the meaure plots by these code. Measureplot.ipynb is for the indivual fish. Amesureplot.ipynb is for the measure across fish.
   ### Run tne dataformodel.ipynb (*)
        You can choose any measures you want to use to fit the models. In the paper, We use the success/session, angular error and distance travelled. Then you will get the model_session_final.csv and model_trial_final.csv in our figshare link.


# Updated on 23/9/2024
