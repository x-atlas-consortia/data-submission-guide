## Section 7 - Local Validation

**NOTE:** TMCs are required to run the submission validation locally BEFORE uploading to Globus. 
  - <span style="background-color: aquamarine;"> Clinical assays do not need to complete this step.</span>
  
**IMPORTANT:** When a new version of a metadata schema is generated, it will be published on the _first_ day of the _next_ month.

**Locally validate the submissions directory:** Use the _validate_submission.py_ code, following the instructions in the <a href="https://hubmapconsortium.github.io/ingest-validation-tools/">README</a>.
  - **Run the validation code.** This code validates the submission directory content against the appropriate assay-specific metadata & data directory schema.
  - **Correct any errors.** Repeat until no errors occur.
  - A successful validation run will end with a **"No errors!"** message.

Contact the <a href="mailto:help@hubmapconsortium.org">HuBMAP Helpdesk</a> OR <a href="mailto:help@sennetconsortium.org">SenNet Helpdesk</a> for assistance with _persistent_ errors.
