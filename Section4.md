## Section 4 - RUI Tissue Blocks
When registering an organ (sample) on HuBMAP or SenNet which is supported in the Human Reference Atlas (HRA), you must register a tissue block for the sample with the HRA using the Registration User Interface (RUI).

**Accessing the RUI** - The RUI is embedded in the sample registration page.
- The RUI option only appears when registering a tissue block (sample) from a supported organ.
- Metadata such as author name, date, etc. is captured as part of the tissue ingest process.
- RUI data is automatically associated with the tissue block on Globus.

**RUI information requirements:**
- Tissue block length, width, and height dimensions (expressed in mm)
- Tissue block placement relative to a Human Reference Atlas 3D Reference Organ
- Entry of all anatomical structures that are a part of the tissue block

**Spatial Registration** - As of February 2022, the RUI supports HRA Tissue Block registration for more than 50 organs.
1. **Is your organ supported?** Open the <a href="https://hubmapconsortium.github.io/ccf-ui/rui/">standalone version of the RUI</a> and check the organ carousel.
2. **Gather materials needed** to document from where (in the subject) the tissue block was extracted.
3. **Open the RUI:** Open the relevant version of the RUI (standalone or ingest portal version).
   - The _Select an organ_ dialog displays when you browse to the RUI webpage.
   - If applicable, select the right or left version of the organ.

**NOTE:** For more detailed instructions, refer to the SOP: <a href="https://zenodo.org/record/6628366#.ZAYfdXbMJD8">Using the CCF Registration User Interface</a>.

**Donor sex and organ selection:**  
**Note:** Step 3 varies depending on whether you are using the "public" or HuBMAP's ingest portal version.
1. Enter the donor’s name.
2. Select the donor’s sex.
3. Organ selection (Varies based on the version you are using). <br>
_Public version_:
   - Click the picture of an organ to select it from the carousel.
   - The organ may take a few seconds to load. <br>
   
   _Ingest portal version_: The organ is pre-selected.
4. Click **Start Registration** to complete this step and display the CCF Registration page. 

### Tissue Placement
 **TIP:** First time using the RUI? Review the _Description of the User Interface (UI)_ section in the <a href="https://zenodo.org/record/6628366#.ZAYfdXbMJD8">SOP</a>.

**Adjusting opacity:** 
   - All anatomical structures are set to **20%** opacity by default.
   - This makes “looking inside” reference organs easier.
   - Use the _Anatomical Structures_ accordion menu in the left (metadata) pane to adjust the opacity.

**Resizing a tissue block**
   - Use the _Tissue Block Dimensions_ text input fields in the top right corner.
   - The default is a **10 x 10 x 10 mm** (L x W x H) block.
   - Enter tissue section thickness in millimeters.

**Moving a tissue block:** There are 3 methods for moving a tissue block into position.
   - **Mouse:** When using the mouse, the tissue block can only be moved in _two_ dimensions at a time.
   - **X, Y, Z axis sliders:** Adjust the rotation of the tissue block using the X, Y, Z axis sliders in the _right_ pane.
   - **A, D, W, S, Q, E keys:** Move the tissue block by pressing these keys on your keyboard.
        - Each key press moves the tissue block by **0.5 mm** in a positive or negative direction.
        - Each pair of keys represent a dimensional axis:
             - **A—D = X** axis
             - **W—S = Y** axis
             - **E—Q = Z** axis
        - This control method can be used in both the _Register_ and _3D Preview_ modes.

**Inspecting placed blocks:** Click the **Previously Registered Blocks** toggle button in the _left_ pane. 
   - This lets you inspect tissue blocks you placed before (for reference).
      - Click the toggle button to show all previously registered tissue blocks based on your browser’s local cache.
      - This feature is supported in most browsers.
   - **Radio buttons (3D pane):** Change the perspective using these radio buttons.
   - **3D Preview mode:** To verify placement, switch to this mode using the corresponding toggle switch at the top of the 3D pane.

**Register Location:** Review your registration data, then click the **Register Location** button.
   - Your data will be saved and shared and the _RUI window_ will close automatically. 
