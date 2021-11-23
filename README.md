## Welcome to the Division of Psychiatry ABCD Data User Manual

Compiled by Niamh MacSweeney (niamh.macsweeney@ed.ac.uk). If you spot any errors or have information to add, please get in touch! 

### Background 

The purpose of this manual is to provide you with the information needed to access and work with the ABCD data. You should only access this data if you have been named on the most recent Data User Certificate (DUC) approved by the NDA. If you have any queries about the DUC, please contact niamh.macsweeney@ed.ac.uk or heather.whalley@ed.ac.uk. The most recent DUC is dated November 2021. 

All named recipients on the DUC need to create an NDA acccount with **University of Edinburgh** listed as their institution. You can create a NDA account at this link: https://nda.nih.gov/user/create_account.html


### Getting Started

To begin, it is recommended that you consult the following resources before working with the ABCD Data:

1. This preprint: “A practical guide for researchers and reviewers using the ABCD Study and other large longitudinal datasets" doi: to go here

    This paper is intended as a guide for researchers and reviewers working with ABCD data, highlighting the features of the data (and the strengths and limitations therein) as well as relevant analytical and methodological considerations. It arose out of discussions from the Modelling Developmental Change ABCD Workshop held in July 2021. It is strongly encouraged that you consult this document when designing your ABCD project as the information contained within provides an excellent (and fairly comprehensive) framework to ease you into working with large, multi-modal datasets like ABCD. It also goes into greater details about the resources listed below (e.g., ABCD workshop, data dictionary, DEAP etc.) 
    
    **NOTE** - The paper is currently under review at Developmental Cognitive Neuroscience as a Next Gen Tools paper. This page will be updated once the final version is available. 
    
    
 2. Modelling Developmental Change ABCD Workshop Website: https://abcdworkshop.github.io

    There are SO many amazing resources on this website including lectures, videos, hands-on tutorials and code. Niamh MacSweeney attended the 2021 workshop so if      you have any questions, please reach out to her. 
        
 3. ABCD Data Dictionary: https://nda.nih.gov/data_dictionary.html?source=ABCD%2BRelease%2B2.0&submission=ALL

    The data dictionary is a good resource for checking variable names within specific measures. See "Practical guide" paper for a detailed walk through of the data dictionary. 
    
 4. Data Exploration Analysis Portal (DEAP; deap.nimhda.org)
    
    Researchers with NDA access are granted access to DEAP a statistical analysis platform wherein researchers can readily engage with the ABCD data, such as exploring variables, downloading data, or running analyses. This is really handy for quickly checking what variables exist within ABCD, and is a bit easier to navigate than the data dictionary. You can also create personalised data frames with variables from different measures (e.g., age, sex, BDI) by adding the variables of interest "to your cart" and then downloading your dataframe as a .Rdata file. This is explained in more detail in the "Practical guide" paper and is a lifesaver for creating covariate dataframes because it saves you from extracting the variables of interest from lots of different individual data frames (i.e., .Rds or .txt files).  
    
    5. ABCD ReproNim course: https://www.abcd-repronim.org

    This is a fairly lengthy course but is broken up into specific topics and focuses on reproducible analysis methods. It is a good way to familiarise yourself with your research area through an "ABCD lens" and also discusses the design and development of the baseline data collection. 



### How do I access the data?

ABCD data is managed by Niamh MacSweeney (niamh.macsweeney@ed.ac.uk) and Gladi Thng (j.g.thng@sms.ed.ac.uk). The ABCD Study team have an annual curated data release around November each year. The most recent data release (4.0) was made available in early November 2021. The data managers downloaded this curated data release and converted the .txt files into .Rds files. All of the ABCD files are stored in .Rds format but if you would like the files in .txt format, please get in touch to the data managers. 


## File path for ABCD Data and associated documents 

The ABCD data is stored at the following folder path: /Volumes/GenScotDepression/data/abcd/release4.0/iii.data

We have categorised the data into different folders such as Mental_Health, Physical_Health, MRI_T_roi, MRI_QC etc. 

In order to understand the data contained within each folder, you need to:

1. Consult the ABCD Master Data dictionary file (Master_abcd4_wcat_data_dictionary.csv) which is located in: ../data/abcd/release4.0/iii.data
    This data dictionary details every variable contained within the data release. You can filter by category (e.g., Mental_Health) to make navigating the spread sheet easier.
    
    As a starting point, you should get your field name of interest from the "ABCD data dictionary" (e.g., abcd_cbcl01) 

3. Consult the ABCD release 4.0 notes, which can be found at this folder path: /Volumes/GenScotDepression/data/abcd/release4.0/release_notes
4. Look at the ABCD data dictionary



The ABCD release notes 

If you do not already have access to the GenScotDepression DataStore, please get in touch with Mark Adams (mark.adams@ed.ac.uk) and kindly ask Mark to grant you access to this shared storage. We recommend creating your own personal folder within the user folder, e.g., users/your_name and keeping all your files associated with ABCD there. 

## Working with ABCD data 

The ABCD Study team strongly Transparency and reproducibility are very important 




```Getting Started

To begin, it is recommended that you consult the following resources before working with the ABCD Data:

1. This preprint: “A practical guide for researchers and reviewers using the ABCD Study and other large longitudinal datasets" doi: to go here

    This paper is intended as a guide for researchers and reviewers working with ABCD data, highlighting the features of the data (and the strengths and limitations        therein) as well as relevant analytical and methodological considerations

ABCD Data Dictionary: https://nda.nih.gov/data_dictionary.html?source=ABCD%2BRelease%2B2.0&submission=ALL
    
    The ABCD data dictionary 

    

# How do I access the data?

ABCD data is managed by Niamh MacSweeney (niamh.macsweeney@ed.ac.uk) and Gladi Thng (j.g.thng@sms.ed.ac.uk). The ABCD Study team have an annual curated data release around November each year. The most recent data release (4.0) was made available in early November 2021. The data managers downloaded this curated data release and converted the .txt files into .Rds files. All of the ABCD files are stored in .Rds format but if you would like the files in .txt format, please get in touch to the data managers. 


## File path for ABCD Data and associated documents 

The ABCD data is stored at the following folder path: /Volumes/GenScotDepression/data/abcd/release4.0/iii.data

We have categorised the data into different folders such as Mental_Health, Physical_Health, MRI_T_roi, MRI_QC etc. 

In order to understand the data contained within each folder, you need to:

1. Consult the ABCD release 4.0 notes, which can be found at this folder path: /Volumes/GenScotDepression/data/abcd/release4.0/release_notes
2. Look at the ABCD data dicto



The ABCD release notes 

If you do not already have access to the GenScotDepression DataStore, please get in touch with Mark Adams (mark.adams@ed.ac.uk) and kindly ask Mark to grant you access to this shared storage. We recommend creating your own personal folder within the user folder, e.g., users/your_name and keeping all your files associated with ABCD there. 

## Working with ABCD data 

The ABCD Study team strongly Transparency and reproducibility are very important 



## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/niamhmacsweeney/ABCD_data_management/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
