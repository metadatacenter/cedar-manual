# CEDAR Manual

A documentation regarding the manual/documentation on how to use CEDAR to create and use metadata templates. That is, a **Meta-documentation about Metadata**.

### Directory Structure
The different files in the CEDAR manual are arranged in the following structure:


##### Chapter folders
These folders contain only Github pages for each chapter. The page has content related to the chapter heading, and then different sections are listed (generated using the Chapter layout template in the _layouts folder). For example, _basic_topics/a1_accounts_and_logging_in.md is the first chapter under "CEDAR Basics for All Users" and the pages for the corresponding sections are present in the _sections/a1/ folder.
- *_advanced_guidance*: Chapters pertaining to the topic "Advanced Guidance"
- *_advanced_topics*: Chapters pertaining to the topic "Advanced Topics for All Users"
- *_basic_topics*: Chapters pertaining to the topic "CEDAR Basics for All Users"
- *_cedar_templates*: Chapters pertaining to the topic "About CEDAR Templates"


##### Content folders
- *_sections*: Each section page for the manual is present as distinct .md file under this _folder. These section pages are organized according to their chapter (e.g. accounts_and_loggin_in chapter has 3 main sections that are present under a1 folder.)
- *pages*: Manual pages that are not specific chapters in this manual, but provide more broad overview that may be referenced from within each section. For example, Glossary.html provides a glossary of all terms specific to CEDAR.


##### Required folders
- *_includes*: HTML elements that remain common across all pages (chapter or section pages). For example, sidebar, header, footer HTML is rendered from this folder.
- *_layouts*: HTML templates that are used to render different pages of the manual (e.g., chapter pages https://metadatacenter.github.io/cedar-manual/basic_topics/a1_accounts_and_logging_in/ is generated from the HTML template chapter.html). Hence, the HTML format remains consistent across different chapters and pages.
- *_sass*: Base CSS for the CEDAR manual (i.e. the Github pages Ed theme) - can be ignored by documentation writers.
- *assets*: Additional CSS, JS, and Images folder. The key folder here is the Images folder (imgs/) which can be used to store CEDAR screenshots used in the manual.


##### Other files
- *index.html*: Main file that is rendered when the user launches metadatacenter.github.io/cedar-manual ... The table of contents is generated from this page and different topics can be created easily (follow previous examples)
- *print.html*: When the user clicks "Print the CEDAR user guide", this is the actual file that is printed. It contains the template to incorporate content from different chapters and sections.
- *_config.yml*: Configuration file to decide to theme color, chapter folders etc. (This will be the file if you wish to create a new "topic" for display, the links of which will need to be edited under index.html)
- *search.html*: Searching is not currently incorporated within the website, but this file can be modified later on.


---------------------------------------------------------------------------
### Section Page

Each section page has the following key-value pairs at the beginning of the page:
---
layout: section
title: Creating a CEDAR Account
author: John Graybeal
status: Ready
chapter: a1
chapter_url: /basic_topics/a1_accounts_and_logging_in/
chapter_title: Accounts and Logging In
---

The layout key indicates the HTML template (stored under _layouts) to be used for rendering it on the Web. The title, author and status (i.e., whether section is ready for release) keys can be rendered separately within the page (again using the _layouts/section.html). The chapter key helps organization of different sections during the rendering of the chapter page, and the chapter_url and chapter_title allows providing "return links" in each section (i.e. return back from section to chapter page). 
@TODO Include chapter_url/chapter_title key-value pairs for each section page.

### Chapter Page

Each chapter page has the following key-value pairs at the beginning of the page:
---
layout: chapter
title: Accounts and Logging In
author: John Graybeal
chapter: a1
status: Ready
---

The explanations for these key-value pairs follow the original explanations, given above for the Section page.





