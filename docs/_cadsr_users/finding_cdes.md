---
layout: cadsr
title: Finding CDEs
author: Jennifer Vendetti
order: 20
---

Common Data Elements (CDEs) are imported into the {{ page.cedarw }} on a 
nightly basis.

This page describes the four main ways to browse and search for CDEs:

- [Browse CDEs via the CATEGORIES pane](#browse-by-category)
- [Browse CDEs via the Community Folder](#browse-by-community)
- [Search for CDEs from the Desktop](#search-from-desktop)
- [Search for CDEs from within templates and elements](#search-from-artifact)
{: .unstyled-list}

***

### Browse CDEs via the CATEGORIES pane
{: #browse-by-category}

The "All Program Areas" tab in the {{ page.cdeb }} displays a list of caDSR 
contexts on the left-hand side of the window. These contexts have been 
imported into the {{ page.cedarw }} and presented as a tree structure in the 
CATEGORIES pane, located on the left-hand side of the window.

In the {{ page.cedarw }}, contexts and classifications are simply referred to 
as "categories". 

To browse CDEs by category, open the root node of the tree structure in the 
CATEGORIES pane entitled "NCI caDSR":

![CATEGORIES pane](../../assets/imgs/cadsr/categories.png)<br />

Select a top-level category, e.g., "ABTC" to see all the CDEs in the category:

![CATEGORIES pane with ABTC selected](../../assets/imgs/cadsr/category-abtc.png)<br />

Continue navigating deeper in the tree to further refine the list of CDEs 
displayed in the center pane:

![CATEGORIES pane with a leaf node in the tree selected](../../assets/imgs/cadsr/category-leaf-node.png)<br />

To see more information about any of the CDEs listed in the center pane, 
select the CDE, click the "Details" button (lowercase 'i'), and look to the 
righ-hand side of the window where the {{ page.cedarw }} displays a details 
pane. The details pane has several tabs that show a wide variety of attributes 
including location, permissions, version, etc.:

![CDE details pane](../../assets/imgs/cadsr/cde-details-pane.png)<br />


### Browse CDEs via the Community Folder
{: #browse-by-community}

The authors of the {{ page.cedarw }} maintain a "Community Folder" that 
contains CEDAR artifacts they feel may be of interest to the entire user 
community. 

To browse CDEs from the Community Folder, click the Community Folder link in 
the upper left portion of the window. In the center pane double-click the 
folder entitled "CDE":

![CDE Community Folder](../../assets/imgs/cadsr/cde-folder.png)<br />

All of the CDEs imported into CEDAR are shown in the center. The buttons at 
the top right-hand side of the window are useful for tweaking how the CDEs 
are displayed, e.g.:

- Use the View button to toggle between grid and list views
- Select any CDE and use the Details button to show and hide the details pane
- Use the Sort button to sort CDEs by creation date, modification date, or title
<br /><br />

![CDEs grid view sorted by title](../../assets/imgs/cadsr/sorted-cdes.png)<br />


### Search for CDEs from the Desktop
{: #search-from-desktop}

The {{ page.cedarw }} displays a search box at the top of what is referred to 
as the "Desktop". One way to make sure the Desktop view is displayed is to 
click on the Workspace link in the upper-left portion of the window. For a 
more in-depth explanation of the Desktop and other components displayed in 
the Workspace, refer to the section entitled 
"[Your CEDAR Workspace](../../sections/a4/your_cedar_workspace)" in the 
"[Desktop and Navigation](../../basic_topics/a4_desktop_and_navigation)" chapter.

When CDEs are imported into the {{ page.cedarw }}, they are named by 
concatenating the Long Name of the CDE with it's Public ID in parentheses. For 
example, the CDE with a Public ID of 62 is imported as "Patient Gender 
Category (62)". To follow are several examples of what to enter in the search 
box to efficiently locate CDEs:

Perform a string search by entering the Long Name of the CDE, surrounded by 
double quotes:

![String search for a CDE by Long Name](../../assets/imgs/cadsr/search-by-long-name.png)<br />

Searching for a shorter Public ID like 62 will sometimes returns too many 
results. Instead, enter the Public ID in parentheses surrounded by double 
quotes:

![String search for a CDE by Public ID](../../assets/imgs/cadsr/search-by-public-id.png)<br />

For longer Public IDs, simply entering the ID in the search box is sufficient:

![Search for a CDE by Public ID](../../assets/imgs/cadsr/search-by-id-only.png)<br />

Perform a search by CDE Version number to see a list of CDEs with a 
particular version:

![Search for CDEs by version](../../assets/imgs/cadsr/search-by-version.png)<br />

Perform a string search by entering the CDE Definition (known as "Description" 
in the {{ page.cedarw }}) surrounded by double quotes:

![Search for CDEs by definition (aka description)](../../assets/imgs/cadsr/search-by-defintion.png)<br />

The {{ page.cedarw }} offers several more sophisticated methods of search 
including the use of wildcards, boolean expressions, and the ability to search 
by field names and values. More information is available in the 
"[Finding Resources](../../basic_topics/a2_finding_resources)" chapter.


### Search for CDEs from within templates and elements
{: #search-from-artifact}

This section assumes basic knowledge of creating and/or editing templates and 
elements in the {{ page.cedarw }}.

To search for a CDE from within a template:

1. Create a new template, or open an existing template.
2. In the resulting template designer interface, click the Search button 
   (magnifying glass icon) in the vertical finder toolbar:
   ![Vertical finder toolbar](../../assets/imgs/cadsr/vertical-finder.png)
3. Use the search box in the resulting dialog to search for the desired CDE.

To search for a CDE from within an element:

1. Create a new element, or open an existing element.
2. In the resulting element designer interface, click the Search button 
   (magnifying glass icon) in the vertical finder toolbar.
3. Use the search box in the resulting dialog to search for the desired CDE.
