# Prompts used to ask ChatGPT (GPT-4, paid subscription)

## Create ChatGPT 'Avatar'
'Associate professor Data Science in Life Sciences & Chemistry'

As an Associate Professor specializing in "Data Science in Life Sciences & Chemistry" at Hogeschool Utrecht (HU), 
you are a member of the Research Group for Innovative Testing (INT). This group, which you founded 15 years ago, 
is now a part of the "Knowledge Center for Healthy and Sustainable Living." The Knowledge Center is overseen by a full professor, 
who is also one of your supervisors, and she serves as its Director. In addition to your research responsibilities, 
you also teach Data Science within the Laboratory Education program at HU. Your role involves actively seeking 
collaborations with other research groups within the Knowledge Center, which encompass a 
variety of fields such as health care, physiotherapy, built environment, and engineering.

### prompt 1
In the capacity of 'Associate Professor', I am hosting a workshop aimed at showiung the potential 
of AI for the different research groups in the Knowledges center. I have 1.5 hours. There needs to be a short 
theoretical intro to what AI is and how it could be used in the context of the research. Followed by a practical hands-on in R 
(tidymodels and tensorflow for R). Write the full documentation for this workshop.

### Prompt 2
Now write this content from the Research as it is being done in the Research Center where I work,

### Prompt 3
Now show this contents in a raw Markdown code chunk.
See also file `./workshop-overview.md`

```
# Workshop Title: 
"Integrating AI in Life Sciences and Chemistry Research: A Hands-On Workshop"

## Date and Venue:
[Insert Date and Venue]

## Duration:
1.5 hours

## Target Audience:
Members of the Knowledge Center, encompassing researchers and faculty in health care, physiotherapy, built environment, and engineering.

## Workshop Objective:
To showcase the potential of Artificial Intelligence (AI) in enhancing research methodologies within the domains of life sciences, chemistry, and other related fields, using R with a focus on `tidymodels` and `tensorflow`.

---

### Part 1: Theoretical Introduction to AI (30 minutes)

#### 1.1 Understanding AI in a Research Context (10 minutes)
- Clarifying AI concepts with a focus on their relevance in life sciences and chemistry.
- The impact of AI on modern research methodologies.

#### 1.2 AI Applications in Research at the Knowledge Center (20 minutes)
- Examples of AI in current projects at the Knowledge Center.
- Potential AI applications in health care, physiotherapy, built environment, and engineering.
- Ethical implications and responsible AI use in research.

---

### Part 2: Practical AI Applications using R (1 hour)

#### 2.1 R for AI: Setup and Overview (10 minutes)
- Introduction to R and its AI-centric packages (`tidymodels`, `tensorflow`).
- Preparing the R environment for AI modeling.

#### 2.2 Modeling with `tidymodels` in Research (25 minutes)
- Exploring data preparation and model building in a life sciences context.
- Interactive session: Developing a predictive model related to a real project from the Knowledge Center.
- Hands-on practice for participants.

#### 2.3 Deep Learning with `tensorflow` in R (25 minutes)
- Basics of neural networks in the context of chemistry and life sciences research.
- Demonstrating a simple neural network model.
- Participant activity: Experimenting with neural network models.

---

### Part 3: Wrap-Up and Interactive Discussion (15 minutes)

#### 3.1 Workshop Summary (5 minutes)
- Recapitulating the main takeaways and their relevance to ongoing research.

#### 3.2 Open Discussion and Q&A (10 minutes)
- Addressing queries and discussing potential AI applications in participants' research areas.
- Encouraging interdisciplinary collaboration within the Knowledge Center.

---

### Additional Resources:
- Curated list of AI research articles and resources relevant to the Knowledge Center's fields.
- Contact details for ongoing support and collaboration in AI-related projects.

---

### Feedback and Follow-Up:
- Collect feedback for workshop improvement.
- Plan for potential follow-up sessions or collaborative meetings.

---

### Logistics:
- Confirm all technical requirements are met, including software installations and data sets for hands-on sessions.

---

**Note:** This workshop is designed to be highly interactive and relevant to the ongoing research at the Knowledge Center, encouraging the practical application of AI in various research domains.
```

## Finding data to use

### Prompt 4
Provide an example of a dataset that would be applicable for the purpose of part 2.2

ANSWER:
For part 2.2 of your workshop, which focuses on modeling with tidymodels in a life sciences context, an appropriate 
dataset could be one related to gene expression profiling. This type of data is highly relevant to life sciences and offers 
a rich ground for predictive modeling.
Example Dataset: Gene Expression Cancer RNA-Seq Data

Overview:

    This dataset contains gene expression profiles gathered through RNA sequencing.
    The data is often used to classify types of cancer based on gene expression patterns.
    Each row represents a sample (for instance, a patient's tumor tissue), and each column represents a gene. 
    The cell values are expression levels of the genes.

Attributes:

    Gene Expression Values: Continuous variables representing the expression level of each gene.
    Cancer Type: A categorical variable indicating the type of cancer (e.g., breast, lung, colon).
    Patient ID: Unique identifier for each patient/sample.
    Clinical Data: Additional variables like age, gender, treatment response, survival time, etc., can be included 
    for more comprehensive analysis.

Potential Analysis with tidymodels:

    Classification Models: Developing models to classify the type of cancer based on gene expression profiles.
    Feature Selection: Identifying key genes that are most predictive of specific cancer types.
    Predictive Analytics: Using clinical data alongside gene expression to predict treatment outcomes or survival rates.

Ethical Considerations:

    Ensure data privacy and ethical use, especially since this involves sensitive health information.
    Use anonymized data or obtain necessary permissions for educational purposes.

Where to Find Similar Datasets:

    Public repositories like The Cancer Genome Atlas (TCGA) or Gene Expression Omnibus (GEO).
    Synthetic datasets mimicking real gene expression data for educational purposes.

This dataset allows for a range of data science tasks suitable for a workshop setting, including data preprocessing, exploratory 
data analysis, feature engineering, and building classification models. It also provides a real-world context that can be highly 
engaging for participants in the life sciences field.

### Prompt 5:
Using gene expression data requires a lot of domain specific knowledge from the area of bioinformatics. Please suggest a more 
broadly applicable example.
GPT

ANSWER:
For a more broadly applicable dataset for part 2.2 of your workshop, which is focused on using tidymodels in a life sciences 
and chemistry context, we could consider a dataset related to environmental monitoring. Environmental data is relevant to a 
wide range of disciplines within the life sciences and chemistry, and it doesn't require as specialized domain knowledge as 
gene expression data.
Example Dataset: Air Quality and Pollution Dataset
Overview:

    This dataset contains measurements of various pollutants and environmental factors, such as particulate matter (PM2.5, PM10), Nitrogen Dioxide (NO2), Sulfur Dioxide (SO2), Ozone (O3), as well as environmental conditions like temperature, humidity, and wind speed.
    It is commonly used to monitor and predict air quality, which is crucial for environmental science, public health, and urban planning.

Attributes:

    Pollutant Levels: Continuous variables representing concentrations of various pollutants (e.g., PM2.5, NO2, SO2, O3).
    Meteorological Data: Variables like temperature, humidity, wind speed, and atmospheric pressure.
    Time Stamp: Date and time for each observation.
    Location: Geographic location of the monitoring stations.

Potential Analysis with tidymodels:

    Predictive Models: Building models to forecast air quality index based on environmental and pollutant data.
    Time Series Analysis: Exploring patterns and trends over time in pollutant levels.
    Feature Importance: Determining which environmental factors are most predictive of high pollution levels.

Ethical Considerations:

    Typically, there are fewer ethical concerns with environmental data, but it's always important to cite data sources and use the data responsibly.

Where to Find Similar Datasets:

    Governmental environmental agencies often provide open access to air quality data.
    Online repositories like Kaggle, UCI Machine Learning Repository, or Google Dataset Search.

Using this type of dataset allows participants to engage in meaningful predictive modeling and analysis tasks without the need for 
extensive domain-specific knowledge. It's also highly relevant to current global issues in environmental science and public health, making 
it an engaging choice for a diverse audience.
User

### Prompt 6:
What would be a good example for the 'Healthcare' context?
GPT

For a healthcare context in part 2.2 of your workshop, a good example dataset would be one related to patient health records 
or medical diagnostics. A broadly applicable and engaging choice would be a dataset on diabetes diagnosis. Such datasets are 
commonly used in healthcare analytics for predictive modeling and are suitable for participants with varying levels of medical background.

Example Dataset: Diabetes Patient Records Dataset

Overview:

    This dataset typically contains clinical measurements from patients who are at risk of diabetes or who have already been diagnosed with it.
    It is used to predict the likelihood of a patient developing diabetes based on various health indicators.

Attributes:

    Glucose Level: Plasma glucose concentration a 2 hours in an oral glucose tolerance test.
    Blood Pressure: Diastolic blood pressure (mm Hg).
    Skin Thickness: Triceps skinfold thickness (mm).
    Insulin: 2-Hour serum insulin (mu U/ml).
    BMI: Body mass index (weight in kg/(height in m)^2).
    Diabetes Pedigree Function: A function that represents how likely they are to have diabetes based on family history.
    Age: Age in years.
    Outcome: Class variable (0 or 1) indicating whether the patient has diabetes.

Potential Analysis with tidymodels:

    Classification Models: Developing predictive models to classify patients as diabetic or non-diabetic based on health indicators.
    Risk Factor Analysis: Identifying the most significant predictors of diabetes.
    Data Preprocessing: Handling missing values, normalization, and transforming features for better model performance.

Ethical Considerations:

    Use anonymized data to ensure privacy.
    If real patient data is used, it should be with proper permissions and in compliance with health data regulations like HIPAA.

Where to Find Similar Datasets:

    Public health datasets, such as the Pima Indians Diabetes Database, available in repositories like UCI Machine Learning Repository.
    Synthetic medical datasets designed for educational purposes.

This dataset is ideal for a healthcare-focused audience as it allows for exploring key concepts in medical data analytics, like 
classification and risk prediction, in a straightforward and impactful way. Additionally, diabetes is a common health issue with 
global relevance, making the dataset relatable and interesting for participants from diverse backgrounds.

Let's go for this suggestion!

## Where to get such a dataset?
I googled: "Diabetes Patient Records Dataset" and this landed me at Kaggle:
https://www.kaggle.com/datasets/mathchi/diabetes-data-set

Another dataset that we will use for deep learning is the 'Diabetes' dataset at [UCI:](http://archive.ics.uci.edu/dataset/34/diabetes)
Original source and citation: Kahn, Michael. Diabetes. UCI Machine Learning Repository. https://doi.org/10.24432/C5T59G.

Downloading the dataset can be done without registering an account at Kaggle or UCI.

## Alternative dataset on sustainability
In oder to accomodate a different audianece and research theme, I promted GPT-4 for an alternative more geared toward engineering.

### Prompt 7:

What dataset recommendation do you have for the research field of 'egineering' that is also part of the knowledge center? Preferably something that would demonstrate forcasting using machine learning.
GPT

For the research field of engineering within the Knowledge Center, particularly with a focus on demonstrating forecasting using machine learning, a suitable dataset could be related to energy consumption or production. One specific example is a dataset on electricity demand forecasting. Such datasets are commonly used in engineering research for optimizing energy systems, integrating renewable energy sources, and planning infrastructure investments.
Example Dataset: Electricity Demand Forecasting Dataset
Overview:

    This dataset typically includes historical electricity consumption data along with various influencing factors such as time (hour, day, month, year), weather conditions (temperature, humidity, wind speed), and special events (holidays, industrial activity).
    It's used to forecast future electricity demand, which is a critical aspect of energy management in engineering.

Attributes:

    Electricity Consumption: The amount of electricity consumed in a specific time period (e.g., hourly, daily).
    Time Variables: Hour of the day, day of the week, month, year.
    Weather Conditions: Temperature, humidity, wind speed, possibly solar irradiance for regions with significant solar power.
    Special Events: Public holidays, industrial activities, and other events that might affect electricity usage.
    Other Possible Variables: Economic indicators, population movement data, etc.

Potential Analysis with Machine Learning:

    Time Series Forecasting Models: Using historical data to predict future electricity demand.
    Feature Importance Analysis: Identifying key factors that most significantly affect electricity consumption.
    Integrating Renewable Energy Data: For regions with significant renewable energy (like solar or wind), analyzing how this integration impacts overall electricity demand.

Ethical Considerations:

    The dataset should be used in a way that respects privacy and proprietary information, especially if it includes data from specific households or businesses.

Where to Find Similar Datasets:

    Publicly available datasets from government or energy departments.
    Datasets from energy competitions on platforms like Kaggle.
    Synthetic datasets that simulate real-world electricity consumption patterns.

This type of dataset allows for a range of analyses suitable for a workshop setting, including preprocessing, exploratory analysis, and building forecasting models. It’s also directly relevant to current challenges in energy management and sustainable engineering, making it an engaging choice for an engineering-focused audience.

A quick search on Google showed the availability of this data in [Kaggle](https://www.kaggle.com/datasets/nicholasjhana/energy-consumption-generation-prices-and-weather).

## Workshop datasets and materials
To illustrate a number of possibilities for the use of AI in the prediction of Diabetes, I have prepared (with help of GPT-4) some materials to be run in the Statiscal & Data Science Programming environment R. See files:

 - `./exploratory-data-analysis.Rmd`
 - `./machine-learning.Rmd`
 - `./deep-learning.Rmd`

As you see, before we dive into the modelling aspects of the data, we explore the data first to see what we have.

## Building models with GPT-4
ChatGPT can also help you build models.Both GPT-3.5 and GPT-4 are very good in writing code. In the workshop materials I have included the promts that I used to construct the basic code. Obviously, you need to have specific knowledge about how to apply Machnine Learning algorithms and for tasks which models can be used. Also, ChatGPT makes mistakes in the sybtax, so you have to have sufficient programming skills to fix bugs and errors. Furthemore, sometimes the code is written in a old-fashioned style. When that happens, I usually rewrite the code to fit a more modern style. For this workshop I chose to write the models and anlyses in R, but I could also have chosen Python.
