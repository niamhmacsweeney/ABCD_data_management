ABCD structural imaging files - data dictionary
================
Miruna Barbu, Niamh MacSweeney, Nikolaj Høier
04/03/2022

### ABCD imaging data files

The following document contains information on ABCD imaging data, from
**release 4.0**. It is a resource that presents what type of information
is available, what imaging modalities are available, variables in each
modality, and any notes to keep into account. It also includes the
latest research on each modality within the ABCD cohort. We would
appreciate if new papers are uploaded as they are found, in each
modality’s section.

The resource additionally includes the latest information on QC criteria
for all modalities. In release 4.0, this has been made especially easy
as there is an “img\_incl” variable for each modality (more information
below).

#### Quality check information

Meeting Prep: What things do we need to consider?

-   What files do you need to load? Make a list for each modality and
    associated QC file (recommended file and short name)
-   What QC variable should you use for each modality (e.g., cortical,
    subcortical, DTI)? Consult Imaging Release 4.0 Notes
-   Let’s make a standardised QC script (look at Nikolaj and Niamh’s -
    adapted from Shen)
-   Need to consider covariates for imaging - what are the essential
    ones, how are we controlling for things like hemisphere, motion,
    scanner, site? Do we need to do any additional analysis when
    incorporating these covariates (e.g., testing for interaction
    effects).
-   Modelling - ideally, we would have a script that can be used (and
    understood) by members of the imaging group to examine assocaitions
    between imaging variables and other constructs of interest (e.g.,
    mental health, puberty, enivonmental factors)
-   GOAL - to have an approved script for imaging QC that all members of
    group are happy with so that we have a uniform and consistent
    approach for all our ABCD work.
-   Ideally, we will apply a similar approach to our statistical models
    (to be discussed at our stats meeting)
-   Wrap up - let’s find a date for our stats meeting.

#### DTI

|                      Name of instrument                       |    Short name    | N variables |
|:-------------------------------------------------------------:|:----------------:|:-----------:|
|                     ABCD dMRI DTI Part 1                      | abcd\_dti\_p101  |     760     |
|                     ABCD dMRI DTI Part 2                      | abcd\_dti\_p201  |     425     |
|         ABCD dMRI DTI Destrieux Parcellations Part 1          | abcd\_ddtidp101  |     980     |
|         ABCD dMRI DTI Destrieux Parcellations Part 2          | abcd\_ddtidp201  |     830     |
|                   ABCD dMRI DTI Full Part 1                   | abcd\_dmdtifp101 |     767     |
|                   ABCD dMRI DTI Full Part 2                   | abcd\_dmdtifp202 |     218     |
|       ABCD dMRI DTI Full Destrieux Parcellations Part 1       | abcd\_ddtifp101  |     980     |
|       ABCD dMRI DTI Full Destrieux Parcellations Part 2       | abcd\_ddtifp201  |     840     |
|  ABCD dMRI RSI Part 1 (RNI: restricted normalized isotropic)  |  abcd\_drsip101  |             |
| ABCD dMRI RSI Part 2 (RND: restricted normalized directional) |  abcd\_drsip201  |             |
|    ABCD dMRI RSI Part 3 (RNT: restricted normalized total)    |  abcd\_drsip301  |             |
|   ABCD dMRI RSI Part 4 (HNI: hindered normalized isotropic)   |  abcd\_drsip401  |             |
|  ABCD dMRI RSI Part 5 (HND: hindered normalized directional)  |  abcd\_drsip501  |             |
|     ABCD dMRI RSI Part 6 (HNT: hindered normalized total)     |  abcd\_drsip601  |             |
|     ABCD dMRI RSI Part 7 (FNI: free normalized isotropic)     |  abcd\_drsip701  |             |

DTI variables in the ABCD cohort. (continued below)

|                                                                                                                                                   Description                                                                                                                                                    |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| INNER SHELL: Average FA, MD, LD, and TD in DTI atlas; fiber tract volume in mm (DTI atlas); average FA, MD, LD, and TD within ASEG ROIs; average FA, MD, LD, and TD within parcellations of sub-adjacent white matter for cortical ROIs; Average FA and MD within parcellations of gray matter for cortical ROIs |
|                                                                                                 INNER SHELL: Average LD and TD in cortical gray matter; Average FA, MD, LD, and TD in gray-white matter contrast                                                                                                 |
|                                                                                            INNER SHELL: Average FA, MD, TD, and LD in white matter; Average FA, MD, and LD in gray matter; all within Destrieux Atlas                                                                                            |
|                                                                                  INNER SHELL: Average TD in gray matter within Destrieux Atlas; Average FA, MD, LD, and TD in gray-white matter contrast within Destriux Atlas                                                                                   |
| FULL SHELL: Average FA, MD, LD, and TD in DTI atlas; fiber tract volume in mm (DTI atlas); average FA, MD, LD, and TD within ASEG ROIs; average FA, MD, LD, and TD within parcellations of sub-adjacent white matter for cortical ROIs; Average FA and MD within parcellations of gray matter for cortical ROIs  |
|                                                                                                                       FULL SHELL: Average FA, MD, LD, and TD in gray-white matter contrast                                                                                                                       |
|                                                                          FULL SHELL: Average FA, LD, TD, and MD within parcellations of sub-adjacent white matter; FA, LD, and MD within parcellations of gray matter (Destrieux Atlas                                                                           |
|                                                                                       FULL: Average LD and TD in grey matter (Destrieux Atlas); Average FA, MD, LD, and TD in gray-white matter contrast (Destrieux Atlas)                                                                                       |

##### Recommendations for DTI variable use:

1.  Full and inner shell derivation of DTI measures: differences between
    the two (taken from dMRI release 4.0)

Two modeling approaches

● DTI inner shell (DTIIS): b values &gt; 1000 excluded from tensor
fitting to avoid need for nonlinear estimation; metric prefix is “dti”

● DTI full shell (DTIFS): all b values used in the tensor fitting;
metric prefix is “dti\_full”

2.  abcd\_ddtidp101 and abcd\_ddtidp201: transverse diffusivity in gray
    matter is in abcd\_ddtidp201, while FA, MD, and LD all in
    abcd\_ddtidp101.

3.  Release notes: noted as abcd\_dmdtifp202; dataset + ABCD data
    dictionary: abcd\_dmdtifp201

4.  abcd\_ddtifp101 : no online data dictionary

#### Cortical

#### Subcortical Volumes

|           Name of instrument            |   Short name    | N variables |
|:---------------------------------------:|:---------------:|:-----------:|
|            ABCD sMRI Part 1             | abcd\_smrip102  |     474     |
|            ABCD sMRI Part 2             | abcd\_smrip202  |     360     |
|            ABCD sMRI Part 3             | abcd\_smrip302  |     360     |
| ABCD sMRI Destrieux Parcellation Part 1 | abcd\_mrisdp102 |     604     |
| ABCD sMRI Destrieux Parcellation Part 2 | abcd\_mrisdp202 |     604     |
| ABCD sMRI Destrieux Parcellation Part 3 | abcd\_mrisdp302 |     452     |

Cortical and subcortical variables in the ABCD cohort. (continued below)

|                                                                                             Description                                                                                              |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
|        Measurement in mm and weighted-average (genetically derived parcellation with multiple clusters) for: thickness, volume, surface area, sulcal depth; subcortical volumes measurements         |
|                Average and weighted-mean T1 intensity of white matter and gray matter; cort-contrast white and gray matter (genetically derived parcellation with multiple clusters)                 |
|                Average and weighted-mean T2 intensity of white matter and gray matter; cort-contrast white and gray matter (genetically derived parcellation with multiple clusters)                 |
|                                                    Measurement in mm mapped to Destrieux atlas for: thickness, volume, surface area, sulcal depth                                                    |
| Average and weighted-mean T1 intensity of white matter and gray matter; cort-contrast white and gray matter (genetically derived parcellation with multiple clusters); all mapped to Destrieux atlas |
| Average and weighted-mean T2 intensity of white matter and gray matter; cort-contrast white and gray matter (genetically derived parcellation with multiple clusters); all mapped to Destrieux atlas |

##### Recommendations for cortical and subcortical variable use:

#### Resting state (maybe we should do this in a separate file)

##### Recommendations for resting state variable use:

### Latest research

#### General methods articles

[Image processing and analysis methods for the Adolescent Brain
Cognitive Development Study, Hagler et
al. 2019](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6981278/)

#### Used in research

[(PREPRINT) White matter microstructure shows sex differences in late
childhood: Evidence from 6,797 children, Lawrence et
al. 2021](https://www.biorxiv.org/content/10.1101/2021.08.19.456728v1.abstract)

[Psychotic-like Experiences and Polygenic Liability in the Adolescent
Brain Cognitive Development Study, Karcher et
al. 2022](https://www.sciencedirect.com/science/article/pii/S2451902221001919?via%3Dihub)
