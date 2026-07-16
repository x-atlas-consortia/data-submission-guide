---
layout: default
---

# Data Submission Guide

This resource documents the key steps of uploading data to the [SenNet Data Sharing Portal](https://data.sennetconsortium.org/search). While data upload consists of multiple components, it is important to understand that these components can be accomplished simultaneously, which allows data providers to work more efficiently, greatly mitigates delays and results in data being published in a timely manner. Keep in mind that data upload can only be done by registered consortium members. To register, contact the SenNet Help Desk.

## Data Upload Components

|    Source Registration   | Metadata Collection and Validation | Experimental Data Upload |
|    --------    | -------- | -------- |
|<b>Register a donor or source</b><br><br>From the [SenNet Data Sharing Portal](https://data.sennetconsortium.org/search), select Create an Entity > Source<br><br><b>Register an organ or sample</b><br><br>In addition to Organ, there are three sample types: Block, Section, and Suspension.<br><br>To register a new human organ or sample, select Create an Entity > Sample:<br> - Select the appropriate field from the Sample Category drop-down.<br>- If <b>organ</b> is selected, select the organ type from the dropdown list.<br><br>A [murine source schema](https://docs.sennetconsortium.org/libraries/ingest-validation-tools/schemas/source-murine) is available for murine sources.<br><br>If registering an organ that is supported in the HRA, it must be [registered using the RUI](https://docs.google.com/document/d/1vKf7xIQ2QegE5qMrdn6bUbLce5nl2rjnetze_3pfMIk/edit?tab=t.0#bookmark=id.c4v78uiwyset).<br><br>[More about Source Registration](#source-registration)|<b>Required metadata templates</b><br><br>[Assay-specific](https://hubmapconsortium.github.io/ingest-validation-tools/current) and [contributors](https://hubmapconsortium.github.io/ingest-validation-tools/contributors/current/) metadata are required for all datasets.<br><br><b>Antibodies metadata</b><br><br>An [antibodies metadata template](https://hubmapconsortium.github.io/ingest-validation-tools/antibodies/current/) is required for all assays that incorporate antibodies. <br><br>Assay-specific, contributors and anti metadata spreadsheets must be validated using the [Metadata Spreadsheet Validator](https://metadatavalidator.metadatacenter.org/) prior to upload.<br><br><b>Human donor metadata</b><br><Br>[Human donor metadata](#human-donor-metadata) must be uploaded directly to a secure Globus directory. Contact the Help Desk for write permission and additional direction.<br><br>[More about Metadata](#metadata)<br><br><br><br><br><br>|<b>Register datasets</b><br><br>From the [SenNet Data Sharing Portal](https://data.sennetconsortium.org/search), select Create an Entity > Data<br><br><b>Create a Globus directory</b><br><br>Complete all required fields and click Create<br><br><b>Upload files to Globus</b><br><br>Upload all data files required by the [assay-specific directory schema](https://docs.hubmapconsortium.org/metadata).<br><br>Once all files have been uploaded, click Submit and notify the Help Desk that the datasets are ready to be validated and ingested.<br><br>[More about Dataset Uploads](#dataset-uploads)<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>|

## <a id="source-registration">Source Registration</a>
When registering a source, do not include protected health information about a donor or source, organ, or specimen.
### Donors and Sources
A [murine source schema](https://docs.sennetconsortium.org/libraries/ingest-validation-tools/schemas/source-murine) is available for SenNet data providers.
### Samples and Organs
Before registering a sample or organ, the associated donor or source must be registered. The Source ID field represents the organ or sample’s parent, the donor. The Ancestor ID field represents the organ or sample’s source.You also need the ID of the organ and the DOI (from [protocols.io](http://protocols.io/)) for the case selection protocol.

<b>Tissue blocks:</b> If the sample is a tissue block, upload a thumbnail image file using the following naming convention: [block_submission_id].[jpg]. Thumbnails should be 800 x 600 pixels and in JPEG or PNG format. For additional information, see the [Images SOP](https://docs.google.com/document/d/1swtxxF9z8Llnptqk4eNvgDpYUwDrViI78KbRI3b1jXg/edit#heading=h.cd53uti4az4).

# <a id="metadata">Metadata test4</a>

## Assay-specific metadata
[Assay-specific metadata](https://hubmapconsortium.github.io/ingest-validation-tools/current) is required for all datasets. If you have assay data that you plan on uploading, but which is not yet supported, contact the Help Desk. 

## Contributors.tsv
A [Contributors metadata file](https://hubmapconsortium.github.io/ingest-validation-tools/contributors/current/) is required for all datasets. This file must be pointed to the assay-specific metadata’s contributors_path field for the corresponding datasets. If all datasets listed in your assay metadata use the same set of contributors, you may submit a single contributors file. 

## Antibodies.tsv 
An [antibodies metadata template](https://hubmapconsortium.github.io/ingest-validation-tools/antibodies/current/) is required for all assays that use antibodies. If all datasets in your assay metadata use the same set of antibodies, you may submit a single antibodies file. A separate antibody validation report is also required for all submissions.

<b>Unique antibody sets:</b> If datasets in the submission use unique sets of antibodies, or use the same set, but with unique Lot IDs, each unique antibody set must be listed in a separate antibodies.tsv with a unique name:
Custom antibodies; If using custom antibodies, indicate the batch date (format: yyyy-mm-dd) in the lot_number field.

<b>Assay-specific channel_id:</b> The channel_id field in the antibodies TSV is populated with assay-specific information in the following formats:
- CODEX: cycle#_CH# > The cycle/channel information is generated by the Akoya instrument used for CODEX
- Cell DIVE: cycle#_CH# > The following 3 assays do not involve cycles:
  - Light sheet: channel_id is the name of the fluorophore tag on the antibody
  - MIBI: channel_id is the name of the metal tag on the antibody
  - IMC: channel_id is the name of the metal tag on the antibody

<b>RRID (Research Resource Identifier) registration:</b> If an [RRID](http://antibodyregistry.org/) has not been assigned for an antibody, it should be registered prior to upload of the dataset.

##  Metadata Validation 
The [Metadata Spreadsheet Validator](https://metadatavalidator.metadatacenter.org/) validates metadata templates against specifications stored in the CEDAR repository and categorizes any errors, as well as provides hints on how to resolve those errors.Refer to the Validator [documentation](https://metadatacenter.github.io/spreadsheet-validator-docs/) for additional information .

<b>Requesting new categorical values:</b> If, while completing your metadata schemas you identify any categorical values that need to be added, contact the Help Desk to open a ticket. When making this request, identify the specific metadata template, the field, and the categorical value(s) needed. Please keep in mind that adding new values can take time, so plan ahead.

# <a id="human_donor_metadata">Human Donor Metadata</a>
Human donor metadata must be uploaded directly to a dedicated directory in a secure Globus endpoint. Human donor metadata should never be included with a dataset upload or sent directly to the Data Curation team or Help Desk. 

Human donor data is curated by hand by honest brokers within the consortia. For this reason, there are no specifications or limits on this data. There are four required fields (age, sex, race and living/deceased) along with the donor’s Source ID, but can include any clinical data. It can also be uploaded in any common file format (including .xlsx, .csv, .txt, .pdf). 

To upload human donor data: 
1. The data provider PI should email the Help Desk (and cc the data uploader) requesting the specified data uploader be given Write permission to the provider’s secure donor directory. The request should also include the data uploader’s Globus Identity and Globus ID.
2. Once permission is granted, the data uploader is able to upload donor data.  
3. Once the data has been uploaded, notify the Help Desk or the honest broker to initiate the ingestion process.

<b>Note:</b> Write permission to the secure Globus endpoint is granted for a period of 90 days, but can be renewed by contacting the Help Desk.

# <a id="dataset_uploads">Dataset Uploads</a>

## EPICS
EPICs (Externally Processed Integrative Collections) allow data providers to upload non-CODCC biological interpretations to the SenNet for publication on the SenNet Data portal.

For more information, refer to the [overview of EPICs](https://docs.hubmapconsortium.org/EPICs/) and [EPIC specifications](https://docs.hubmapconsortium.org/metadata).

# Additional Topics
## Registering Experimental Protocols
All experimental protocols, each requiring a digital object identifier (DOI), must be registered via [protocols.io](https://www.protocols.io/welcome). Note that there are three types of required protocols: 
- <b>Case selection protocols</b> describe the inclusion and exclusion criteria applied to donors/sources in the study. 
- <b>Sample preparation protocols</b> outline a lab’s procedure to derive a tissue sample from a donor/source. 
- <b>Assay preparation protocols</b> describe how an experiment for a specific modality is carried out. 

## Registering an organ using the HRA RUI: 
The RUI is embedded in the sample registration page and only appears when registering a tissue block (sample) from a supported organ. Metadata such as author name, date, etc. is captured as part of the tissue ingest process. To determine if your organ is supported, open the [standalone version of the RUI](https://hubmapconsortium.github.io/ccf-ui/rui/) and check the organ carousel.

Organ registration requires the following:
- Tissue block length, width, and height dimensions, in mm
- Tissue block placement relative to a Human Reference Atlas 3D Reference Organ
- Entry of all anatomical structures that are a part of the tissue block

For detailed organ registration instructions, refer to [Using the CCF Registration User Interface](https://zenodo.org/record/6628366#.ZAYfdXbMJD8).

### Best Practices
<b>Immediate Spatial Registration Post-Sectioning:</b> Prioritize conducting spatial registrations directly after sectioning tissue samples whenever possible. This approach helps preserve the accuracy of spatial information and minimizes morphological alterations that might occur over time.

<b>Detailed Documentation of Extraction Site:</b> In scenarios where immediate spatial registration is impractical, carefully document the extraction site. Use photographs and detailed annotations on anatomical images to accurately capture the original location and orientation of the tissue. Such documentation can aid subsequent registration efforts.

<b>Preserving Context:</b>
- For diseased tissue, clinical imaging, surgeon’s operative notes (if available), and pathology notes can provide insights into the specific characteristics and conditions of the tissue.
- For normal tissue, communication between the surgeon, the tissue collector, and the specimen collection manager can improve documentation accuracy and handling of tissue samples

<b>Aligning Tissue Using Anatomical Landmarks:</b> The Anatomical Landmarks pane on the bottom left side of the RUI interface serves as a useful reference for orienting tissue samples and navigating reference organs.

<b>Cross-Training on the RUI:</b> Ensure that multiple team members are trained in using the RUI to prevent processing bottlenecks. Having several proficient RUI users allows for continuity in work, even in the absence of key personnel.

#### Tissue Registration Issues
If you have doubts about whether the tissue sample can or should be spatially registered, proceed with the registration process while documenting the issue. In case your tissue sample is missing metadata or there is another issue that you would like to report, open [this Google Form](https://docs.google.com/forms/d/e/1FAIpQLSe0faIih0S-1zqn5FCdalCF7YTxK7ECMgg0svVv0dvlEF7gKQ/viewform) and follow the required steps. Based on the nature of your issue, you will either be granted an exemption from registration or asked to document the issue and proceed.

## dbGaP submission
The submission of data to that dbGaP study is a joint process undertaken by both the data provider and the CODCC. We encourage data providers to create a dbGaP study and notify the CODCC as early as possible, as the dbGaP submission process can take up to six months after the publication of your sequence data in the SenNet Data Sharing portal.

All datasets from the same data provider should be submitted to the same study. For any questions regarding this, please contact the Help Desk.

To begin dbGaP submission:
1. The Data Provider PI should follow the [process outlined here](https://sharing.nih.gov/genomic-data-sharing-policy/submitting-genomic-data/how-to-register-and-submit-a-study-in-dbgap) to identify an NIH Genomic Program Administrator (GPA) who will help them prepare a study for dbGaP. 
2. The Data Provider PI and NIH GPA register a study in the [dbGaP Submission System](https://dbgap.ncbi.nlm.nih.gov/dbgap/ss/dbgapss.cgi?login) and create a Bioproject for the study. This step should be done by the data provider as early as possible, ideally before any data are generated. When establishing a dbGaP study, please ensure the title of the study starts with “SenNet”. 
3. The data provider PI or PM identifies a team member as a data submitter. This individual should contact the Help Desk to request a CODCC member to work with on the dbGap data submission. The data provider PI must then add the CODCC data submitter(s) to the dbGaP study on the [NCBI dbGaP submission portal](https://submit.ncbi.nlm.nih.gov/dbgap/).
4. The Data Provider PI or their designated data submitter completes the Submission Portal Questionnaire NCBI dbGaP submission portal for the registered study.
5. Following the [dbGaP instructions](https://www.ncbi.nlm.nih.gov/gap/docs/submissionguide/#astart), the data submitters work together to complete the [dbGaP Submission Guide Templates](https://ftp.ncbi.nlm.nih.gov/dbgap/dbGaP_Submission_Guide_Templates/), which minimally includes the following:
   - [Study Config](https://www.ncbi.nlm.nih.gov/gap/docs/submissionguide/#aconfig)
   - [Subject Consent Dataset & Data Directory](https://www.ncbi.nlm.nih.gov/gap/docs/submissionguide/#asc)
   - [Subject Sample Mapping Dataset & Data Directory](https://www.ncbi.nlm.nih.gov/gap/docs/submissionguide/#assm)
   - [Sample Attributes Dataset & Data Directory](https://www.ncbi.nlm.nih.gov/gap/docs/submissionguide/#asampattr)

The designated data submitter may also need to complete the following files for upload:
- [Mapping Study Samples](https://www.ncbi.nlm.nih.gov/gap/docs/submissionguide/#ncbidb)
- [Subject Phenotypes Dataset & Data Directory](https://www.ncbi.nlm.nih.gov/gap/docs/submissionguide/#crucialdata)
- [Pedigree Dataset & Data Directory](https://www.ncbi.nlm.nih.gov/gap/docs/submissionguide/#aped)
- Study Documents (consent forms, protocols, etc.)

6. The submitters review the checklist to ensure that the Phenotype Datasets and Data dictionary files pass the dbGaP quality control tests, then submit all required forms.
7. The dbGaP Phenotype curator will contact the submitters when the above information has been loaded into dbGaP and entities have received NCBI BioSample and SRA IDs.
8. The CODCC data submitter follows instructions to upload sequencing metadata.
9. After validation of the sequencing metadata, the CODCC data submitter works with a SRA curator to upload raw sequence reads to a protected area of SRA.
10. SRA processes the sequence data and metadata and notifies dbGaP and the submitters.
### Updating an existing dbGaP study
Making any additions or deletions to the data in a published dbGaP study requires creating a new version of the study. Keep in mind that the previous version of the study will no longer be available for download after the new version has been released. 
1. Verify that all of the datasets for the new version have been published on the portal, then complete the [Study Data Outline](https://www.ncbi.nlm.nih.gov/gap/docs/submissionguide/#sdogloss) in the [dbGaP Submission Portal](https://www.ncbi.nlm.nih.gov/gap/docs/submissionguide/#spgloss). 
2. After the new version is created, your GPA will be notified and should complete the registration in the [dbGaP Submission System](https://www.ncbi.nlm.nih.gov/gap/docs/submissionguide/#ssgloss). 
3. Send any consent changes and/or Acknowledgment Statement changes to the GPA.
4. Update the Study Config to include information about all versions of the study (not only the new version), and notify the Help Desk when it is complete. 
5. The CODCC dbGaP team member will work with the data provider to identify changes in the data, and to create and upload required files and data.

<b>Note:</b> For edits to only the Study Config page text, contact the assigned dbGaP curator directly.


<br><br><br>This resource documents the key steps for TMCs, Assay teams, and others who need to upload data to the HuBMAP Data Ingest portal (HuBMAP Consortium) or SenNet Data Sharing Portal (SenNet Consortium).

Links to additional related portals, sites, and other resources are also provided herein.

- Use the _Table of Contents_ to jump to a section of interest. <br>

<hr />
<hr />

### Information on [EPICs](https://docs.hubmapconsortium.org/EPICs/) and [EPIC upload requirements](https://docs.hubmapconsortium.org/EPICs/#minimum-upload-requirements)
  
<hr />

### Information on [Pass Through Dataset Types](https://docs.hubmapconsortium.org/pass-thrus/)

<hr />

### Information on [Publication Page Submission](https://docs.hubmapconsortium.org/Publications/)
