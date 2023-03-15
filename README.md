# Langmuir-Waves-Analysis
Image template for analyzing timing of Langmuir waves detection

A complete guide on how to use download the data and plot it can also be found here in the 'Langmuir Waves Plot Template-Lab Tutorial' ipynb file.

RHESSI BROWSER GUIDE:

-Go to  http://sprg.ssl.berkeley.edu/~tohban/browser/

-Select the day and time of the event you're interested in

-Check:
    GOES w/ RHESSI Times 
    RHESSI by Time 
    RHESSI by Flare 

-After selecting the flare of interest, click on 'Image Archive: for this flare' 
 to get info on the flare HXR peaktime, position etc.

----------------------------------------------

NASA CDA WEB GUIDE:

-Go to  https://cdaweb.gsfc.nasa.gov/index.html  

-Tick the boxes next to the instruments you want to use (Wind, in this case) and submit 

-Uncheck all boxes by clicking on 'Click here to CLEAR All checkboxes' and only select 
 the data you're intereseted in, in this case:

 WI_ELSP_3DP
 
 WI_EHSP_3DP
 
 WI_SFSP_3DP
 
 WI_H1_WAV

 and submit

-Select

 WI_ELSP_3DP: ---> As stacked plot
 
 WI_EHSP_3DP: ---> As stacked plot
 
 WI_SFSP_3DP: ---> As stacked plot
 
 
 WI_H1_WAV: Normalized receiver average voltage (RAD2, 1075-13825 kHz)
 
            Normalized receiver average voltage (RAD1, 20-1040 kHz)
            
            Normalized receiver average voltage (TNR, 4-245 kHz)

Select the time range of interest and submit to plot the data to make sure that it's what you're looking for

Instead of plotting, to download data as csv files:


-Tick 'List Data (ASCII/CSV):'

    -Tick 'CSV options'
    
         -Tick 'Data and global attribute info in CSV'


In your JupyterHub working directory create a folder; you can call it whatever you want, but in this
example its called 'Langmuir waves analysis'.
Inside this folder, for each event you analyse create a new folder named after 
the date of the event you're analysing (dd-mm-yyyy), e.g. 25-04-2002

For each event, move the files you downloaded

WI_H1_WAV_filenumber.csv

WI_EHSP_3DP_filenumber.csv

WI_ELSP_3DP_filenumber.csv

WI_SFSP_3DP_filenumber.csv

into their respective folder

----------------------------------------------

Final steps:

-Change the fields below to match the event you're analyzing

-Run all cells and pray
