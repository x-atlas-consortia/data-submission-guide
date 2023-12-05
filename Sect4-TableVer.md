## Section 4 - Registering RUI Tissue Block Locations

When registering an organ (sample) on HuBMAP or SenNet which is supported in the Human Reference Atlas (HRA), you must register a tissue block for the sample with the HRA using the Registration User Interface (RUI).

|Step | Comments |
|:---------------------------------------|:------------------------------------------------------------------------|
|Accessing the RUI | The RUI is embedded in the sample registration page but the option only appears... <br> &nbsp; • When registering a tissue block (sample) from a supported organ.  <br> &nbsp; • Metadata such as author name, date, etc. is captured as part of the tissue ingest process. <br> &nbsp; • RUI data is automatically associated with the tissue block on Globus.|
|RUI information requirements | &nbsp; • Tissue block length, width, and height dimensions (expressed in mm) <br> &nbsp; • Tissue block placement relative to a Human Reference Atlas 3D Reference Organ <br> &nbsp; • Entry of all anatomical structures that are a part of the tissue block|
|**Spatial Registration** | As of February 2022, the RUI supports HRA Tissue Block registration for more than 50 organs.|
|&nbsp; 1. Is your organ supported? | Open the <a href="https://hubmapconsortium.github.io/ccf-ui/rui/">standalone version of the RUI</a> and check the organ carousel.|
|&nbsp; 2. Gather materials ... | Needed to document from where (in the subject) the tissue block was extracted.|
|&nbsp; 3. Open the RUI | &nbsp; • Open the relevant version of the RUI (standalone or ingest portal version). <br> &nbsp; • The _Select an organ_ dialog displays when you browse to the RUI webpage.|

**NOTE:** For more detailed instructions, refer to the SOP: <a href="https://zenodo.org/record/6628366#.ZAYfdXbMJD8">Using the CCF Registration User Interface</a>.

|Step | Comments |
|:---------------------------------------|:------------------------------------------------------------------------|
|**Donor sex and organ selection:** | Some steps vary depending on whether you are using the "public" or HuBMAP's ingest portal version.|
|&nbsp; 1. Enter the donor’s name | This step is the same for both versions.|
|&nbsp; 2. Select the donor’s sex  | This step is the same for both versions.|
|&nbsp; 3. Organ selection | &nbsp; • _Public version_: <br> &nbsp; &nbsp;  ‣ Click the picture of an organ to select it from the carousel. <br> &nbsp; &nbsp;  ‣ If applicable, select the right or left version of the organ. <br> &nbsp; &nbsp;  ‣ The organ may take a few seconds to load. <br> &nbsp; • _Ingest portal version_: The organ is pre-selected. |
|&nbsp; 4. Click **Start Registration** | To complete this step and display the CCF Registration page. |
|**Tissue Placement** | **TIP:** First time using the RUI? Review the _Description of the User Interface (UI)_ section in the <a href="https://zenodo.org/record/6628366#.ZAYfdXbMJD8">SOP</a>.|
|&nbsp; **‣ Adjusting opacity** | All anatomical structures are set to **20%** opacity by default. <br> &nbsp; • This makes “looking inside” reference organs easier. <br> &nbsp; • Use the _Anatomical Structures_ accordion menu in the left (metadata) pane to adjust the opacity.|
|&nbsp; **‣ Resizing a tissue block** | Use the _Tissue Block Dimensions_ text input fields in the top right corner. <br> &nbsp; • The default is a **10 x 10 x 10 mm** (L x W x H) block. <br> &nbsp; • Enter tissue section thickness in millimeters.|
|&nbsp; **‣ Moving a tissue block** | There are 3 methods for moving a tissue block into position:|
|&nbsp; &nbsp; **a. Mouse** | When using the mouse, the tissue block can only be moved in _two_ dimensions at a time. |
|&nbsp; &nbsp; **b. X, Y, Z axis sliders** | Adjust the rotation of the tissue block using the X, Y, Z axis sliders in the right (manipulation) pane.|
|&nbsp; &nbsp; **c. A, D, W, S, Q, E keys** | Move the tissue block by pressing these keys on your keyboard. <br> &nbsp; • Each key press moves the tissue block by **0.5 mm** in a positive or negative direction. <br> &nbsp; • Each pair of keys represent a dimensional axis: <br> &nbsp; &nbsp; **‣ A—D = X** axis <br> &nbsp; &nbsp; **‣ W—S = Y** axis <br> &nbsp; &nbsp; **‣ E—Q = Z** axis <br> &nbsp; • This control method can be used in both the Register and 3D Preview modes. |
|&nbsp; **‣ Inspecting placed blocks** | Click the **Previously Registered Blocks** toggle button in the left pane. <br> &nbsp; • This lets you inspect tissue blocks you placed before (for reference).|
|&nbsp; &nbsp; a. Click the toggle button | To show all previously registered tissue blocks based on your browser’s local cache. <br> &nbsp; • This feature is supported in most browsers. |
|&nbsp; &nbsp; b. Radio buttons (3D pane) | Change the perspective using these radio buttons.|
|&nbsp; &nbsp; c. 3D Preview mode | To verify placement, switch to this mode using the corresponding toggle switch at the top of the 3D pane.|
|&nbsp; Click **Register Location** | Review your registration data, then click the **Register Location** button. <br> &nbsp; • Your data will be saved and shared and the RUI window will close automatically. |
