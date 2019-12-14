---
layout: section
title: Working with CDEs
author: John Graybeal
status: In Progress
chapter: c4
chapter_url: /cedar_templates/c4_advanced_template_topics/
chapter_title: Advanced Template Topics
---
CEDAR contains nearly 60,000 Common Data Elements imported from the National Cancer Institute'section caDSR Data Element repository. These are represented as Fields in CEDAR, as each CDE
describes a single question and its possible answers.

Because all of these CDEs are managed by caDSR following the same metadata model, we can offer some tips for working with them efficiently in the CEDAR system.

## **Finding and Browsing CDEs** 

### Searching from the CEDAR Desktop

- by identity number, name, or description
- by version number 

### Browsing All CDEs

If you search on "CDE" from the Desktop, one of the first entries you'll see is the CDE folder.
This is the location of all the imported CDEs from caDSR.

![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/cde-folder-20191212.png){:width="80%" class="centered"}

You will quickly discover that navigating through this list isn't practical, as only a small 
number can be presented at any one time. Instead, use the search bar to narrow down the list, 
as described above.

### Browsing by CDE Categories

![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/category-dropdown-20191212.png){:width="20%" class="right"}
In caDSR, CDEs and forms can be classified using Classifications, more specifically 
Classification Schemes and Classification Scheme Item. The caDSR classifications have been
imported into CEDAR as hierarchical categories under the NCI caDSR category, 
as shown in the image on the right. 

You can find CDEs in a particular category by using the CEDAR categories menu 
in the left-hand navigation panel. Selecting an item at any level of the category
hierarchy will show all the CDEs contained within that level, and all lower levels.

You can view the Category or Categories for any CDE you see in the Desktop by clicking on
the CDE, [bringing up the information metadata tab](https://metadatacenter.github.io/cedar-manual/cedar_templates/basic_topics/a3_viewing_resource_metadatda/), and selecting the Categories tab.
CEDAR lists all the Categories to which the selected CDE belongs.

### When Creating a Template

On bringing up the search pop-up display,
- searching similar to searching from CEDAR Desktop
- navigation using bottom navigation bar

## **Obtaining and Maintaining CDEs**

By importing the XML-defined CDEs from the caDSR system into JSON Schema-defined fields in CEDAR, 
we make these specifications available to any CEDAR user. 
So far we run the conversion process manually, 
but we expect to run conversions as frequently as nightly 
to keep the CEDAR CDEs up-to-date with respect to the source content.

When run, the conversion process updates any caDSR-updated CDEs in the CEDAR system, 
replaces all the CDE Value Sets in BioPortal, and 
ensures that the Categories in CEDAR are updated to the Classifications 
provided in the caDSR export. 

We do not manage the entire CDE specification that contains a comprehensive implementation of the ISO/IEC 11179 standard, but focus instead on core functionality that relates to the precise specification of questions and the values used to answer those questions.







