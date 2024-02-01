## Section 3 - Validating Metadata
Directions for adding Metadata for an organ or samples and validating that metadata. Note that the procedures for uploading the validated metadata currently differ between HuBMAP and SenNet.
Click the provided links in this section to access additional relevant information or resources.

<ol>
  <li> <b>Download metadata template(s):</b> Access lists of metadata schemas (and related information) from HuBMAP’s <a href="https://hubmapconsortium.github.io/ingest-validation-tools/">Data Upload Guidelines</a> page.</li>
  <b>Note:</b> Many HuBMAP metadata schemas are shared by SenNet. The <a href="https://docs.sennetconsortium.org/libraries/ingest-validation-tools/schemas/source-murine">murine source schema</a> is <em>unique</em> to SenNet. 
  <ul>
    <li> Download and complete Excel metadata template(s) for organ or sample types:</li>
    <ul> 
      <li> <a href="https://hubmapconsortium.github.io/ingest-validation-tools/organ/">organ</a></li>
      <li> <a href="https://hubmapconsortium.github.io/ingest-validation-tools/sample-block/">sample - block</a></li>
      <li> <a href="https://hubmapconsortium.github.io/ingest-validation-tools/sample-section/">sample - section</a> </li>
      <li><a href="https://hubmapconsortium.github.io/ingest-validation-tools/sample-suspension/">sample - suspension</a> </li>
    </ul>
    <li> Click on any assay or sample type on the lists to jump to a page for that type. </li> 
    <ul>
      <li> Select the <b>Excel template</b> on that page.</li>
    </ul>
  </ul>
  <li> <b>Is a template missing any categorical values</b> (that you need for specific fields: instrument name, researcher ID, etc.)? </li>
  <ul>
    <li> Contact the <a href="mailto:help@hubmapconsortium.org">HuBMAP Helpdesk</a> OR <a href="mailto:help@sennetconsortium.org">SenNet Helpdesk</a> to add these value(s) to the relevant template.</li>
    <li> When making this request, identify the specific Excel template, fields, and categorical values needed.</li>
    <b>NOTE:</b> Adding new values to a field can take time, so please plan ahead.
  </ul>
  <li> <b>Validate your metadata spreadsheet (template)</b> using the <a href="https://metadatavalidator.metadatacenter.org/"> Metadata Spreadsheet Validator</a>. This tool: </li>
  <ul>
    <li> Validates metadata spreadsheets against specifications stored in the CEDAR repository.</li>
    <li> Categorizes any errors found and provides hints on how to fix those errors. </li>
    <li> <a href="https://metadatacenter.github.io/spreadsheet-validator-docs/">Help documentation</a> for the Validator: </li>
    <ul> 
      <li> Includes a user manual and tutorial videos.</li>
      <li> Will assist you with fixing any errors your metadata spreadsheet may contain.</li>
    </ul>
    <li> TMCs are required to validate their metadata BEFORE uploading it to the HIVE or CODCC.</li>
  </ul>
</ol>
  
### Validation procedure
  
Follow the steps outlined below to validate any metadata spreadsheet (except Donor metadata) using the Validator.
  1. **Upload completed template** - Upload your completed Excel spreadsheet (metadata template) to the Validator (see link above).
  2. **Click "Start Validating" to check your spreadsheet.**
     - Any detected errors will display.
     - If errors are detected, use the Validator tools to correct any errors.
     - When no errors are found, you may safely upload your spreadsheet.
  4. **Download corrected template** - Once all errors are corrected, download the <em>corrected</em> metadata spreadsheet (TSV format).
  5. **Hover the mouse cursor** over the **"Download" button**, then select **TSV format**.
  6. **Need to validate more templates?**  Repeat steps **1 - 4** (above) to validate additional metadata spreadsheets.
  7. **Upload validated TSVs:**
     - HuBMAP:
         - Send validated (organ or sample) metadata TSV files to the <a href="mailto:help@hubmapconsortium.org">HuBMAP Helpdesk</a>
         - The Helpdesk will manually validate and upload the files.
      - SenNet:
         - Use the <em>Upload Metadata</em> dropdown from the <em>Navigation Bar</em> in the <a href="https://data.sennetconsortium.org/search">SenNet Data Sharing portal</a>
         - Select the type of metadata: (<em>Mouse</em> or <em>Organ, Block, Section,</em> or <em>Suspension</em> — sample types).</li>

**NOTE:** To learn more about metadata validation, see also the <a href="https://docs.google.com/document/d/1lfgiDGbyO4K4Hz1FMsJjmJd9RdwjShtJqFYNwKpbcZY/edit#heading=h.d6xf2xeysl78">Metadata Validation Workflow</a>.
