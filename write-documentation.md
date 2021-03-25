---
title: Writing Documentation
layout: default
nav_order: 3
---
# Writing Documentation
This workshop focuses on writing documentation for libraries and other cultural institutions.  
## What are you writing?
The documents you write today will contain markdown and be published to Github Pages.
## What is the purpose of your documentation?
The purpose of your documentation will influence the technical style you use.
### Provide instructions
Step-by-step instructions can include bulleted or numbered lists and are more likely to use short phrases or sentences than paragraphs. Introductory paragraphs can be helpful but instructional text should be short and clear.
### Map a workflow
Flowcharts and bulleted lists are useful when representing workflow.
### Describe department operations
This type of documentation can use a more traditional paragraph format. Lists of services can also be useful for some audiences.
## Who is the audience for your documentation?
The kind of content you include will depend on the audience. Determining your audience might also indicate whether your documentation will be offline, internal, or publicly available.
### Department staff
Documentation for staff within a department can include acronyms (Acronyms should always be spelled out before they are abbreviated.) and shared professional terminology. All the same, write documents that can be understood equally by new staff. Offline documentation can sometimes include privacy and security information like IP ranges or login instructions. Consider the culture of your department.
### Institution staff
The content of documentation for an institution will fall somewhere between department specific and public documentation depending on the institution.
### Public
Writing documentation for a public audience may require additional considerations like localization.
## Style
### Microsoft Style Guide
* [Microsoft Style Guide](https://docs.microsoft.com/en-us/style-guide/welcome/){:target="_blank"}
* A good introduction to style for documentation
* I recommend reading it through once then returning to sections as you think of questions related to your documentation.
* Write content first. Add images later.  
<!-- Add examples -->
### Organizing Information
* Group related information.  
<div class="code-example" markdown="1">
<!-- <details open markdown="block"> -->
## File Transfers  
    The most common method of transfer uses a Bagit script via command line.  

## Disk Imaging  
    Disk images are created when they facilitate viewing and accessing born-digital material.  
    Some legacy file formats cannot be viewed in recent operating systems. Imaging this material  
    allows it to be viewed in an emulator.  

## Vendor Transfers
    When the lab does not have the proper drive to access a type of media the media may be sent to  
    a vendor for transfer.  

## Network Transfers  
    In some cases born-digital material may be transferred over a network. Accessioning procedures  
    for these types of transfers are still in progress.  

<!-- </details> -->
</div>
* Keep the number of grouped documents manageable.
* Use 1 or 2 levels of facets.
    * See [Clarity](###Clarity) section.
* Link related documents.
* Balance linking to other documents with repeating information within documents.
### Clarity
* Text should be skimmable.
    * Users should be able to follow your documentation without closely reading every word.
    * No negative or double negative gotchas.
* Parallelism
    * Sentences should be formatted uniformly.
    * Words should appear in the same order in sentences within a section.  
    * You may think repetition will lull users into skipping instructions but it’s easier for users that are reading along as they perform the instructions.
<div class="code-example" markdown="1">       
**Good Example**
## Complete the transfer.
* Turn off the Tableau and the device.
* Disconnect power and data cables from the device.
* Return the device to its record carton.
* Return the power and data cables to the equipment rack.

**Not Parallel**
## Completing the transfer.
* The Tableau and the device should be turned off.
* Disconnect power and data cables from the device.
* The device can then be put into its record carton.
* The equipment rack holds power and data cables when you are done with them.
</div>
    
* Short sentences
    * Keep sentences short and actionable.
    * It’s tempting to provide as much information as possible. Make sure sentences are short enough to be skimmed.
    * Use note boxes when more description or explanation is needed.  
    
|When commercial software is present do not enter it in CMS or label it. Send commercial software as is to Digital Preservation.|   

### Types of documents	
* Instructions
    * Use bullet pointed lists.
    * Use 1 level of indentation in most instances.
    * Lists can be numbered but don’t use elaborate combinations of numbers and letters.
<div class="code-example" markdown="1">
**Not Great List**
5. Wait at least one minute for the Activity light to turn on. If it does not, turn the Tableau off and on again.  
    a. Zip disk drives almost always need to be turned off and on before they will connect. This may also be necessary between Zip disks.  
6. Check for a Windows prompt or a listing in Windows Explorer indicating the device has been connected.    
    a. When imaging legacy media the device might only appear in the FTK Imager drive list.  
    b. If the device does not appear, contact Digital Archives staff.  
</div>
* Map a workflow.
    * Use bullet pointed lists.
    * Create Flowcharts.
* Describe your department.
    * Write short paragraphs.
<div class="code-example" markdown="1">
This website holds the documentation for the New Amsterdam Research Libary (NARL) Digital Archives. It is intended for the use by NARL staff. Documents are also available publicly for feedback, outreach, and education purposes.
</div> 

### Audience  
* Consider the detail of documentation.
* Consider the use of sensitive information (passwords).
* Consider the use of institutional and professional acronyms.
* Consider how to display contact information.

## TL;DR
* First things first.
* No negative or double negative gotchas.
* Parallel Structures 
    * You may think repetition will lull users into skipping instructions but it’s easier for users that are reading along as they perform the instructions.
* It’s tempting to provide as much information as possible. Make sure sentences are short enough to be skimmed.
* Lists can be numbered but don’t use fractions or combine letter and number hierarchies.
