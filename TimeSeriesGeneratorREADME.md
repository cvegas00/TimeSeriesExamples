# TimeSeriesGenerator
Welcome to the TimeSeriesGenerator app! To exploit all the functionalities that this app presents please read the instructions carefully. Also, if you find this app useful and you utilise our software, please cite the following work:

Christian Velasco-Gallego & Iraklis Lazakis (2022). **A novel framework for imputing large gaps of missing values from time series sensor data of marine machinery systems.** Ships and Offshore Structures, 17:8, 1802-1811, DOI: [10.1080/17445302.2021.1943850](https://doi.org/10.1080/17445302.2021.1943850).

## Data format
To simplify the uploading process, only files in CSV format are accepted. This CSV file should only contain one column with all the numeric values referring to the time series data. The first row of this column should contain a brief description of the time series data (please see an example below). Please note that the utilisation of any other data format may lead to app malfunction.

## Configuration settings
Some settings can be configured to customise the user experience. These settings relate to the following:

- **Number of states.** This setting is utilised to determine the dimensions of the transition matrix. The default setting is set to determine this number of states automatically based on the original work presented by Velasco-Gallego & Lazakis (2022). However, the number of states can also be selected manually by the user through the utilisation of the slide bar.
- **Series to generate.** This setting refers to the number of series to be generated.
- **Size of the series.** This setting aims to define the lenght of each of the series being generated.

## Example: Generated synthetic time series data from a uniform time series sample
Let's play with this TimeSeriesGenerator app! If you have not accessed to this app already, please go to [https://cvegas00-timeseriesgenerator-main-6quawh.streamlitapp.com/](https://cvegas00-timeseriesgenerator-main-6quawh.streamlitapp.com/). The following UI will appear:


![image2](https://user-images.githubusercontent.com/112953894/188858304-dd98d862-e2d9-4329-9638-6c1403b1b0ea.png)

**Uploading data**

Firstly, we need to upload the time series data that we are going to use to define the transition matrix through the implementation of the first-order Markov chain. If you do not have any time series data available, you can use the one that is being provided as [example](https://github.com/cvegas00/TimeSeriesExamples/blob/main/UniformTimeSeries.csv). To upload the file, we just need to drag & drop the file into the predetermined area or click on the *browse files* button to select one file from your local computer. **Please note that you need to upload a file that follows the data format indicated in the data format section of this document**. 

**Exploratory Data Analysis (EDA)**

Once the file is uploaded, the Exploratory Data Analysis (EDA) section is presented. This section is comprised of three main stages: 1) visualisation of the uploaded data, 2) provision of the descriptive statistics, and 3) visualisation of the time series data in a graphical form.

<img width="1430" alt="Captura de Pantalla 2022-09-07 a les 11 49 09" src="https://user-images.githubusercontent.com/112953894/188860476-7a0047c4-c414-4f98-ba97-53182daf59c3.png">

**Model configuration**

The model configuration section is the subsequent section. This section introduces a form so that the main settings can be defined (please see section configuration settings for further information).

<img width="1432" alt="Captura de Pantalla 2022-09-07 a les 11 53 02" src="https://user-images.githubusercontent.com/112953894/188861217-b1a63fa6-586c-40bb-b873-c4041af84b8b.png">

**Generate synthetic data**
After defining the main settings, we can click on the *Generate series* to finally obtain our synthetic time series data. The data generation process may take a while depending on the settings define in the preceding section. Don't worry, eventually we will get our synthetic data!

Once all the data has been generated, a time series plot of one of the samples will be visualise. Also, you will be able to download all the generated data by clicking on the *Download syntehtic data as CSV* button.

<img width="1429" alt="Captura de Pantalla 2022-09-07 a les 11 59 56" src="https://user-images.githubusercontent.com/112953894/188862512-b1c6c104-4205-4a49-a8b2-83fd346345ab.png">

I hope you enjoy the TimeSeriesGenerator app! Please feel free to contact me if you find any bug or you require further information about the app.
