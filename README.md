# Data Submission Guide
A documentation site for the Data Submission Guide used by both HuBMAP and SenNet

The Markdown (MD) files in this repo consist of sections in the Data Submission Guide (DSG), a resource for data submitters in the HuBMAP and SenNet Consortia.
The files are syncronized via GitHub Actions to both the SenNet (https://docs.sennetconsortium.org/data-submission) and HuBMAP documentation (https://docs.hubmapconsortium.org/data-submission) sites which are hosted by GitHub Pages via repos https://github.com/sennetconsortium/documentation and https://github.com/hubmapconsortium/documentation respectively. 

Updating and maintaining this content is simply a matter of updating the relevant MD file(s), PR/merge into main as changes are needed, and GitHub will automatically distribute the changes to the dependent documentation sites.

**Note:** Changes to the content for each section are made to the markdown (MD) files in the DSG repository in GitHub's x-atlas-consortia, as described above.
- If the title of any section is modified this will NOT automatically update in the DSG's Table of Contents (TOC).
- To update the TOC, update the "en.json" file located here: https://github.com/hubmapconsortium/documentation/blob/main/docs/lang/en.json
- Take care to only modify the name of the relevant section(s), without making other changes to the JSON file.
- Save the changes and complete a PR/merge to update the TOC as needed.
