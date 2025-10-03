---
layout: page
title: CopiBook OS XD Book Scanner Guide
permalink: /copibook/
last_modified_date: October 2 2025
---

# {{ page.title }}

This document serves as a guide for digitization practices supporting the American Philosophical Society’s digital initiatives. These efforts are part of a broader commitment to preserving and providing access to the Society’s collections through the use of Islandora and Drupal platforms. Specifically, this guide is intended to assist project staff in the use of the CopiBook OS XD Book Scanner to produce high-quality digital surrogates of original materials.

This document will be updated as needed to reflect changes in software, hardware, or digitization standards.

## Step 1: 
Open Limb Capture program from desktop. 

![limp capture scanner desktop shortcut]({{ site.baseurl }}/assets/limp-capture-shortcut.png)  

## Step 2:  
From the Initial Book Scanner Menu select from, *Digitize a new book*, *Resume an existing book scan*, or *Resume last book scan*.
 * Most often you will choose "Digitize a new book"

![limp capture inital scanner menu]({{ site.baseurl }}/assets/copibook_1.png)  

## Step 3:  
If *Digitize a new book* is selected, adjusting new book settings will be necessary:  

**Book configuration** – make sure "from a template" is chosen
 * *Single* – 1 scanning frame (use for bound material to capture full scope of object)
 * *Double* – 2 scanning frames
 * Note: Number of frames dependent on material

**Scan Configuration**  
 * *Scan Format* – **Max should be selected**
 * *Resolution* – DPI is dependent on material. See documentation on [scanning specifications](https://americanphilosophicalsociety.github.io/APS_digitization/digitization/#scanning-equipment-and-specifications)
 * *Scan Mode* - True Color  
 * *Scan Rotation* – Based on layout of material
 * *Calibration Profile* – Last Settings should be selected

**Book Properties**
 * *Name* - Collection or Call number 
 * Saved Image Path - Select folder created in P:drive or external hard drive

**Select Create**

![limp capture new book menu]({{ site.baseurl }}/assets/copibook_2.png) 

## Step 4:  
Place collection material on the scanner bed.
 * By default, the screen will display the real time preview or scanned image (just after scan).
 * If marquee is dotted, then:
    * Right click mouse inside marquee and click ‘auto save’
    * Marquee should turn to a solid line

## Step 5:  
Adjust properties of the frames.
 * Right click inside the marquee and select properties. The frame properties screen will appear.

**Frame name** - Leave as *Main_frame*

**Image number** - 1 (this indicates you would like to start at 1)  
 
**Name pattern**
 * Add root file name in first box (follow [APS file format standards](https://americanphilosophicalsociety.github.io/APS_digitization/digitization/#file-storage))
 * Delete all text in third box
 * You should see a preview of the file name in *Name preview* field

**Number of digits** - 3  

**Increment** - 1 (this indicates you would like files to be sequential)

**File formats** - tif (for preservation quality)

![limp capture full screen]({{ site.baseurl }}/assets/copibook_3.png)
![limp capture right click menu]({{ site.baseurl }}/assets/copibook_4.png)
![limp capture properties menu]({{ site.baseurl }}/assets/copibook_5.png)

## Step 6:  
Adjust the marquee to properly capture the image.  
 * The selected area should perfectly outline the object on the scanner bed leaving a very small, roughly 1 cm. border. Adjust material placement on the scanner bed if necessary and draw the marquee again.
 * The scanner controls of raising and lowering the platform will need to be adjusted and the glass plate lowered depending on the material.

![copibook scanner controls]({{ site.baseurl }}/assets/scanner-controls.png)  

## Step 7:  
Once frames are ready and properly adjusted, scanning can begin!  
 * Press either of the scan buttons on the scanner controls or click the Scan button on the right bottom side of the window.  
   When the Scan button is selected, a progress bar will appear. The bar will initially display red, then change to yellow, at which point you may turn the page. Once it turns green, the system is ready to begin the next scan.  
   **Important**: Starting a scan while the progress bar is still red or yellow may cause the program to crash.  
   The duration of each stage (red, yellow, green) may vary depending on the file size, file type, and the dimensions of the scanned material.  

   
 * Always scan both sides of a rare manuscript item/page dated prior to 1850, even if blank. See other image capture scenarios [here](https://americanphilosophicalsociety.github.io/APS_digitization/digitization/#image-capture).  
 * After each scan a thumbnail of the completed scan will be available on the left side of the screen. These previews should be periodically checked for quality control.  
 * Double clicking on the thumbnail image at the left will open up a larger preview of the image in a viewer.  
 * If you need to delete a page, you can delete its thumbnail image (it will remove the file from the server or hardrive as well). However, make sure to update the *Image number* value in the properties menu to keep the file sequence in order. Other you will need to use Bulk Rename Utility software to rename files after scanning is complete.  

![copibook thumbnail and preview]({{ site.baseurl }}/assets/copibook_6.png)  


## Step 8:
After all material has been scanned:
 * Remove material from scanner bed
 * Lower scanner bed and glass
 * Proceed to [Post-Processing](https://americanphilosophicalsociety.github.io/APS_digitization/digitization/#post-processing) and [Quality Control](https://americanphilosophicalsociety.github.io/APS_digitization/digitization/#quality-control-measures) workflows.
