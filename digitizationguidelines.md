---
layout: page
title: Digitization Guidelines
permalink: /digitization/
last_modified_date: June 10 2024
---

# {{ page.title }}

This document is intended as a guide to digitization, specifically image and metadata capture for the American Philosophical Society Digital Library. It will be updated as modifications in the equipment, software and/or metadata schema necessitate.

## **Preparing the Work Station**  
Before any digitization takes place, staff should ensure that all of the following conditions have been met:
* Work on a clean, roomy, and tidy work table. Ensure that the work table is large enough to accommodate the objects and their housing enclosures.
Be sure that the scanner bed and workspace are clean and free of dust. Use the lint-free cloths, if necessary.
* Wash and dry hands before working with library materials.
* Determine materials and supplies needed and gather them prior to digitization. This includes book supports, chlorine-free nitrile (medical) gloves for handling photographs, flatbed scanner inserts for digitizing slides, etc.
* Use only pencils near library materials. No ink or felt tip pens or markers, colored pencils, crayons, etc.
* Keep work spaces free of food and drink.
* Close books and folders and cover collection items when leaving the work area.
* Do not leave valuable items unattended while away from the workspace.
* Remove and replace materials in their containers carefully.

## **Handling Materials**
It is vital to assess the physical condition of materials before subjecting them to digitization. Please contact the project supervisor or CDS staff if you have any questions or concerns about digitizing any item or if you encounter any of the following issues:
* Folds or creases obscuring text
* Cockled, undulating paper or photos that would be damaged by scanner pressure
* Tears greater than 1”
* Books with loose joints or detached spines or boards
* Restricted bindings
* Signs of active mold such as soft, furry spots. Active mold is sticky and can smear. Inactive mold is dry and powdery. Excessive powder should be sent to the conservation lab for clean up.
* Difficult formats, such as scrolls, accordion books, panoramas, or oversized items

### **Special Handling Notes**:
* Bound material:
  * BINDINGS: Weak, damaged, or restricted bindings require special care to prevent further damage. Handle, open, and close these items gently and using both hands. During image capture, place these items in a book cradle.
  * BRITTLE PAPER: Handle brittle paper with extreme care. Artwork, documents, manuscripts, prints, photographs, and their mounts can also be brittle. Use clean hands to handle paper.
  * FOLDOUTS: Don’t remove foldouts from books. Carefully open the foldout onto a support (like a board) during image capture.
  * IRON GALL INK: As much as is possible, avoid touching areas of iron gall ink, as this promotes further corrosion.
  * LOOSE ITEMS: A book may contain loose items between its leaves that may need to be temporarily removed to allow digitization of the contents of a given page. Make note of the item’s location, image the item itself, and then immediately replace it following image capture.
  * PAGE FLATTENING: Don’t apply heavy pressure to books in order to flatten them for image capture.  Such pressure can break the spine or loosen or break off brittle pages in a book. If a page cannot be imaged without being held down, options for applying gentle temporary pressure at the edges with book weights, silk thread, or polyethylene straps can be explored with the guidance of a conservator.
* Unbound textual material:
  *  BRITTLE PAPER: Handle brittle paper with extreme care. Artwork, documents, manuscripts, prints, photographs, and their mounts can also be brittle. Use a microspatula and clean hands to handle paper.
  *  IRON GALL INK: As much as is possible, avoid touching areas of iron gall ink, as this promotes further corrosion.
  *  OVERSIZE MATERIAL: Flatbed scanners cannot safely accommodate objects larger than 12.25” x 17” (Epson Expression 12000XL) or 11.5” x 16.5” (Epson GT-15000), therefore oversize material should be scanned on the CopiBook OS XD Book Scanner.

## **Scanning Equipment and Specifications**
The type or medium of a material affects which tools are necessary to digitize it. Bound materials, unbound textual materials, maps and oversized graphic materials require different quality standards and imaging equipment.

APS maintains a variety of scanning, imaging, and digitization equipment. Their specifications are listed below:

Equipment name | Type of equipment | Max scan area (H x W) | Best for 
--- | :---: | --- | :---:
Epson Expression 12000XL | Flatbed scanner | 12.25” x 17” | Photographic prints, photographic transparencies, graphic materials, unbound textual materials (manuscript or printed) 
Epson GT-15000 | Flatbed scanner | 11.5” x 16.5” | Photographic prints, graphic materials, unbound textual materials (manuscript or printed)
CopiBook OS XD | Overhead scanner | 20” x 28” | Maps, oversize graphic materials, bound volumes (manuscript or printed)  

*  Bound material should be scanned on a CopiBook Book Scanner. Detailed instructions on the CopiBook OS XD can be found here (LINK) and instructions on the CopiBook Cobalt can be found here (LINK).
*  Unbound textual material should be scanned on an Epson Flatbed Scanner. Detailed instructions on the Epson Expression 12000 XL can be found here (LINK) and on the Epson FT-15000 can be found here (LINK).
*  Maps and similarly oversized materials should be scanned on a CopiBook Book Scanner. Detailed instructions on the CopiBook OS XD can be found here (LINK).
*  Extra oversized material will need to be consulted with your project supervisor.

All digitized material should be scanned according to specifications based upon their item type. Follow the below standards for archival-quality scans:

Item Type | Resolution (dpi) | Color Space | Bit Depth | File Format | Notes
--- | :---: | :---: | :---: | :---: | :---:
Manuscripts & (Rare) typed/printed | 400-600 | Color | 24-bit | Raw TIFF |
(Non-rare) Typed/printed | 300-400 | Color | 24-bit | Raw TIFF | Higher resolution if item is poor in quality or legibility

## **File Storage**
Before scanning begins, it is important to create a folder to save the image files. All scanned images should be saved to the APS servers. Files will live here temporarily until they are ready for long-term, public-facing storage in the APS Digital Library. 

File organization and naming is a vital component of maintaining a clear connection between a physical object and its corresponding digital surrogate. A good guideline to follow is to imagine being someone else, or you in a year, looking at your scans - is it obvious what they are? Are they unambiguously one specific folder or item in the finding aid?

The files should be arranged by collection (prefixed with the collection call number or accession number).
* The folder name must be the same root as the file name
  *  Folder name = Mss_Coll_190_001 ;
  *  Filenames within folder = Mss_Coll_190_001-001.tif, Mss_Coll_190_001-002.tif, Mss_Coll_190_001-003.tif, etc.

For specific information on file naming conventions, see American Philosophical Society Digital Library Metadata Guidelines. For special cases, consult your project supervisor.

**Back ups**
Digital preservation is a central aspect of the APS, and is provided by continual backups, server maintenance and file-level services. The APS hosts all data on three onsite servers and a host of virtual machines. All data is backed up remotely in consistent rotations, and all daily data modification is mirrored to an offsite data center in West Chester, Pennsylvania. For added security, the APS also enabled the Datto Endpoint Server and Disaster Recovery Solution.

## **Metadata Entry and Formatting**
Uploads into the APS Digital Library will be carried out using Islandora Workbench, a command-line tool that allows creation, updating, and deletion of Islandora content from CSV data. This tool allows the simultaneous upload of items within multiple collections into the Islandora repository, complete with metadata. In order for Workbench to properly associate metadata with its parent and children, metadata entries must be formatted in a certain way. 

There are two spreadsheets that will be used for ingest. Depending on what type of format(s) you are ingesting, you will use either the Book Objects or Other Content Types spreadsheets and instructions. Both Workbench spreadsheets are set up for simple entry of metadata for multiple items. Required fields are rendered light red. Please see the APS Digital Library Metadata Guidelines for detailed information about each field in the spreadsheet.

_For special digitization projects:_
There will be a Workbench sheet within each _Collection Metadata Management_ spreadsheet. In addition to the formatted Workbench sheet, the Collection Metadata Management spreadsheet also contains an _Inventory_ sheet where you will keep track of various stages of the digitization process, including scanning, metadata creation, and quality control. The Inventory sheet is meant to be used for tracking workflow, as well as a “working document” for creation of collection metadata during scanning and/or quality control.  Digitization Technicians should enter “rough” metadata into the Inventory sheet and enter complete, correctly formatted metadata to the Workbench sheet.

