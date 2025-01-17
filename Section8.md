---
layout: default
---

## Section 8 - Creating an Upload Directory
This section describes the basic steps needed to create an upload directory to submit metadata and data uploads to the HIVE (HuBMAP) or CODCC (SenNet). <b>NOTE:</b> The steps required for this differ for <span class="txt--highlight">_Clinical_</span> versus _non-Clinical_ assays. _Prerequisite:_ The submission directory has been successfully validated locally.

<ol>
    <li> <b>Getting started</b> </li> 
        <ul>
            <li>HuBMAP members:</li>
              <ul>
              <li>On the <a href="http://ingest.hubmapconsortium.org">HuBMAP ingest portal</a></li>
              <li>Register a single donor, sample, dataset, or publication or bulk register samples or data.</li> 
              </ul>
            <li>SenNet members: </li>
              <ul>
              <li>On the <a href="http://data.sennetconsortium.org/search">SenNet Data Sharing portal</a></li> 
              <li>Register a single source, sample, dataset, or publication or bulk register samples or data.</li>
              </ul>
          </ul>
    <li><b>From the Navigation bar:</b></li>
        <ul>
           <li>HuBMAP members select <b>REGISTER NEW > BULK  > Data </b></li>
           <li>SenNet members select: <b>Create an Entity > Data </b></li> 
           <li>This action initiates the data upload process.</li>
         </ul>
     <li><b>Complete the required fields</b> - Select a title that both you and the HIVE or CODCC can use to recognize the data upload. </li>
     <li><b>Click "Create"</b> - This creates a Globus folder where you upload your dataset files. </li>
     <li><b>Setting up an upload directory</b> - Upload directories have several required components. At minimum, three parts are necessary: </li>
         <ul>
           <li><b>An assay metadata file</b> ending in "metadata.tsv" that has been validated using the <a href="https://metadatavalidator.metadatacenter.org/">HuBMAP Metadata Spreadsheet Validator</a>. A list of supported assays can be found <a href="https://docs.hubmapconsortium.org/metadata">here</a>.</li>
           <li><b>A contributors metadata file</b> ending with a title of "contributors.tsv" that has been validated using the <a href="https://metadatavalidator.metadatacenter.org/">HuBMAP Metadata Spreadsheet Validator</a>. The contributors metadata template can be found <a href="https://hubmapconsortium.github.io/ingest-validation-tools/contributors/current/">here</a>.</li>
           <li><b>Data files required by the assay's directory schema.</b> A list of supported assays can be found <a href="https://docs.hubmapconsortium.org/metadata">here</a>. Each dataset should have a corresponding subdirectory containing all the files in the directory schema. Each row of the metadata file should reference one of these subdirectories via the data_path field.</li>
         </ul>
     <li><b>Need to add or modify files?</b> - Follow the highlighted Globus link. </li>
        <ul>
            <li><b>Save:</b>  To make changes to the <em>Title</em> or <em>Description</em> fields use the <b>Save</b> button.</li>
            <li><b>Submit:</b> Click <b>Submit</b> once all data has been uploaded to Globus.</li> 
            <li>Contact the <a href="mailto:help@hubmapconsortium.org">HuBMAP Helpdesk</a> if further processing by the HIVE is needed. </li>
            <li>Contact the <a href="mailto:help@sennetconsortium.org">SenNet Helpdesk</a> if further processing by the CODCC is needed. </li>
       </ul>
</ol>

<b>EPICs</b>

EPICs (Externally Processed Integrative Collections) allow data providers to upload non-HIVE biological interpretations to the HIVE for publication on the HuBMAP Data Sharing Portal. The process for submitting EPICs to the HIVE is similar to the process above. Metadata and directory schemas can be found on the schema documentation under <a href="https://docs.hubmapconsortium.org/metadata">EPICs</a>. However, EPICs may have additional files that need to be uploaded, such as objects-by-feature matrices for Segmentation Masks. These details are documented on the relevant schema pages.

<span class="txt--highlight">This section is for Clinical Assays only:</span>

<ol>
    <li> <b>Email the <a href="mailto:help@hubmapconsortium.org">HuBMAP Helpdesk</a> OR <a href="mailto:help@sennetconsortium.org">SenNet Helpdesk</a> when ready to upload.</b></li>
    <ul>
        <li> Be sure to use an institutional email address (e.g. <em>name@institution.edu).</em></li>
        <li> The Help desk relays this request for space on the protected endpoint to the Pitt team.</li>
        <li> The Pitt team provides the assay team with the protected data endpoint.</li>
    </ul>
    <li> <b>Upload your data as compressed / zipped folders, using Globus.</b></li>
</ol>

<span class="txt--highlight">**IMPORTANT:** This location is distinct from where NON-Clinical HIVE or CODCC data is uploaded. </span>
