# News


## ANNOUNCEMENT!!

We are very excited to announce that we will be launching a new version of our UCSF cBioPortal that will include de-identified clinical data elements (e.g. vital status) from de-identified clinical data warehouse (CDW) July 2021. This will allow us to enrich the genomics data in the portal with clinical data in a scalable manner. Patient de-identifiers within the portal will utilize those in de-identified CDW in this new version, which will allow you as a researcher to then obtain additional clinical data you want for your cohort directly from de-identified CDW as well.  

In our initial launch, we will be including race, ethnicity, and whether patient is alive or deceased into cBioPortal. Additional clinical data elements we plan to add this calendar year are (de-identified) dates of diagnosis, tumor collection, sequencing, last visit, and death to name a few.  

This new version of the UCSF cBioPortal will also have significant improvements in variant filtering (e.g. removing variants deemed to be benign, common polymorphisms or germline VUSes) and address long-standing issues we have had such as missing structural variants and germline variants. It will also bring in molecular pathologist assigned classification of UCSF500 variants.  We will be able to load more data into the portal with more frequency than we have before.

In other big news, this new version will also include Foundation Medicine data for UCSF patients where a UCSF clinician report.
 
THE NEW VERSION OF CBIOPORTAL WILL REQUIRE ADDITIONAL REGULATORY MEASURES TO BE MET; PLEASE READ CAREFULLY BELOW:

All users must apply for a de-identified CDW account and complete de-identified CDW onboarding if they do not have one already:
<ul>
   <li>Follow ‘First Time Users’ steps found <a href="https://ars.ucsf.edu/de-identified-clinical-data-warehouse">here.</a></li>; you can indicate 'Michelle Turski' as the approver. 
   <li>You will need to have a current attestation form (Statement of Responsibility) on file; users will get a Docusign invitation if their form is not current or signed</li>
   <li>Three training modules need to be completed, two of which most users will likely have already completed (‘CyberSecurity Fundamentals’ & ‘HIPAA101’); the third training module, ‘Your Responsibilities when Working with Clinical Data’ should take less than 15 minutes to complete </li>
   <li>While our new pipeline connecting to de-identified CDW undergoes certification for de-identification, we will need to add all users to an existing IRB for the UCSF cBioPortal research application. For this, there is nothing you as a user need to do, this is more of a FYI. Once our pipeline is certified, which we hope will be the case in the next 3-6 months, we will no longer need to execute this step and will remove cBioPortal users from the IRB.</li>
</ul>

We will continue to remind our users about de-identified CDW training over the next few weeks prior to launch; at launch, if you have NOT completed the training/account request for de-identified CDW, you will no longer have access to data in UCSF cBioPortal.

Any questions or concerns please send to ucsf.cbioportal@ucsf.edu. The UCSF500 data currently in cBioPortal will not disappear but be stored as a separate study you can still access within the portal; we will not however be maintaining this dataset in anyway (no longer adding cases, bug fixes etc).

## README

* Data in portal represents cases signed-out up to June 1st, 2021 and includes mutation, copy number and fusion data. For more information, please refer to the [FAQs](https://cbioportal.ucsf.edu/cbioportal/faq) page ("What data types are in the portal?"). 
    * We will be doing new data releases approximately every 2-3 months
* Report-derived pathogenicity annotations are not yet displayed in portal 
* There are several known bugs we have reported to the cBioPortal development team:
   * H3F3A variants are showing up as H3F3B variants in portal!
* Some fusions as well as SNPs/small indels are not showing up in the portal; we are in the process of investigating the source cause of this.
* Primary site
   * This is derived directly from the UCSF500 report and actually represents the source location of the biopsy; therefore it might not represent the true primary site of the tumor per se. We are working on obtaining the true primary site for cases in the portal.

## June 17th, 2021
Version 3.0 of UCSF cBioPortal released to UCSF community!
  * UCSF500 cases signed-out prior to 1/05/2021
    * 6,937 patients and 7,844 samples
  * Version of UI has been upgraded 3.6.18.


## February 5th, 2021
Version 3.0 of UCSF cBioPortal released to UCSF community!
  * UCSF500 cases signed-out prior to 1/05/2021
    * 5,789 patients and 6,432 samples
  * Version of UI has been upgraded 3.6.3. New Features/Enhancements Include:
  
   (1) **New Feature**: Extended the _Comparison_ tab to support the comparison of altered samples per gene or alteration. In the example shown below, a query              compares NSCLC patients with 1) both mutated and amplified EGFR, 2) mutated EGFR only, and 3) amplified EGFR only
   ![image](https://user-images.githubusercontent.com/840895/78508085-3ea13f80-7752-11ea-8e87-e486061def12.png)
   
   
   (2) **New Feature**: Annotate mutations using the _Mutation Mapper Tool_ on the GRCh38 reference genome:
    [![mutation_mapper_tool_grch38](https://user-images.githubusercontent.com/1334004/79233555-07f4b480-7e37-11ea-9d0a-0cafff434fa5.png)](https://www.cbioportal.org/mutation_mapper)
    
    
   (3) **Enhancement**: using [OQL](https://www.cbioportal.org/oql#oql-modifiers) to query for mutations based on a protein position range. 
![image](https://user-images.githubusercontent.com/840895/84427197-83ce6b80-abf2-11ea-9d18-3a4f4524e545.png)


   (4) **New Feature**: you can now send the OncoPrint data to the [OncoPrinter tool](https://www.cbioportal.org/oncoprinter) for customization.
![image](https://user-images.githubusercontent.com/840895/84318326-3c85a380-ab3c-11ea-97c1-34343cb3e996.png)


   (5) **Enhancement**: Mutational spectrum data can be downloaded from OncoPrint
![image](https://user-images.githubusercontent.com/840895/84322695-68585780-ab43-11ea-9224-a965331e35fc.png)


   (6) **New Feature**: The *Mutations* tab now has the option to show mutation effects for different transcripts / isoforms. Note that some annotation features are only available for the canonical isoform.
![image](https://user-images.githubusercontent.com/840895/88306535-d95d6400-ccd8-11ea-9e64-0c6600f65e50.png)


   (7) **New Feature**: You can now share custom groups in the *Study View* 
    <img width="333" alt="" src="https://user-images.githubusercontent.com/840895/88309724-b7fe7700-ccdc-11ea-969a-28ed8551ffd7.png">
    
    
   (8) **Enhancement**: _Study View_ now allows comparing samples with mutations or copy number alterations in different genes
![image](https://user-images.githubusercontent.com/840895/99558433-ba729400-2991-11eb-9054-1d8751b4d84f.png)


   (9) **New Feature**: Add your own custom data for a sample or patient to use on the study or comparison view
    <img src="https://user-images.githubusercontent.com/1334004/104651553-ce7efd00-5685-11eb-8017-c43f24421e3f.png" width="700">
    
    
  (10) **New Feature**: Show the mutations of a patient inside a pathway schematic using PathwayMapper
   <img src="https://user-images.githubusercontent.com/1334004/104649378-9f1ac100-5682-11eb-91eb-4e0f024a4ded.png" width="700">


  (11) **New Feature**: The Plots tab on _Results View_ now allows you to group alterations by Driver and VUS
    <img src="https://user-images.githubusercontent.com/1334004/104768867-56bfd980-573c-11eb-8e03-5ad86d01f25a.png" width="700">

  
## October 11th, 2020
Version 2.2 of UCSF cBioPortal released to UCSF community!
  * Version of **data** is 2.2
    * UCSF500 cases signed-out prior to 10/1/2020
    * 4,868 patients and 5,381 samples
  * Version of **UI** is 3.2.2 (no change from previous release)
  
## June 23rd, 2020
Version 2.1 of UCSF cBioPortal released to UCSF community!
  * Version of **data** is 2.1
    * UCSF500 cases signed-out prior to 6/8/2020
  * Version of **UI** is 3.2.2 (no change from previous release)
   
## March 17th, 2020
Version 2.0 of UCSF cBioPortal released to UCSF community!

  * Version of **data** is 2.0
    * UCSF500 cases signed-out prior to 2/24/2020
  * Version of **UI** is 3.2.2. New features include:
    * Genome Aggregation Database (gnomAD) population frequencies in the mutations table - see [example](http://bit.ly/2ISHgiu):
 ![gnomad feature news](https://user-images.githubusercontent.com/1334004/59794400-e07c9c00-92a6-11e9-97ea-a79bfc8f3885.gif)
    * Group Comparison Feature: Compare clinical and genomic features of user-defined groups of samples/patients. [View Tutorial](https://www.cbioportal.org/tutorials#group-comparison)
![group-comparison](https://user-images.githubusercontent.com/840895/59052073-40f9eb00-885c-11e9-9ddb-6d036533e5f5.png)
    * Use the new quick search tab on the homepage to more easily navigate to a study, gene or patient:
 ![quick_search_news](https://user-images.githubusercontent.com/1334004/55113078-8f4c7a00-50b4-11e9-9d95-e9a6e1dcda52.gif)
     * Bookmarking or sharing your selected samples as virtual studies with the _share_ icon on the study summary page. [Example: a virtual study of breast tumors](https://www.cbioportal.org/study?id=5a12fd57498eb8b3d5605cd4)

## August 12, 2019
Version 1.0 of UCSF cBioPortal released to UCSF community!

  *  Version of **data** is 1.0
  * Version of **UI** is 1.18.1
