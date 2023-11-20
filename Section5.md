## Section 5 - Preparing a Submissions Directory

**NOTE:** The steps below are shared by both _Clinical_ and _non-Clinical_. <span style="background-color: aquamarine;">Highlighted items apply to Clinical assays only.</span>

|Step | Comments |
|:---------------------------------------|:------------------------------------------------------------------------|
|Prepare a Submissions Directory | Use for submitting datasets to the HIVE (HuBMAP) or CODCC (SenNet).|
|&nbsp; Set up the submissions directory:| Based on assay-specific directory schema for each assay in Github: <br> &nbsp; • (e.g. <a href="https://hubmapconsortium.github.io/ingest-validation-tools/codex/">CODEX Directory structure</a>). <br> &nbsp; • These requirements are defined via a collaborative process. |
|&nbsp; 1. Include these items: | &nbsp; &nbsp; ‣ One assay metadata spreadsheet per assay type (e.g. assay_metadata.tsv) |
| | &nbsp; &nbsp; ‣ One contributor’s metadata spreadsheet per dataset (e.g. contributors.tsv) |
| | &nbsp; &nbsp; ‣ One antibody metadata spreadsheet  per dataset—if applicable—(e.g. antibodies.tsv) |
| | &nbsp; &nbsp; ‣ One data directory for each dataset |

**Next steps for non-Clinical (most) assays.** This includes ANY assay type _except_ the specific clinical types listed below.

|Step | Comments |
|:---------------------------------------|:------------------------------------------------------------------------|
|&nbsp; 2. Assay-specific directory schema |Access via GitHub link (e.g., <a href="https://software.docs.hubmapconsortium.org/assays/codex">CODEX example</a>) or <a href="https://software.docs.hubmapconsortium.org/metadata">HuBMAP metadata specifications</a> in the portal. |
|&nbsp; 3. Organize the dataset | Components (i.e., data and metadata files) in a submission directory according to the required <br> directory structure specified in the GitHub page for the assay (e.g., <a href="https://github.com/hubmapconsortium/ingest-validation-tools/tree/main/docs/codex">CODEX directory structure</a>).|

<span style="background-color: aquamarine"> **Next steps for Clinical assays (ONLY)**. Clinical assays include the following: <strong>Body CT, MRI, MicroCT, OCT,</strong> and <strong>Ultrasound</strong>.</span>

|Step | Comments |
|:---------------------------------------|:------------------------------------------------------------------------|
|<span style="background-color: aquamarine">&nbsp; 2. Create a root directory </span> | <span style="background-color: aquamarine">Inside this directory place the metadata.tsv and contributors.tsv files.</span>|
|<span style="background-color: aquamarine">&nbsp; 3. Create a data subdirectory </span> | <span style="background-color: aquamarine">(Datadir) Inside the root directory — When all the files are ready, compress the root directory <br> using a utility (e.g. tar or .zip) to reduce its file size for submission.</span>|

<span style="background-color: aquamarine"> **NOTE:** Clinical assays may have protected patient information (PPI) embedded in the metadata or images. <br> &nbsp; • PPI <em>must</em> be removed before the metadata or images are made available through HuBMAP. <br> &nbsp; • This process allows us to review and remove the information in a way that is Institutional Review Board (IRB) compliant.</span>

|Step | Comments |
|:---------------------------------------|:------------------------------------------------------------------------|
|&nbsp; 4. Extras directory (optional) | (<span style="background-color: aquamarine">Clinical</span> and Non-Clinical) <br> Use this optional directory for any other files your team wants to include. <br> **NOTE:** The contents of this directory will not be vetted by the HIVE. <br> **IMPORTANT** - Do NOT include TMC-processed data in the extras directory.|
