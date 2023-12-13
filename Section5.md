## Section 5 - Submissions Directory Prep
This section decribes setting up the submissions directory. Some directions differ for <span style="background-color: aquamarine;">_Clinical_</span> versus _non-Clinical_ assays. 
Most steps are shared by both <span style="background-color: aquamarine;">_Clinical_</span> and _non-Clinical_ assays, except as noted below.

<hr>

Prepare a Submissions Directory. Use this directory for submitting datasets to the HIVE (HuBMAP) or CODCC (SenNet).
  - Set up the directory based on the assay-specific directory schema for each assay in Github: (e.g. [CODEX Directory structure](https://hubmapconsortium.github.io/ingest-validation-tools/codex/)).
  - These requirements are defined via a collaborative process.

1. Include these items:
   - One assay metadata spreadsheet per assay type (e.g. assay_metadata.tsv)
   - One contributor’s metadata spreadsheet per dataset (e.g. contributors.tsv)
   - One antibody metadata spreadsheet  per dataset—if applicable—(e.g. antibodies.tsv)
   - One data directory for each dataset 

**Next steps for non-Clinical (most) assays.** This includes ANY assay type _except_ the specific clinical types listed below.

  2. Assay-specific directory schema. Access via GitHub link (e.g., <a href="https://software.docs.hubmapconsortium.org/assays/codex">CODEX example</a>) or <a href="https://software.docs.hubmapconsortium.org/metadata">HuBMAP metadata specifications</a> in the portal. 
  3. Organize the dataset components (i.e., data and metadata files) in a submission directory according to the required directory structure specified in the GitHub page for the assay (e.g., <a href="https://github.com/hubmapconsortium/ingest-validation-tools/tree/main/docs/codex">CODEX directory structure</a>).

<hr>

<span style="background-color: aquamarine;"> 
<b>Next steps for Clinical assays (ONLY)</b>. Clinical assays include the following: <b>Body CT, MRI, MicroCT, OCT,</b> and <b>Ultrasound</b>.

  2. Create a root directory. Inside this directory place the metadata.tsv and contributors.tsv files.
  3. Create a data subdirectory inside the root directory. When all the files are ready, compress the root directory using a utility (e.g. tar or .zip) to reduce its file size for submission.

 <b>NOTE:</b> Clinical assays may have protected patient information (PPI) embedded in the metadata or images.
   - PPI <em>must</em> be removed before the metadata or images are made available through HuBMAP.
   - This process allows us to review and remove the information in a way that is Institutional Review Board (IRB) compliant. </span>

<hr>

4. Extras directory (optional, used by both Clinical and Non-Clinical assays).
   - Use this optional directory for any other files your team wants to include.
   
**NOTE:** The contents of this directory will not be vetted by the HIVE. 
**IMPORTANT:** Do NOT include TMC-processed data in the extras directory.
