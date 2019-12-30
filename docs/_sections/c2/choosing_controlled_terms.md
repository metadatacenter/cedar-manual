---
layout: section
title: Field Type Reference
author: John Graybeal
status: In Progress
chapter: c2
chapter_url: /cedar_templates/c2_building_basic_templates/
chapter_title: Building Basic Templates
---




## **About CEDAR Field Types**

While specifying a field in a templating resource (a Template, Element, or Field), 
you can customize the Field resource in a number of ways,
including constraining the values that metadata editors can input 
when they enter their metadata for the field. 
Some customizations apply to almost every field type; 
others are only allowed for one or two field types.

### Choosing the Field Type

The following tables show the field types that CEDAR offers, 
and the customizations or purpose supported by that field type.

Many supported customizations are available to a broad class of fields. 

| Generic Field Type | Description | Supported Customizations |
| --------- | ----- | -------------- |
| Most Data Fields |  | Required; Multiple; Hidden |
| Basic Text |  |  Min/Max Length, Suggestions  |


Individual field types offered by CEDAR are described here.

| Unique Field Type | Data Type(s) | Unique Supported Customizations |
| --------- | ----- | -------------- |
| Short Text |   | Values  |
| Paragraph Text |   |   |
| Numeric   |  integer, long integer, single precision real, double precision real |  Unit of Measure, Minimum Value, Maximum Value, Decimal Places  |
| Email |   |   |
| Link |   |   |
| Multi-Choice |   |   |
| Checkbox |   |   |
| Pick From List |   |   |
| Phone |   |   |

These special field types do not support data storage for the metadata creator,
but allow the template author to customize presentation of the template
to the metadata creator.

| Special Field Type | Description | Purpose |
| --------- | --------- | ------- |
| Section | Creates a section break | Provides a textual separator with optional explanatory text  |
| Page | Creates a page break | Breaks up form into multiple pages when entering metadata |
| Rich Text |   |   |
| Image |   |   |
| YouTube |   |   |


### Common Customizations

Thes customizations are supported for most fields.

#### Required

#### Multiple

#### Value Type

### Customizations for Basic Text Field

#### Values

#### Suggestions


### Customizations for Numeric Fields



## **Creating a Stand-Alone Field**

This process begins by creating the Field artifact, 
almost exactly like creating the Template Artifact in <a href="">First Steps</a>. 
After that, the content of the field is created exactly as is performed 
in the Creating Field Content subsection above.

To create a new stand-alone Field, 
click the "New" button on the Desktop's navigation sidebar
(upper left of the Workspace view) and
select the "Field" option in the dropdown menu. 
This step opens up the Field creation form as shown below. 

Enter the human-readable label, identifier and description of the Field  
using the three text input fields ('Untitled', 'Identifier', 'Description') 
underlined in the image below. 

## **Importing a Stand-Alone Field**


