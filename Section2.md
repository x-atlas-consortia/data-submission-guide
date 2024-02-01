## Section 2 - Register Data Sources
Directions for registering donors (in HuBMAP), sources (in SenNet), and organs or samples that derive from those donors or sources. **NOTE:** Both consortia strongly recommend that you collect donor or source information when you get the organ and sample, well before you begin actual preparations to submit data.

### Register a donor or source
  - **Register a donor** via <a href="http://ingest.hubmapconsortium.org">HuBMAP ingest portal</a>. A <em>donor</em> in HuBMAP is an individual from which organs and samples originate.
  - **Register a source** via <a href="https://data.sennetconsortium.org/search">SenNet Data Sharing Portal</a>. A <em>source</em> in SenNet is the organism being studied.
  1. **Search for the donor or source:** Verify that the donor or source has not already been registered.
  2. **From the Navigation bar select:**
     - In HuBMAP: <b>REGISTER NEW > INDIVIDUAL > Donor</b>
     - In SenNet: <b>Create an Entity > Source</b> <br>
  3. **Record donor or source information.** Do <em>NOT</em> include <a href="https://ingest.hubmapconsortium.org/new/donor">protected health information</a> about a donor or source, organ, or specimen. <br>
  4. **Complete registration of the Donor or source:**
     - In HuBMAP click <b>Generate ID</b> to complete the registration process.
     - In SenNet click <b>Submit</b> to complete the registration process.

**IMPORTANT** _Prerequisite:_ Before registering a sample or organ, the associated donor or source <em>must</em> be registered. You also need the ID of the organ and the DOI (from <a href="http://protocols.io">protocols.io</a>) for the case selection protocol.
  
### Register an organ or sample
In addition to <em>organ</em> there are 3 sample types: <em>Block, Section,</em> and <em>Suspension</em>.
  <ol>
    <li> <b>From the Navigation bar select:</b></li>
    <ul>
      <li>In HuBMAP:</li>
      <ul>
        <li> <b>REGISTER NEW > INDIVIDUAL > Sample</b> (used for both organs and samples).</li>
        <li> For organs - Select <b>Organ</b> from the <em>Tissue Sample Type</em> drop down. </li>
        <li> For samples - Select <b>Block, Section,</b> or <b>Suspension</b> from the <em>Tissue Sample Type</em> drop down</li>
      </ul>
      <li>In SenNet:</li>
      <ul>
        <li> <b>Create an Entity > Sample</b> (used for both organs and samples).</li>
        <li> Select the appropriate field from the <em>Sample Category</em> drop-down:</li>
        <ul> 
          <li> <b>block, section, suspension, bodily fluid, organ,</b> or <b>organ piece</b>.</li>
        </ul>
        <li> If <strong>organ</strong> is selected, select the <em>organ type</em> from the dropdown list.</li>
      </ul>
    </ul>
    <li> <b>Record information about the sample.</b> </li>
    <ul> 
      <li> In HuBMAP, the <em>Source ID</em> field represents the organ or sample’s parent, the donor.</li>
      <li> In SenNet, the <em>Ancestor ID</em> field represents the organ or sample’s source.</li>
    </ul>
    <li> <b>If the sample is a tissue block, upload a thumbnail image: </b></li>
    <ul> 
      <li> A stained microscopy image of a tissue section that represents the tissue block. </li> 
      <li> Label the image using this format: <em>[block_submission_id].[jpg]</em>. </li> 
      <li> Preferably, <b>800 x 600</b> pixels, in JPEG or PNG format. </li> 
      <li> See also: the <a href="https://docs.google.com/document/d/1swtxxF9z8Llnptqk4eNvgDpYUwDrViI78KbRI3b1jXg/edit#heading=h.cd53uti4az4">Images SOP. </a></li>
    </ul>
    <li> <b>Does a 3D reference object exist for the organ</b> (as part of the <em>Common Coordinate Framework (CCF)</em>)? </li> 
    <ul> 
      <li> See the <a href="https://hubmapconsortium.github.io/ccf/pages/ccf-3d-reference-library.html"> CCF Portal </a> for a listing of supported organs.</li>
      Yes — click <b>Register Location</b><br>
      No — (no existing CCF)
      <li> To register the sample in CCF Coordinate space see this <a href="https://www.youtube.com/watch?v=142hGer4xvU"> video </a> or download the SOP <a href="https://doi.org/10.5281/zenodo.5575776">here</a>. </li> 
      <li> Contact <a href="infoccf@indiana.edu"> MC-IU </a> if the organ or tissue you are imaging is <em>not</em> represented in the CCF.</li>
    </ul>
    <li> <b>Complete registration of the organ or sample</b></li>
    <ul>
      <li> In HuBMAP click <b>Generate ID</b> to complete the registration process.</li>
      <li> In SenNet click <b>Submit</b> to complete the registration process.</li>
      <li> After an organ or sample is registered, the system will confirm the process and assign an ID for the item.</li>
    </ul>
  </ol>
