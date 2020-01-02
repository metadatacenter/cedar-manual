---
layout: section
title: Field Type Reference
author: John Graybeal
status: Pending
chapter: c2
chapter_url: /cedar_templates/c2_building_basic_templates/
chapter_title: Building Basic Templates
---


## **Field Type Reference**

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
| Rich Text | Support entry of rich text in HTML  | Provide a descriptive lead-in to the following field for metadata creators |
| Image | Specify location of an image to display | Provide a static visual lead-in to the following field for metadata creators |
| YouTube | Specify location of a YouTube video to display | Provide a video lead-in to the following field for metadata creators |  


### Common Customizations

Thes customizations are supported for most fields.

#### Required

#### Multiple

#### Value Type

### Customizations for Basic Text Field

#### Values

#### Suggestions


### Customizations for Numeric Fields



