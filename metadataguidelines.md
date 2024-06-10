---
layout: page
title: APS Digital Library Metadata Guidelines
permalink: /metadata/
last_modified_date: June 10 2024
---

# {{ page.title }}

This document is intended as a guide to data entry and descriptive cataloging for the American Philosophical Soceity Digital Libary using Islandora and Drupal software. It is designed to help the creator of the record metadata decide what information is required, which field is the best choice for the information, and the format in which the information should be entered.  It will be updated as modifications in the software and/or metadata schema necessitate.

<details open markdown="block">
  <summary>
 Table of Contents
    </summary>
- TOC
{:toc}
</details>

## **Each field includes the following information**
**Field name:** Display label for the name of the field in Islandora.  
**Definition:** A combination of MODS definitions, Islandora Workbench definitions, and APS modifications as appropriate.  
**Obligation:** A statement about whether the field is required, required if applicable, recommended, or optional; and information about whether or not you can have more than one value in the field (i.e. repeatable or not repeatable).  
**Enter Data in Spreadsheet Column:** The corresponding column heading in the Workbench spreadsheet to enter the data. The column name indicates to Workbench which field to add value and must be exactly as the drupal machine name is spelled/formatted.  
**Type of field:** The type of data that can be entered into a particular field.  
**Application:** Specification on formatting and tips for entering data into a particular field.  
**Example(s):** Sample data that would be acceptable in this field.  

## **General Information and Guidelines**
* The terms “item,” “resource,” and “object” have been used interchangeably throughout these guidelines. An “item,” “resource,” or “object” can be a number of different things including a an individual document, a folder of documents, a photograph, a photo album (filled with many photographs), a journal, a diary, an account book, a published book, a recorded oral history, a scrapbook, a map, an atlas, a postcard, a video or audio recording etc.
* Be consistent in your use of the metadata fields.
* One row in the Workbench spreadsheet equates to one Drupal node. A node is created to hold descriptive metadata about content in the repository.
* If you have no data for a metadata field, **leave it blank**; do not enter “N/A” or “None” or question mark.
* Ending punctuation is not required for field content and is only recommended in fields where complete sentences are used (e.g. abstract, notes).
* Do not use ampersands (“&”) to connect sentence elements. An ampersand should only be used when it is part of an official corporate name or logo.
* Where multiple values are appropriate in a repeatable field (names, subjects, languages, etc.), you **must** separate them with a pipe "\|" and no spaces in between values when entering into the workbench spreadsheet.
* Avoid the use of abbreviations. Writing words out enables users to find items consistently and also helps to avoid confusion (such as abbreviating both County and Company to “Co.”). An exception to this rule is the use of “St.” in a city or place name (e.g. St. Peter, St. Paul or St. Benedict).
* **Spell-check your metadata.** After entering your information into the MIK spreadsheet, run the spell check to catch any misspelled words. Also, verify the spelling of local place names and individual’s names that may not be caught during the spell-check process.


## **Required Metadata**

### **File**
**Definition:** The location of files that are used to create Drupal Media.  
**Obligation:** Required; not repeatable  
**Enter Data in Spreadsheet Column:** file  
**Type of field:** Text  
**Application:**  
* If you are uploading multiple **Book objects** (objects with multiple pages), the file column should be formatted:
  *  Enter the folder name that contains the media
  *  The folder name must be the same root as the file name
  
      Folder name = Mss_Coll_190_001  (this is entered in the _file_ field only)  
      Filenames within folder = Mss_Coll_190_001-001.tif, Mss_Coll_190_001-002.tif, etc.

* If you are uploading multiple **Single Graphics, Audio, or Video objects**, the file column should be formatted:
  *  Enter the appropriate **directory path** and individual filename with file extension.

For file names in general:
* Only use alphanumeric characters without diacritics, and underscores and hyphens, i.e. [a-z] [A-Z] [0-9] [_] [-]
* Periods should only be used for the file extension.
* File names generally follow this pattern:

Prefix (root) | Separator | Number | Period | Extension 
--- | --- | --- | --- | --- |
Mss_Ms_Coll_190 | - | 001 | . | tif 

  *  The **prefix** identifies the file as part of a collection, and should contain the collection call number, item identifier, or any other useful information. It should not be long, and is not intended to include all necessary metadata. It cannot contain hyphens, but can contain underscores.
  *  The **separator** (a hyphen) separates the prefix from the file number.
  *  The **number** is used to distinguish sequential files, e.g. pages in a folder or book, or photographs in an album. It should be padded to at least three digits, resulting in e.g. [001, 002,..., 099, 100] instead of [1, 2,..., 99, 100], which may alphabetize differently on different systems.
  *  The **period** separates the main file name from the extension, and should only be used once.
  *  The **extension** identifies the type of file, and is typically added automatically.

The Bulk Rename Utility application can be used to apply bulk changes to both folder and file names. 

**Examples:**
* Book object:
  *  Mss_B_F_327_001
  *  Coll_190_001
  *  Am_23
* Other content types (Graphic, Audio, Video):
  *  /mnt/ingest/data/Mss_497_3_Am4-001.mp4
  *  /mnt/ingest/data/Mss_B_P31_F8_62_5.tif
  *  /mnt/ingest/data/audio9177.wav

***

### **Total Scans**
**Definition:** Number of digital files for a given object or resource.  
**Obligation:** _Required for Book objects only!_; not repeatable  
**Enter Data in Spreadsheet Column:** total_scans  
**Type of field:** Integer  
**Application:**  
* Enter the number of digital files in a folder for each book object to be ingested.
* This number must match the amount of files in your object’s folder in order for workbench to run the ingest and upload the files.

**Example:**

Object folder | total_scans field
--- | ---
7 tif files | 7
158 tif files | 158
40 jpg files | 40

***

### **Resource Type**
**Definition:** A broad term that specifies the characteristics or general physical aspect of the content of the resource.   
**Obligation:** Required; not repeatable  
**Enter Data in Spreadsheet Column:** field_resource_type  
**Type of field:** Entity reference  
**Application:**  
* Enter the term from the controlled list below that best characterizes or describes the item. Only one value may be assigned.
* The first letter of the term must be capitalized.

Term name | External link  
--- | --- 
Collection | http://purl.org/dc/dcmitype/Collection 
Data Set | http://purl.org/dc/dcmitype/Dataset 
Image | http://purl.org/dc/dcmitype/Image 
Interactive Resource | http://purl.org/dc/dcmitype/InteractiveResource 
Moving Image | http://purl.org/dc/dcmitype/MovingImage 
Physical Object | http://purl.org/dc/dcmitype/PhysicalObject 
Service | http://purl.org/dc/dcmitype/Service 
Software | http://purl.org/dc/dcmitype/Software 
Sound | http://purl.org/dc/dcmitype/Sound 
Still Image | http://purl.org/dc/dcmitype/StillImage 
Text | http://purl.org/dc/dcmitype/Text 

Note: The Born-Digital Islandora 2.0 theme requires specific combinations of Resource Type and Model terms in order for compound objects, collections, and paged objects to display correctly. Please refer to Appendix B: Born-Digital Islandora 2.0 Theme Object View Configurations.

**Example:**  

Object Type | Resource Type term | Islandora Model term  
--- | --- | --- 
Collection | Collection | Collection 
Audio | Sound | Audio 
Basic Image (jpeg) | Still Image | Image 
Book (parent of pages) | Still Image | Image 
Large Image (tiff) | Still Image | Image 
Page | Text | Page 
PDF | [any] | Digital Document 
Video | Moving Image | Video 

***

### **Model**
**Definition:** Type of content being represented by a node (e.g. an image, a video, a collection of other items, etc...)  
**Obligation:** Required; not repeatable  
**Enter Data in Spreadsheet Column:** field_model  
**Type of field:** Entity reference  
**Application:**  
* Enter the term from the controlled list below that best characterizes or describes the item. Only one value may be assigned.
* The first letter of the term must be capitalized.

Term Name | External URI  
--- | --- 
Audio | http://purl.org/coar/resource_type/c_18cc 
Binary | http://purl.org/coar/resource_type/c_1843 
Collection | http://purl.org/dc/dcmitype/Collection#Model 
Compound Object | http://vocab.getty.edu/aat/300242735 
Digital Document | https://schema.org/DigitalDocument 
Image | http://purl.org/coar/resource_type/c_c513 
Newspaper | https://schema.org/Newspaper 
Page | http://id.loc.gov/ontologies/bibframe/part 
Paged Content | https://schema.org/Book 
Publication Issue | https://schema.org/PublicationIssue 
Video | http://purl.org/coar/resource_type/c_12ce 

Note: The Born-Digital Islandora 2.0 theme requires specific combinations of Resource Type and Model terms in order for compound objects, collections, and paged objects to display correctly. Please refer to Appendix B: Born-Digital Islandora 2.0 Theme Object View Configurations.

**Example:** 

Object Type | Resource Type term | Islandora Model term  
--- | --- | --- 
Collection | Collection | Collection 
Audio | Sound | Audio 
Basic Image (jpeg) | Still Image | Image 
Book (parent of pages) | Still Image | Image 
Large Image (tiff) | Still Image | Image 
Page | Text | Page 
PDF | [any] | Digital Document 
Video | Moving Image | Video 

***

### **Member of**  
**Definition:** Determines the parent of the object. It is used to identify the collection to which an object belongs, or the parent/container object if the object is a page or compound object.  
**Obligation:** Required (if adding to a pre-existing collection); not repeatable  
**Enter Data in Spreadsheet Column:** field_member_of  
**Type of field:** node reference  
**Application:**  
* For the purposes of Workbench, the Member Of column is used if you have a pre-existing collection in Drupal into which you want to ingest an object. In this case, you will enter the collection’s node ID in the Member Of column in the object row that belongs to the collection.
* If you are adding a new collection to Drupal, you will leave this column blank. However you will not delete the column when ready for ingest.

***