## Welcome to the Division of Psychiatry ABCD Data User Manual

Compiled by Niamh MacSweeney (niamh.macsweeney@ed.ac.uk). If you spot any errors or have information to add, please get in touch! 

## Background 

The purpose of this manual is to provide you with the information needed to access and work with the ABCD data. You should only access this data if you have been named on the most recent Data User Certificate (DUC) approved by the NDA. If you have any queries about the DUC, please contact niamh.macsweeney@ed.ac.uk or heather.whalley@ed.ac.uk. The most recent DUC is dated November 2021. 

All named recipients on the DUC need to create an NDA acccount with **University of Edinburgh** listed as their institution. You can create a NDA account at this link: https://nda.nih.gov/user/create_account.html


## Getting Started

Before you start planning your own ABCD Study, you should check what research using the ABCD data has been published to date. We recommend checking the following databases/lists to get idea of what has been done with the data so far (note, these resources are not comprehensive and may be overlapping but they are a good starting point)

1. Existing studies of ABCD data found on the ABCD Study website under the <a href="https://abcdstudy.org/publications/">Publications tab </a>
2. NDA "<a href="https://nda.nih.gov/general-query.html?q=query=studies%20~and~%20dataRepositories=Adolescent%20Brain%20Cognitive%20Development%20~and~%20orderBy=id%20~and~%20orderDirection=Ascending">Data from Papers </a> page also has a list of studies that use ABCD data (please see Acknowledgements section for further info on creating an NDA study ID -         you must do this prior to submitting any ABCD paper for publication. 
3. Preregistered studies that plan to use ABCD data can be found on platforms like the <a href= "https://osf.io/search/"> Open Science Framework </a> 

Once you have an idea of existing ABCD research, it is recommended that you consult the following resources before working with the ABCD Data:

1. ABCD Study Protocols: <a href="https://abcdstudy.org/scientists/protocols/">https://abcdstudy.org/scientists/protocols/</a>

    The ABCD Study has excellent documentation of assessment protocols for every wave. At a high level, data collection protocols outline the following: an annual comprehensive battery of physical health, mental health, substance use, culture and environment, and biospecimens; a bi-annual (every 24 months) MRI scan; and intermediate mid-year phone assessments of youth behavior, substance use, and affect.
    
    You are also encouraged to consult existing literature that uses ABCD data to see if there are any published guidelines or protocols for your variables of interest. For example, guidelines for working with the imaging (e.g., <a href="https://doi.org/10.1016/j.neuroimage.2019.116091">Hagler et al., 2019</a> ;<a href="https://doi.org/10.1038/s41593-021-00867-9"> Chaarani et al., 2021</a>), cognition (<a href="https://doi.org/10.1016/j.dcn.2018.02.006">Luciana et al., 2018</a>), puberty measures (<a href="https://doi.org/10.3389/fendo.2021.608575">Cheng et al., 2021</a>; <a href="https://dx.doi.org/10.3389%2Ffendo.2020.549928">Herting & Uban, et al., 2021</a>), assessment of culture and environment (<a href="https://doi.org/10.1016/j.dcn.2021.101021">Gonzales et al., 2021</a>) and substance use behavior (<a href="https://doi.org/10.1016/j.dcn.2018.02.007">Lisdahl et al., 2018</a>) have been published to date.


2. This preprint: “<a href="https://psyarxiv.com/aqckx"> A practical guide for researchers and reviewers using the ABCD Study and other large longitudinal datasets</a> 

    This paper is intended as a guide for researchers and reviewers working with ABCD data, highlighting the features of the data (and the strengths and limitations therein) as well as relevant analytical and methodological considerations. It arose out of discussions from the Modelling Developmental Change ABCD Workshop held in July 2021. It is strongly encouraged that you consult this document when designing your ABCD project as the information contained within provides an excellent (and fairly comprehensive) framework to ease you into working with large, multi-modal datasets like ABCD. It also goes into greater details about the resources listed below (e.g., ABCD workshop, data dictionary, DEAP etc.) 
    
    
    **NOTE** - The paper is currently under review at Developmental Cognitive Neuroscience as a Next Gen Tools paper. This page will be updated once the final version is available. 
    
    
3. Modelling Developmental Change ABCD Workshop Website:  <a href="https://abcdworkshop.github.io">https://abcdworkshop.github.io</a>

    There are SO many amazing resources on this website including lectures, videos, hands-on tutorials and code. Niamh MacSweeney attended the 2021 workshop so if      you have any questions, please reach out to her. 
        
 4. ABCD Data Dictionary: <a href="https://nda.nih.gov/data_dictionary.html?source=ABCD%2BRelease%2B4.0&submission=ALL">Found at this link</a>

    The data dictionary is a good resource for checking variable names within specific measures. See “<a href="https://psyarxiv.com/aqckx"> "Practical guide for researchers" paper </a> for a detailed walk through of the data dictionary. 
    
 5. Data Exploration Analysis Portal (DEAP; <a href="https://deap.nimhda.org/applications/User/login.php?url=/index.php">deap.nimhda.org<a/>)
    
    Researchers with NDA access (your DEAP login details are the same as your NDA ones) are granted access to DEAP a statistical analysis platform wherein researchers can readily engage with the ABCD data, such as exploring variables, downloading data, or running analyses. This is really handy for quickly checking what variables exist within ABCD, and is a bit easier to navigate than the data dictionary. You can also create personalised data frames with variables from different measures (e.g., age, sex, BDI) by adding the variables of interest "to your cart" and then downloading your dataframe as a .Rdata file. This is explained in more detail in the "Practical guide" paper and is a lifesaver for creating covariate dataframes because it saves you from extracting the variables of interest from lots of different individual data frames (i.e., .Rds or .txt files).  
    
  6. ABCD ReproNim course: <a href= "https://www.abcd-repronim.org">https://www.abcd-repronim.org<a/>

 This is a fairly lengthy course but is broken up into specific topics and focuses on reproducible analysis methods. It is a good way to familiarise yourself with your research area through an "ABCD lens" and also discusses the design and development of the baseline data collection. 



## How do I access the data?

ABCD data is managed by Niamh MacSweeney (niamh.macsweeney@ed.ac.uk) and Gladi Thng (j.g.thng@sms.ed.ac.uk). The earlier releases of the ABCD data were managed by X.Shen and a huge thanks to Shen for the help with the data management of the current release!

The ABCD Study team have an annual curated data release around November each year. The most recent **data release (4.0)** was made available in early November 2021. The data managers downloaded this curated data release and converted the .txt files into .Rds files. All of the ABCD files are stored in .Rds format but if you would like the files in .txt format, please get in touch to the data managers. 

The ABCD data is stored on the GenScotDepression DataStore (**not on the Eddie GenScotDepression**). DataStore is a University computer storage cluster and the GenScotDepression is our designated storage space. GenScotDepresison is managed by Dr Mark Adams (Research Fellow in the Division of Pyschiatry). If you do not already have access to the GenScotDepression DataStore, please get in touch with Mark (mark.adams@ed.ac.uk) and kindly ask him to grant you access to this shared storage. We recommend creating your own personal folder within the user folder, e.g., users/your_name and keeping all your files associated with ABCD there. 
    
Please note that the copy of the data on DataStore is **read-only** to avoid any accidental changes being made to the data. You should be able to read the data into your analysis software of choice from this file. 
    
If anyone is having issues with conflicting working directories in RMarkdown — please get in touch with Niamh (your Rmd file and data need to be in the same working directory which isn't possible with how the ABCD data is stored in DataStore but there is an easy workaround for this!)

### File path for ABCD Data and associated documents 

**On DataStore, the ABCD data is stored at the following folder path: /GenScotDepression/data/abcd/release4.0/iii.data**

We have categorised the data into different folders such as Mental_Health, Physical_Health, MRI_T_roi, MRI_QC etc. 

In order to understand the data contained within each folder, you need to:

1. Consult the **ABCD Master Data dictionary file** (Master_abcd4_wcat_data_dictionary.csv) which is located in: ../data/abcd/release4.0/iii.data
    This data dictionary details every variable contained within the data release. You can filter by category (e.g., Mental_Health) to make navigating the spread sheet easier.
    
    As a starting point, you should get the "short name" of your measure of interest from the <a href="https://nda.nih.gov/data_dictionary.html?source=ABCD%2BRelease%2B4.0&submission=ALL"> ABCD Data Dictionary </a> because the .Rds files in the ../iii.data folder correspond to the "short name" measures listed in the data dictionary. For example, the "short name" for the ABCD Parent Child Behavior Checklist Raw Scores Aseba (CBCL) is "abcd_cbcl01" on the ABCD data dictionary and the associated .Rds file is "abcd_cbcl01.rds", which can be found in the "../iii.data/Mental_Health folder. 

2. You also NEED to consult the **ABCD release 4.0 notes**, which can be found at this folder path: /Volumes/GenScotDepression/data/abcd/release4.0/release_notes in order to understand any changes that have been made to your measures of interest since the last data release. 


## Working with ABCD data 

The ABCD Study team strongly encourage transparent and reproducibible research methods. Software like RMarkdown, which allows you to weave together narrative text and code, can be very useful in making your workflow reproducible because you can document each decision made in the data processing and quality control steps. 
    
The ABCD study team very much encourage researchers to pre-register their analyses on platforms like the OSF. Further details about pre-registration can be found in the “<a href="https://psyarxiv.com/aqckx"> "Practical guide for researchers" paper </a> linked above. 
    
 ### ABCD Research Topics and Areas of Expertise
    
Ideally, we would like to create resource whereby group members can list the kinds of ABCD data they have worked with. This could then serve as a directory that people could consult when starting projects and will aid sharing code and expertise within the group. 
    
    
   -  Niamh MacSweeney (niamh.macsweeney@ed.ac.uk): Structural (T1, DTI) imaging data; puberty (physical and hormonal) data; depression (KSADS, CBCL) measures; demographic measures. 


### Acknowledgements 
    
When preparing your ABCD manuscript for publication, please make sure you consult and follow the information outlined on the NDA website, which can be found at this <a href="https://nda.nih.gov/get/manuscript-preparation.html">link </a>
    
  Special thanks for X. Shen, Mark Adams, and Gladi Thng for their assistance with data management. 

