---
layout: cadsr
title: CEDAR for caDSR Users
author: Jennifer Vendetti
permalink: cedar-for-cadsr
---

<!-- <h1 class="page-title">{{ page.title }}</h1><br /> -->

The target audience for this section is end users of the [{{ page.fb }}](https://formbuilder.nci.nih.gov/FormBuilder/){:target="_blank"} application.

The intent of this section is to help end users of the {{ page.fb }} learn how to accomplish the same type of tasks, e.g., building forms with questions/CDEs, in the {{ page.cedarw }}.

The {{ page.fb }} and {{ page.cedarw }} use different naming conventions to describe the various components in their systems. The following table offers a translation: 

<table class="naming-translations">
  <thead>
    <tr>
      <th class="naming-translations">{{ page.fb }}</th>
      <th class="naming-translations">{{ page.cedarw }}</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>common data element (CDE)</td>
      <td>field</td>
    </tr>
    <tr>
      <td>data element</td>
      <td>field</td>
    </tr>
    <tr>
      <td>question</td>
      <td>field</td>
    </tr>
    <tr>
      <td>classification</td>
      <td>category</td>
    </tr>
    <tr>
      <td>classification scheme</td>
      <td>category</td>
    </tr>
    <tr>
      <td>classification scheme item</td>
      <td>category</td>
    </tr>
    <tr>
      <td>context</td>
      <td>category</td>
    </tr>
    <tr>
      <td>form</td>
      <td>template</td>
    </tr>
    <tr>
      <td>module</td>
      <td>element</td>
    </tr>
    <tr>
      <td>permissible values</td>
      <td>values</td>
    </tr>
  </tbody>
</table><br />

To get started with any of the following topics, navigate to the [{{ page.cedarw }}](http://cedar.metadatacenter.org/){:target="_blank"} and log in to your account. If you need instructions for creating an account, please refer to the "[Accounts and Logging In](basic_topics/a1_accounts_and_logging_in "Accounts and Logging In")" section of the user guide.

<ul class="unstyled-list">
  {% assign sorted_pages = site.cadsr_users | sort: "order" %}
  {% for node in sorted_pages %}
    <li><a href="{{ site.baseurl }}{{ node.url }}">{{ node.title }}</a></li>
  {% endfor %}
</ul>

<!-- <br />Please {% github_edit_link "help improve this article" %}. -->

