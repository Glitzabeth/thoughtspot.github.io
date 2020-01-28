---
title: [How to view a data schema]
keywords: schema viewer, relationships, keys, worksheet
last_updated: 12/13/2018
tags: [Modeling]
toc: true
summary: "Use the schema viewer to see tables and worksheets and their relationships. "
sidebar: mydoc_sidebar
permalink: /:collection/:path.html
---
ThoughtSpot offers a schema viewer that lets you see your database schema in the
web browser. The Schema Viewer is interactive, so you can configure it to show
just what you want to see.

You need **Admin** privileges to use the **Schema Viewer**.

## Bringing up the Schema Viewer

You can bring up the Schema Viewer from the **Data** screen. Click the ellipses icon
(3 dots) ![R info icon]({{ site.baseurl }}/images/r-icon-more-options.png){: .inline},
and select **View Schema**.

 ![]({{ site.baseurl }}/images/access_schema_viewer.png "Access the Schema Viewer")

When viewing the schema, you can filter the tables shown similarly to how you
filter data sources. The list of tables, worksheets, and imported data on the
left includes only those objects you want to see. Clicking on one of the objects
brings it to the middle of the viewer and highlights it. You can drag the
objects around in the viewer.

 ![]({{ site.baseurl }}/images/schema_viewer.png "Schema Viewer filters")

## Why to use the Schema Viewer

You can use the Schema Viewer to find out information like:

-   What is the relationship between two tables?
-   What tables make up this worksheet, and how are they joined?

The schema viewer shows joins between tables, join directionality, and join type
(whether they are Foreign Key to Primary Key, relationship joins, or joins
defined by users through the web interface). Use the **Table** list to find a
specific table or worksheet.

## Worksheet view

For worksheets, you can also click on one to view the worksheet. The worksheet
view shows the following information:

-   All tables in the worksheet, and the relationships between these tables.
-   Source columns for all columns of a worksheet.

-   Keys and definitions for each relationship, as well as join paths and types.

-   Columns that are derived from formulas.

-   Correct join paths for newly created chasm trap worksheets. Existing chasm trap worksheets will not show the correct join paths.


 ![]({{ site.baseurl }}/images/worksheet_viewer.png "Worksheet view example")

The worksheet view does not work for aggregated worksheets, but does works for
worksheets built on top of aggregated worksheets.
