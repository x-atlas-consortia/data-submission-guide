---
layout: default
---

## Section 6 - Preparing Metadata 
This section provides links to access relevant metadata templates, and provides information for assays that include antibodies or assay-specific channel IDs.
Click the provided links in this section to access additional relevant information or resources.

**Create metadata files.** Download and complete the latest version of each required metadata template:
  - assay-specific
  - <a href="https://hubmapconsortium.github.io/ingest-validation-tools/contributors/current/">contributors</a>
  - <a href="https://hubmapconsortium.github.io/ingest-validation-tools/antibodies/current/">antibodies</a> (if relevant) 
  
  Lists of assay-specific templates are available from the HuBMAP consortium’s <a href="https://hubmapconsortium.github.io/ingest-validation-tools/">Data Upload Guidelines</a> page.
  
  **Note:** Many HuBMAP metadata schemas are shared by SenNet. The <a href="https://docs.sennetconsortium.org/libraries/ingest-validation-tools/schemas/source-murine">murine source schema</a> is _unique_ to SenNet.

1. **Assay-specific templates** 
   - Clicking on an assay type (on the page linked above) takes you to a page for that type.
   - Select the <strong>Excel template</strong> on that page.
   - Each page includes field name descriptors, format requirements.
2. **<a href="https://hubmapconsortium.github.io/ingest-validation-tools/contributors/current/">Contributors template</a>** 
   - Lists the names, institutions, and ORCID ID's of contributors to the dataset.
   - If _ALL_ datasets listed in your assay metadata use the same set of contributors, you may submit just one contributors file.
   - Point to the file in the <em>contributors_path</em> field for the corresponding datasets.
3. **<a href="https://hubmapconsortium.github.io/ingest-validation-tools/antibodies/current/"> Antibodies template</a>** 
   - Required for all assays that use antibodies.
   - If _ALL_ datasets in your assay metadata use the same set of antibodies, you may submit just one <em>antibodies</em> file.
     
**NOTE:** A separate antibody _validation report_ is also required. 

**If datasets in the submission use _Different sets_ of antibodies — OR —  the same set, but different lots...**
  - Each unique antibody set must be listed in a separate _antibody.tsv_ with a unique name:
      - (e.g., dataset<font color=red>1</font>_antibodies.tsv, dataset<font color=red>2</font>_antibodies.tsv, etc).
      - Different lot numbers for different datasets
  - **Custom antibodies**
      - Indicate the batch date (_format: yyyy-mm-dd_) in the lot_number field.
  - **Assay-specific channel_id**
      - The _channel_id_ field in the antibodies TSV is populated with assay-specific information in the following formats:
          - **CODEX: cycle#_CH#** > The cycle/channel information is generated by the <em>Akoya</em> instrument used for CODEX.
          - **Cell DIVE: cycle#_CH#** > The following 3 assays do not involve cycles:
              - **Light sheet:** _channel_id_ is the name of the _fluorophore_ tag on the antibody.
              - **MIBI:** _channel_id_ is the name of the _metal_ tag on the antibody.
              - **IMC:** _channel_id_ is the name of the _metal_ tag on the antibody.

**Check for RRID registration:** If an RRID (Research Resource Identifier) has _not_ been assigned for an antibody, <a href="http://antibodyregistry.org">register the antibody</a>.
