# Supermarket Sales Analysis Report
This project analyzes supermarket sales data to identify key performance metrics, customer behavior, and product/category performance. The goal was to derive actionable insights that can assist in strategic decision-making.

Tools Used: Power BI, Microsoft Excel
Dataset source: https://www.kaggle.com/datasets/chadwambles/supermarket-sales/data

Process:

Data Preparation:

Cleaned and structured the dataset to ensure accuracy in reporting.
Verified key fields like sales, revenue, and reward points.
Data Analysis and Visualization:

Created a Power BI dashboard to present insights visually.

Key visuals included:
Revenue and Sales Count Analysis by gender, city, and customer type.
Product Category Performance for sales and reward points.
Customer Distribution by city and type using stacked bar charts.

Key Findings:
Chicago generated the highest percentage of revenue among all cities.
Members contribute higher total revenue compared to Normal customers.
The Fruits and Personal Care categories were the top performers in sales count and reward points.
Male customers had slightly higher revenue contributions than female customers.
Results:
The dashboard provided clear insights into customer behavior, city-wise sales performance, and top-performing product categories, enabling data-driven decision-making for marketing and operations strategies.

![image](https://github.com/user-attachments/assets/5f8a13ee-d3f4-48be-ab37-3696cd8904cf)

# ADVANCED Supermarket Sales Analysis Insights

Objective
This project analyzed supermarket sales data to identify key performance metrics, customer behavior, and product/category performance. The goal was to provide actionable insights that assist in strategic decision-making and demonstrate advanced data science techniques, including clustering and predictive modeling.

Project Highlights
Exploratory Data Analysis (EDA)

Visualized trends in revenue across cities, product categories, and customer types using Python libraries like Pandas, Matplotlib, and Seaborn.
Conducted deep dives into revenue drivers and identified high-performing branches, products, and customer segments.
Customer Segmentation (Clustering)

Utilized K-Means Clustering to segment customers into actionable groups such as "High Spenders" and "Bargain Shoppers."
Segmentation based on features like purchase quantity, total spending, and customer type enabled targeted marketing strategies.
Predictive Modeling for Sales (Regression)

Built a Linear Regression model to predict total sales based on features like product category, unit price, and customer behavior.
Achieved an R² score of 85% and demonstrated the ability to forecast sales for better revenue management.
Actionable Business Insights

Identified high-revenue product categories and cities, enabling targeted promotions and inventory optimization.
Proposed customer-focused recommendations to improve revenue and customer retention strategies.
Tools and Technologies Used
Data Analysis: Pandas, NumPy, Matplotlib, Seaborn
Machine Learning: Scikit-learn (Clustering, Regression)
Data Engineering: Data cleaning, transformation, and feature encoding
Visualization: Python plots and interactive charts for trends and segment insights
Results
Successfully segmented customers into actionable groups to tailor marketing strategies.
Forecasted sales trends, enabling data-driven decision-making for product placement and promotions.
Delivered business insights to maximize revenue and optimize operational efficiency.
This project demonstrates expertise in end-to-end data science workflows, from exploratory analysis to machine learning, while showcasing strong business acumen through actionable recommendations.
[Uploading Untitled.html…]()<!DOCTYPE html>

<html lang="en">
<head><meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>Untitled</title><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>
<style type="text/css">
    pre { line-height: 125%; }
td.linenos .normal { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
td.linenos .special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
span.linenos.special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
.highlight .hll { background-color: var(--jp-cell-editor-active-background) }
.highlight { background: var(--jp-cell-editor-background); color: var(--jp-mirror-editor-variable-color) }
.highlight .c { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment */
.highlight .err { color: var(--jp-mirror-editor-error-color) } /* Error */
.highlight .k { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword */
.highlight .o { color: var(--jp-mirror-editor-operator-color); font-weight: bold } /* Operator */
.highlight .p { color: var(--jp-mirror-editor-punctuation-color) } /* Punctuation */
.highlight .ch { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Hashbang */
.highlight .cm { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Multiline */
.highlight .cp { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Preproc */
.highlight .cpf { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.PreprocFile */
.highlight .c1 { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Single */
.highlight .cs { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Special */
.highlight .kc { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Constant */
.highlight .kd { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Declaration */
.highlight .kn { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Namespace */
.highlight .kp { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Pseudo */
.highlight .kr { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Reserved */
.highlight .kt { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Type */
.highlight .m { color: var(--jp-mirror-editor-number-color) } /* Literal.Number */
.highlight .s { color: var(--jp-mirror-editor-string-color) } /* Literal.String */
.highlight .ow { color: var(--jp-mirror-editor-operator-color); font-weight: bold } /* Operator.Word */
.highlight .pm { color: var(--jp-mirror-editor-punctuation-color) } /* Punctuation.Marker */
.highlight .w { color: var(--jp-mirror-editor-variable-color) } /* Text.Whitespace */
.highlight .mb { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Bin */
.highlight .mf { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Float */
.highlight .mh { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Hex */
.highlight .mi { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Integer */
.highlight .mo { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Oct */
.highlight .sa { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Affix */
.highlight .sb { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Backtick */
.highlight .sc { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Char */
.highlight .dl { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Delimiter */
.highlight .sd { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Doc */
.highlight .s2 { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Double */
.highlight .se { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Escape */
.highlight .sh { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Heredoc */
.highlight .si { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Interpol */
.highlight .sx { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Other */
.highlight .sr { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Regex */
.highlight .s1 { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Single */
.highlight .ss { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Symbol */
.highlight .il { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Integer.Long */
  </style>
<style type="text/css">
/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*
 * Mozilla scrollbar styling
 */

/* use standard opaque scrollbars for most nodes */
[data-jp-theme-scrollbars='true'] {
  scrollbar-color: rgb(var(--jp-scrollbar-thumb-color))
    var(--jp-scrollbar-background-color);
}

/* for code nodes, use a transparent style of scrollbar. These selectors
 * will match lower in the tree, and so will override the above */
[data-jp-theme-scrollbars='true'] .CodeMirror-hscrollbar,
[data-jp-theme-scrollbars='true'] .CodeMirror-vscrollbar {
  scrollbar-color: rgba(var(--jp-scrollbar-thumb-color), 0.5) transparent;
}

/* tiny scrollbar */

.jp-scrollbar-tiny {
  scrollbar-color: rgba(var(--jp-scrollbar-thumb-color), 0.5) transparent;
  scrollbar-width: thin;
}

/* tiny scrollbar */

.jp-scrollbar-tiny::-webkit-scrollbar,
.jp-scrollbar-tiny::-webkit-scrollbar-corner {
  background-color: transparent;
  height: 4px;
  width: 4px;
}

.jp-scrollbar-tiny::-webkit-scrollbar-thumb {
  background: rgba(var(--jp-scrollbar-thumb-color), 0.5);
}

.jp-scrollbar-tiny::-webkit-scrollbar-track:horizontal {
  border-left: 0 solid transparent;
  border-right: 0 solid transparent;
}

.jp-scrollbar-tiny::-webkit-scrollbar-track:vertical {
  border-top: 0 solid transparent;
  border-bottom: 0 solid transparent;
}

/*
 * Lumino
 */

.lm-ScrollBar[data-orientation='horizontal'] {
  min-height: 16px;
  max-height: 16px;
  min-width: 45px;
  border-top: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='vertical'] {
  min-width: 16px;
  max-width: 16px;
  min-height: 45px;
  border-left: 1px solid #a0a0a0;
}

.lm-ScrollBar-button {
  background-color: #f0f0f0;
  background-position: center center;
  min-height: 15px;
  max-height: 15px;
  min-width: 15px;
  max-width: 15px;
}

.lm-ScrollBar-button:hover {
  background-color: #dadada;
}

.lm-ScrollBar-button.lm-mod-active {
  background-color: #cdcdcd;
}

.lm-ScrollBar-track {
  background: #f0f0f0;
}

.lm-ScrollBar-thumb {
  background: #cdcdcd;
}

.lm-ScrollBar-thumb:hover {
  background: #bababa;
}

.lm-ScrollBar-thumb.lm-mod-active {
  background: #a0a0a0;
}

.lm-ScrollBar[data-orientation='horizontal'] .lm-ScrollBar-thumb {
  height: 100%;
  min-width: 15px;
  border-left: 1px solid #a0a0a0;
  border-right: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='vertical'] .lm-ScrollBar-thumb {
  width: 100%;
  min-height: 15px;
  border-top: 1px solid #a0a0a0;
  border-bottom: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='horizontal']
  .lm-ScrollBar-button[data-action='decrement'] {
  background-image: var(--jp-icon-caret-left);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='horizontal']
  .lm-ScrollBar-button[data-action='increment'] {
  background-image: var(--jp-icon-caret-right);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='vertical']
  .lm-ScrollBar-button[data-action='decrement'] {
  background-image: var(--jp-icon-caret-up);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='vertical']
  .lm-ScrollBar-button[data-action='increment'] {
  background-image: var(--jp-icon-caret-down);
  background-size: 17px;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-Widget {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
}

.lm-Widget.lm-mod-hidden {
  display: none !important;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.lm-AccordionPanel[data-orientation='horizontal'] > .lm-AccordionPanel-title {
  /* Title is rotated for horizontal accordion panel using CSS */
  display: block;
  transform-origin: top left;
  transform: rotate(-90deg) translate(-100%);
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-CommandPalette {
  display: flex;
  flex-direction: column;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-CommandPalette-search {
  flex: 0 0 auto;
}

.lm-CommandPalette-content {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  min-height: 0;
  overflow: auto;
  list-style-type: none;
}

.lm-CommandPalette-header {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.lm-CommandPalette-item {
  display: flex;
  flex-direction: row;
}

.lm-CommandPalette-itemIcon {
  flex: 0 0 auto;
}

.lm-CommandPalette-itemContent {
  flex: 1 1 auto;
  overflow: hidden;
}

.lm-CommandPalette-itemShortcut {
  flex: 0 0 auto;
}

.lm-CommandPalette-itemLabel {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.lm-close-icon {
  border: 1px solid transparent;
  background-color: transparent;
  position: absolute;
  z-index: 1;
  right: 3%;
  top: 0;
  bottom: 0;
  margin: auto;
  padding: 7px 0;
  display: none;
  vertical-align: middle;
  outline: 0;
  cursor: pointer;
}
.lm-close-icon:after {
  content: 'X';
  display: block;
  width: 15px;
  height: 15px;
  text-align: center;
  color: #000;
  font-weight: normal;
  font-size: 12px;
  cursor: pointer;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-DockPanel {
  z-index: 0;
}

.lm-DockPanel-widget {
  z-index: 0;
}

.lm-DockPanel-tabBar {
  z-index: 1;
}

.lm-DockPanel-handle {
  z-index: 2;
}

.lm-DockPanel-handle.lm-mod-hidden {
  display: none !important;
}

.lm-DockPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}

.lm-DockPanel-handle[data-orientation='horizontal'] {
  cursor: ew-resize;
}

.lm-DockPanel-handle[data-orientation='vertical'] {
  cursor: ns-resize;
}

.lm-DockPanel-handle[data-orientation='horizontal']:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}

.lm-DockPanel-handle[data-orientation='vertical']:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}

.lm-DockPanel-overlay {
  z-index: 3;
  box-sizing: border-box;
  pointer-events: none;
}

.lm-DockPanel-overlay.lm-mod-hidden {
  display: none !important;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-Menu {
  z-index: 10000;
  position: absolute;
  white-space: nowrap;
  overflow-x: hidden;
  overflow-y: auto;
  outline: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-Menu-content {
  margin: 0;
  padding: 0;
  display: table;
  list-style-type: none;
}

.lm-Menu-item {
  display: table-row;
}

.lm-Menu-item.lm-mod-hidden,
.lm-Menu-item.lm-mod-collapsed {
  display: none !important;
}

.lm-Menu-itemIcon,
.lm-Menu-itemSubmenuIcon {
  display: table-cell;
  text-align: center;
}

.lm-Menu-itemLabel {
  display: table-cell;
  text-align: left;
}

.lm-Menu-itemShortcut {
  display: table-cell;
  text-align: right;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-MenuBar {
  outline: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-MenuBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: row;
  list-style-type: none;
}

.lm-MenuBar-item {
  box-sizing: border-box;
}

.lm-MenuBar-itemIcon,
.lm-MenuBar-itemLabel {
  display: inline-block;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-ScrollBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-ScrollBar[data-orientation='horizontal'] {
  flex-direction: row;
}

.lm-ScrollBar[data-orientation='vertical'] {
  flex-direction: column;
}

.lm-ScrollBar-button {
  box-sizing: border-box;
  flex: 0 0 auto;
}

.lm-ScrollBar-track {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
  flex: 1 1 auto;
}

.lm-ScrollBar-thumb {
  box-sizing: border-box;
  position: absolute;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-SplitPanel-child {
  z-index: 0;
}

.lm-SplitPanel-handle {
  z-index: 1;
}

.lm-SplitPanel-handle.lm-mod-hidden {
  display: none !important;
}

.lm-SplitPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}

.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle {
  cursor: ew-resize;
}

.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle {
  cursor: ns-resize;
}

.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}

.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-TabBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-TabBar[data-orientation='horizontal'] {
  flex-direction: row;
  align-items: flex-end;
}

.lm-TabBar[data-orientation='vertical'] {
  flex-direction: column;
  align-items: flex-end;
}

.lm-TabBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex: 1 1 auto;
  list-style-type: none;
}

.lm-TabBar[data-orientation='horizontal'] > .lm-TabBar-content {
  flex-direction: row;
}

.lm-TabBar[data-orientation='vertical'] > .lm-TabBar-content {
  flex-direction: column;
}

.lm-TabBar-tab {
  display: flex;
  flex-direction: row;
  box-sizing: border-box;
  overflow: hidden;
  touch-action: none; /* Disable native Drag/Drop */
}

.lm-TabBar-tabIcon,
.lm-TabBar-tabCloseIcon {
  flex: 0 0 auto;
}

.lm-TabBar-tabLabel {
  flex: 1 1 auto;
  overflow: hidden;
  white-space: nowrap;
}

.lm-TabBar-tabInput {
  user-select: all;
  width: 100%;
  box-sizing: border-box;
}

.lm-TabBar-tab.lm-mod-hidden {
  display: none !important;
}

.lm-TabBar-addButton.lm-mod-hidden {
  display: none !important;
}

.lm-TabBar.lm-mod-dragging .lm-TabBar-tab {
  position: relative;
}

.lm-TabBar.lm-mod-dragging[data-orientation='horizontal'] .lm-TabBar-tab {
  left: 0;
  transition: left 150ms ease;
}

.lm-TabBar.lm-mod-dragging[data-orientation='vertical'] .lm-TabBar-tab {
  top: 0;
  transition: top 150ms ease;
}

.lm-TabBar.lm-mod-dragging .lm-TabBar-tab.lm-mod-dragging {
  transition: none;
}

.lm-TabBar-tabLabel .lm-TabBar-tabInput {
  user-select: all;
  width: 100%;
  box-sizing: border-box;
  background: inherit;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-TabPanel-tabBar {
  z-index: 1;
}

.lm-TabPanel-stackedPanel {
  z-index: 0;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Collapse {
  display: flex;
  flex-direction: column;
  align-items: stretch;
}

.jp-Collapse-header {
  padding: 1px 12px;
  background-color: var(--jp-layout-color1);
  border-bottom: solid var(--jp-border-width) var(--jp-border-color2);
  color: var(--jp-ui-font-color1);
  cursor: pointer;
  display: flex;
  align-items: center;
  font-size: var(--jp-ui-font-size0);
  font-weight: 600;
  text-transform: uppercase;
  user-select: none;
}

.jp-Collapser-icon {
  height: 16px;
}

.jp-Collapse-header-collapsed .jp-Collapser-icon {
  transform: rotate(-90deg);
  margin: auto 0;
}

.jp-Collapser-title {
  line-height: 25px;
}

.jp-Collapse-contents {
  padding: 0 12px;
  background-color: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  overflow: auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* This file was auto-generated by ensureUiComponents() in @jupyterlab/buildutils */

/**
 * (DEPRECATED) Support for consuming icons as CSS background images
 */

/* Icons urls */

:root {
  --jp-icon-add-above: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPGcgY2xpcC1wYXRoPSJ1cmwoI2NsaXAwXzEzN18xOTQ5MikiPgo8cGF0aCBjbGFzcz0ianAtaWNvbjMiIGQ9Ik00Ljc1IDQuOTMwNjZINi42MjVWNi44MDU2NkM2LjYyNSA3LjAxMTkxIDYuNzkzNzUgNy4xODA2NiA3IDcuMTgwNjZDNy4yMDYyNSA3LjE4MDY2IDcuMzc1IDcuMDExOTEgNy4zNzUgNi44MDU2NlY0LjkzMDY2SDkuMjVDOS40NTYyNSA0LjkzMDY2IDkuNjI1IDQuNzYxOTEgOS42MjUgNC41NTU2NkM5LjYyNSA0LjM0OTQxIDkuNDU2MjUgNC4xODA2NiA5LjI1IDQuMTgwNjZINy4zNzVWMi4zMDU2NkM3LjM3NSAyLjA5OTQxIDcuMjA2MjUgMS45MzA2NiA3IDEuOTMwNjZDNi43OTM3NSAxLjkzMDY2IDYuNjI1IDIuMDk5NDEgNi42MjUgMi4zMDU2NlY0LjE4MDY2SDQuNzVDNC41NDM3NSA0LjE4MDY2IDQuMzc1IDQuMzQ5NDEgNC4zNzUgNC41NTU2NkM0LjM3NSA0Ljc2MTkxIDQuNTQzNzUgNC45MzA2NiA0Ljc1IDQuOTMwNjZaIiBmaWxsPSIjNjE2MTYxIiBzdHJva2U9IiM2MTYxNjEiIHN0cm9rZS13aWR0aD0iMC43Ii8+CjwvZz4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGNsaXAtcnVsZT0iZXZlbm9kZCIgZD0iTTExLjUgOS41VjExLjVMMi41IDExLjVWOS41TDExLjUgOS41Wk0xMiA4QzEyLjU1MjMgOCAxMyA4LjQ0NzcyIDEzIDlWMTJDMTMgMTIuNTUyMyAxMi41NTIzIDEzIDEyIDEzTDIgMTNDMS40NDc3MiAxMyAxIDEyLjU1MjMgMSAxMlY5QzEgOC40NDc3MiAxLjQ0NzcxIDggMiA4TDEyIDhaIiBmaWxsPSIjNjE2MTYxIi8+CjxkZWZzPgo8Y2xpcFBhdGggaWQ9ImNsaXAwXzEzN18xOTQ5MiI+CjxyZWN0IGNsYXNzPSJqcC1pY29uMyIgd2lkdGg9IjYiIGhlaWdodD0iNiIgZmlsbD0id2hpdGUiIHRyYW5zZm9ybT0ibWF0cml4KC0xIDAgMCAxIDEwIDEuNTU1NjYpIi8+CjwvY2xpcFBhdGg+CjwvZGVmcz4KPC9zdmc+Cg==);
  --jp-icon-add-below: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPGcgY2xpcC1wYXRoPSJ1cmwoI2NsaXAwXzEzN18xOTQ5OCkiPgo8cGF0aCBjbGFzcz0ianAtaWNvbjMiIGQ9Ik05LjI1IDEwLjA2OTNMNy4zNzUgMTAuMDY5M0w3LjM3NSA4LjE5NDM0QzcuMzc1IDcuOTg4MDkgNy4yMDYyNSA3LjgxOTM0IDcgNy44MTkzNEM2Ljc5Mzc1IDcuODE5MzQgNi42MjUgNy45ODgwOSA2LjYyNSA4LjE5NDM0TDYuNjI1IDEwLjA2OTNMNC43NSAxMC4wNjkzQzQuNTQzNzUgMTAuMDY5MyA0LjM3NSAxMC4yMzgxIDQuMzc1IDEwLjQ0NDNDNC4zNzUgMTAuNjUwNiA0LjU0Mzc1IDEwLjgxOTMgNC43NSAxMC44MTkzTDYuNjI1IDEwLjgxOTNMNi42MjUgMTIuNjk0M0M2LjYyNSAxMi45MDA2IDYuNzkzNzUgMTMuMDY5MyA3IDEzLjA2OTNDNy4yMDYyNSAxMy4wNjkzIDcuMzc1IDEyLjkwMDYgNy4zNzUgMTIuNjk0M0w3LjM3NSAxMC44MTkzTDkuMjUgMTAuODE5M0M5LjQ1NjI1IDEwLjgxOTMgOS42MjUgMTAuNjUwNiA5LjYyNSAxMC40NDQzQzkuNjI1IDEwLjIzODEgOS40NTYyNSAxMC4wNjkzIDkuMjUgMTAuMDY5M1oiIGZpbGw9IiM2MTYxNjEiIHN0cm9rZT0iIzYxNjE2MSIgc3Ryb2tlLXdpZHRoPSIwLjciLz4KPC9nPgo8cGF0aCBjbGFzcz0ianAtaWNvbjMiIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNMi41IDUuNUwyLjUgMy41TDExLjUgMy41TDExLjUgNS41TDIuNSA1LjVaTTIgN0MxLjQ0NzcyIDcgMSA2LjU1MjI4IDEgNkwxIDNDMSAyLjQ0NzcyIDEuNDQ3NzIgMiAyIDJMMTIgMkMxMi41NTIzIDIgMTMgMi40NDc3MiAxMyAzTDEzIDZDMTMgNi41NTIyOSAxMi41NTIzIDcgMTIgN0wyIDdaIiBmaWxsPSIjNjE2MTYxIi8+CjxkZWZzPgo8Y2xpcFBhdGggaWQ9ImNsaXAwXzEzN18xOTQ5OCI+CjxyZWN0IGNsYXNzPSJqcC1pY29uMyIgd2lkdGg9IjYiIGhlaWdodD0iNiIgZmlsbD0id2hpdGUiIHRyYW5zZm9ybT0ibWF0cml4KDEgMS43NDg0NmUtMDcgMS43NDg0NmUtMDcgLTEgNCAxMy40NDQzKSIvPgo8L2NsaXBQYXRoPgo8L2RlZnM+Cjwvc3ZnPgo=);
  --jp-icon-add: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDEzaC02djZoLTJ2LTZINXYtMmg2VjVoMnY2aDZ2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-bell: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE2IDE2IiB2ZXJzaW9uPSIxLjEiPgogICA8cGF0aCBjbGFzcz0ianAtaWNvbjIganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMzMzMzMzIgogICAgICBkPSJtOCAwLjI5Yy0xLjQgMC0yLjcgMC43My0zLjYgMS44LTEuMiAxLjUtMS40IDMuNC0xLjUgNS4yLTAuMTggMi4yLTAuNDQgNC0yLjMgNS4zbDAuMjggMS4zaDVjMC4wMjYgMC42NiAwLjMyIDEuMSAwLjcxIDEuNSAwLjg0IDAuNjEgMiAwLjYxIDIuOCAwIDAuNTItMC40IDAuNi0xIDAuNzEtMS41aDVsMC4yOC0xLjNjLTEuOS0wLjk3LTIuMi0zLjMtMi4zLTUuMy0wLjEzLTEuOC0wLjI2LTMuNy0xLjUtNS4yLTAuODUtMS0yLjItMS44LTMuNi0xLjh6bTAgMS40YzAuODggMCAxLjkgMC41NSAyLjUgMS4zIDAuODggMS4xIDEuMSAyLjcgMS4yIDQuNCAwLjEzIDEuNyAwLjIzIDMuNiAxLjMgNS4yaC0xMGMxLjEtMS42IDEuMi0zLjQgMS4zLTUuMiAwLjEzLTEuNyAwLjMtMy4zIDEuMi00LjQgMC41OS0wLjcyIDEuNi0xLjMgMi41LTEuM3ptLTAuNzQgMTJoMS41Yy0wLjAwMTUgMC4yOCAwLjAxNSAwLjc5LTAuNzQgMC43OS0wLjczIDAuMDAxNi0wLjcyLTAuNTMtMC43NC0wLjc5eiIgLz4KPC9zdmc+Cg==);
  --jp-icon-bug-dot: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiPgogICAgICAgIDxwYXRoIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNMTcuMTkgOEgyMFYxMEgxNy45MUMxNy45NiAxMC4zMyAxOCAxMC42NiAxOCAxMVYxMkgyMFYxNEgxOC41SDE4VjE0LjAyNzVDMTUuNzUgMTQuMjc2MiAxNCAxNi4xODM3IDE0IDE4LjVDMTQgMTkuMjA4IDE0LjE2MzUgMTkuODc3OSAxNC40NTQ5IDIwLjQ3MzlDMTMuNzA2MyAyMC44MTE3IDEyLjg3NTcgMjEgMTIgMjFDOS43OCAyMSA3Ljg1IDE5Ljc5IDYuODEgMThINFYxNkg2LjA5QzYuMDQgMTUuNjcgNiAxNS4zNCA2IDE1VjE0SDRWMTJINlYxMUM2IDEwLjY2IDYuMDQgMTAuMzMgNi4wOSAxMEg0VjhINi44MUM3LjI2IDcuMjIgNy44OCA2LjU1IDguNjIgNi4wNEw3IDQuNDFMOC40MSAzTDEwLjU5IDUuMTdDMTEuMDQgNS4wNiAxMS41MSA1IDEyIDVDMTIuNDkgNSAxMi45NiA1LjA2IDEzLjQyIDUuMTdMMTUuNTkgM0wxNyA0LjQxTDE1LjM3IDYuMDRDMTYuMTIgNi41NSAxNi43NCA3LjIyIDE3LjE5IDhaTTEwIDE2SDE0VjE0SDEwVjE2Wk0xMCAxMkgxNFYxMEgxMFYxMloiIGZpbGw9IiM2MTYxNjEiLz4KICAgICAgICA8cGF0aCBkPSJNMjIgMTguNUMyMiAyMC40MzMgMjAuNDMzIDIyIDE4LjUgMjJDMTYuNTY3IDIyIDE1IDIwLjQzMyAxNSAxOC41QzE1IDE2LjU2NyAxNi41NjcgMTUgMTguNSAxNUMyMC40MzMgMTUgMjIgMTYuNTY3IDIyIDE4LjVaIiBmaWxsPSIjNjE2MTYxIi8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-bug: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0yMCA4aC0yLjgxYy0uNDUtLjc4LTEuMDctMS40NS0xLjgyLTEuOTZMMTcgNC40MSAxNS41OSAzbC0yLjE3IDIuMTdDMTIuOTYgNS4wNiAxMi40OSA1IDEyIDVjLS40OSAwLS45Ni4wNi0xLjQxLjE3TDguNDEgMyA3IDQuNDFsMS42MiAxLjYzQzcuODggNi41NSA3LjI2IDcuMjIgNi44MSA4SDR2MmgyLjA5Yy0uMDUuMzMtLjA5LjY2LS4wOSAxdjFINHYyaDJ2MWMwIC4zNC4wNC42Ny4wOSAxSDR2MmgyLjgxYzEuMDQgMS43OSAyLjk3IDMgNS4xOSAzczQuMTUtMS4yMSA1LjE5LTNIMjB2LTJoLTIuMDljLjA1LS4zMy4wOS0uNjYuMDktMXYtMWgydi0yaC0ydi0xYzAtLjM0LS4wNC0uNjctLjA5LTFIMjBWOHptLTYgOGgtNHYtMmg0djJ6bTAtNGgtNHYtMmg0djJ6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-build: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE0LjkgMTcuNDVDMTYuMjUgMTcuNDUgMTcuMzUgMTYuMzUgMTcuMzUgMTVDMTcuMzUgMTMuNjUgMTYuMjUgMTIuNTUgMTQuOSAxMi41NUMxMy41NCAxMi41NSAxMi40NSAxMy42NSAxMi40NSAxNUMxMi40NSAxNi4zNSAxMy41NCAxNy40NSAxNC45IDE3LjQ1Wk0yMC4xIDE1LjY4TDIxLjU4IDE2Ljg0QzIxLjcxIDE2Ljk1IDIxLjc1IDE3LjEzIDIxLjY2IDE3LjI5TDIwLjI2IDE5LjcxQzIwLjE3IDE5Ljg2IDIwIDE5LjkyIDE5LjgzIDE5Ljg2TDE4LjA5IDE5LjE2QzE3LjczIDE5LjQ0IDE3LjMzIDE5LjY3IDE2LjkxIDE5Ljg1TDE2LjY0IDIxLjdDMTYuNjIgMjEuODcgMTYuNDcgMjIgMTYuMyAyMkgxMy41QzEzLjMyIDIyIDEzLjE4IDIxLjg3IDEzLjE1IDIxLjdMMTIuODkgMTkuODVDMTIuNDYgMTkuNjcgMTIuMDcgMTkuNDQgMTEuNzEgMTkuMTZMOS45NjAwMiAxOS44NkM5LjgxMDAyIDE5LjkyIDkuNjIwMDIgMTkuODYgOS41NDAwMiAxOS43MUw4LjE0MDAyIDE3LjI5QzguMDUwMDIgMTcuMTMgOC4wOTAwMiAxNi45NSA4LjIyMDAyIDE2Ljg0TDkuNzAwMDIgMTUuNjhMOS42NTAwMSAxNUw5LjcwMDAyIDE0LjMxTDguMjIwMDIgMTMuMTZDOC4wOTAwMiAxMy4wNSA4LjA1MDAyIDEyLjg2IDguMTQwMDIgMTIuNzFMOS41NDAwMiAxMC4yOUM5LjYyMDAyIDEwLjEzIDkuODEwMDIgMTAuMDcgOS45NjAwMiAxMC4xM0wxMS43MSAxMC44NEMxMi4wNyAxMC41NiAxMi40NiAxMC4zMiAxMi44OSAxMC4xNUwxMy4xNSA4LjI4OTk4QzEzLjE4IDguMTI5OTggMTMuMzIgNy45OTk5OCAxMy41IDcuOTk5OThIMTYuM0MxNi40NyA3Ljk5OTk4IDE2LjYyIDguMTI5OTggMTYuNjQgOC4yODk5OEwxNi45MSAxMC4xNUMxNy4zMyAxMC4zMiAxNy43MyAxMC41NiAxOC4wOSAxMC44NEwxOS44MyAxMC4xM0MyMCAxMC4wNyAyMC4xNyAxMC4xMyAyMC4yNiAxMC4yOUwyMS42NiAxMi43MUMyMS43NSAxMi44NiAyMS43MSAxMy4wNSAyMS41OCAxMy4xNkwyMC4xIDE0LjMxTDIwLjE1IDE1TDIwLjEgMTUuNjhaIi8+CiAgICA8cGF0aCBkPSJNNy4zMjk2NiA3LjQ0NDU0QzguMDgzMSA3LjAwOTU0IDguMzM5MzIgNi4wNTMzMiA3LjkwNDMyIDUuMjk5ODhDNy40NjkzMiA0LjU0NjQzIDYuNTA4MSA0LjI4MTU2IDUuNzU0NjYgNC43MTY1NkM1LjM5MTc2IDQuOTI2MDggNS4xMjY5NSA1LjI3MTE4IDUuMDE4NDkgNS42NzU5NEM0LjkxMDA0IDYuMDgwNzEgNC45NjY4MiA2LjUxMTk4IDUuMTc2MzQgNi44NzQ4OEM1LjYxMTM0IDcuNjI4MzIgNi41NzYyMiA3Ljg3OTU0IDcuMzI5NjYgNy40NDQ1NFpNOS42NTcxOCA0Ljc5NTkzTDEwLjg2NzIgNC45NTE3OUMxMC45NjI4IDQuOTc3NDEgMTEuMDQwMiA1LjA3MTMzIDExLjAzODIgNS4xODc5M0wxMS4wMzg4IDYuOTg4OTNDMTEuMDQ1NSA3LjEwMDU0IDEwLjk2MTYgNy4xOTUxOCAxMC44NTUgNy4yMTA1NEw5LjY2MDAxIDcuMzgwODNMOS4yMzkxNSA4LjEzMTg4TDkuNjY5NjEgOS4yNTc0NUM5LjcwNzI5IDkuMzYyNzEgOS42NjkzNCA5LjQ3Njk5IDkuNTc0MDggOS41MzE5OUw4LjAxNTIzIDEwLjQzMkM3LjkxMTMxIDEwLjQ5MiA3Ljc5MzM3IDEwLjQ2NzcgNy43MjEwNSAxMC4zODI0TDYuOTg3NDggOS40MzE4OEw2LjEwOTMxIDkuNDMwODNMNS4zNDcwNCAxMC4zOTA1QzUuMjg5MDkgMTAuNDcwMiA1LjE3MzgzIDEwLjQ5MDUgNS4wNzE4NyAxMC40MzM5TDMuNTEyNDUgOS41MzI5M0MzLjQxMDQ5IDkuNDc2MzMgMy4zNzY0NyA5LjM1NzQxIDMuNDEwNzUgOS4yNTY3OUwzLjg2MzQ3IDguMTQwOTNMMy42MTc0OSA3Ljc3NDg4TDMuNDIzNDcgNy4zNzg4M0wyLjIzMDc1IDcuMjEyOTdDMi4xMjY0NyA3LjE5MjM1IDIuMDQwNDkgNy4xMDM0MiAyLjA0MjQ1IDYuOTg2ODJMMi4wNDE4NyA1LjE4NTgyQzIuMDQzODMgNS4wNjkyMiAyLjExOTA5IDQuOTc5NTggMi4yMTcwNCA0Ljk2OTIyTDMuNDIwNjUgNC43OTM5M0wzLjg2NzQ5IDQuMDI3ODhMMy40MTEwNSAyLjkxNzMxQzMuMzczMzcgMi44MTIwNCAzLjQxMTMxIDIuNjk3NzYgMy41MTUyMyAyLjYzNzc2TDUuMDc0MDggMS43Mzc3NkM1LjE2OTM0IDEuNjgyNzYgNS4yODcyOSAxLjcwNzA0IDUuMzU5NjEgMS43OTIzMUw2LjExOTE1IDIuNzI3ODhMNi45ODAwMSAyLjczODkzTDcuNzI0OTYgMS43ODkyMkM3Ljc5MTU2IDEuNzA0NTggNy45MTU0OCAxLjY3OTIyIDguMDA4NzkgMS43NDA4Mkw5LjU2ODIxIDIuNjQxODJDOS42NzAxNyAyLjY5ODQyIDkuNzEyODUgMi44MTIzNCA5LjY4NzIzIDIuOTA3OTdMOS4yMTcxOCA0LjAzMzgzTDkuNDYzMTYgNC4zOTk4OEw5LjY1NzE4IDQuNzk1OTNaIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down-empty-thin: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iOS45LDEzLjYgMy42LDcuNCA0LjQsNi42IDkuOSwxMi4yIDE1LjQsNi43IDE2LjEsNy40ICIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down-empty: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik01LjIsNS45TDksOS43bDMuOC0zLjhsMS4yLDEuMmwtNC45LDVsLTQuOS01TDUuMiw1Ljl6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik01LjIsNy41TDksMTEuMmwzLjgtMy44SDUuMnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-caret-left: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwYXRoIGQ9Ik0xMC44LDEyLjhMNy4xLDlsMy44LTMuOGwwLDcuNkgxMC44eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-caret-right: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik03LjIsNS4yTDEwLjksOWwtMy44LDMuOFY1LjJINy4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-caret-up-empty-thin: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iMTUuNCwxMy4zIDkuOSw3LjcgNC40LDEzLjIgMy42LDEyLjUgOS45LDYuMyAxNi4xLDEyLjYgIi8+Cgk8L2c+Cjwvc3ZnPgo=);
  --jp-icon-caret-up: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwYXRoIGQ9Ik01LjIsMTAuNUw5LDYuOGwzLjgsMy44SDUuMnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-case-sensitive: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0MTQxNDEiPgogICAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiAgPC9nPgogIDxnIGNsYXNzPSJqcC1pY29uLWFjY2VudDIiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTcuNiw4aDAuOWwzLjUsOGgtMS4xTDEwLDE0SDZsLTAuOSwySDRMNy42LDh6IE04LDkuMUw2LjQsMTNoMy4yTDgsOS4xeiIvPgogICAgPHBhdGggZD0iTTE2LjYsOS44Yy0wLjIsMC4xLTAuNCwwLjEtMC43LDAuMWMtMC4yLDAtMC40LTAuMS0wLjYtMC4yYy0wLjEtMC4xLTAuMi0wLjQtMC4yLTAuNyBjLTAuMywwLjMtMC42LDAuNS0wLjksMC43Yy0wLjMsMC4xLTAuNywwLjItMS4xLDAuMmMtMC4zLDAtMC41LDAtMC43LTAuMWMtMC4yLTAuMS0wLjQtMC4yLTAuNi0wLjNjLTAuMi0wLjEtMC4zLTAuMy0wLjQtMC41IGMtMC4xLTAuMi0wLjEtMC40LTAuMS0wLjdjMC0wLjMsMC4xLTAuNiwwLjItMC44YzAuMS0wLjIsMC4zLTAuNCwwLjQtMC41QzEyLDcsMTIuMiw2LjksMTIuNSw2LjhjMC4yLTAuMSwwLjUtMC4xLDAuNy0wLjIgYzAuMy0wLjEsMC41LTAuMSwwLjctMC4xYzAuMiwwLDAuNC0wLjEsMC42LTAuMWMwLjIsMCwwLjMtMC4xLDAuNC0wLjJjMC4xLTAuMSwwLjItMC4yLDAuMi0wLjRjMC0xLTEuMS0xLTEuMy0xIGMtMC40LDAtMS40LDAtMS40LDEuMmgtMC45YzAtMC40LDAuMS0wLjcsMC4yLTFjMC4xLTAuMiwwLjMtMC40LDAuNS0wLjZjMC4yLTAuMiwwLjUtMC4zLDAuOC0wLjNDMTMuMyw0LDEzLjYsNCwxMy45LDQgYzAuMywwLDAuNSwwLDAuOCwwLjFjMC4zLDAsMC41LDAuMSwwLjcsMC4yYzAuMiwwLjEsMC40LDAuMywwLjUsMC41QzE2LDUsMTYsNS4yLDE2LDUuNnYyLjljMCwwLjIsMCwwLjQsMCwwLjUgYzAsMC4xLDAuMSwwLjIsMC4zLDAuMmMwLjEsMCwwLjIsMCwwLjMsMFY5Ljh6IE0xNS4yLDYuOWMtMS4yLDAuNi0zLjEsMC4yLTMuMSwxLjRjMCwxLjQsMy4xLDEsMy4xLTAuNVY2Ljl6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-check: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik05IDE2LjE3TDQuODMgMTJsLTEuNDIgMS40MUw5IDE5IDIxIDdsLTEuNDEtMS40MXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-circle-empty: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyIDJDNi40NyAyIDIgNi40NyAyIDEyczQuNDcgMTAgMTAgMTAgMTAtNC40NyAxMC0xMFMxNy41MyAyIDEyIDJ6bTAgMThjLTQuNDEgMC04LTMuNTktOC04czMuNTktOCA4LTggOCAzLjU5IDggOC0zLjU5IDgtOCA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-circle: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iOSIgY3k9IjkiIHI9IjgiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-clear: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8bWFzayBpZD0iZG9udXRIb2xlIj4KICAgIDxyZWN0IHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgZmlsbD0id2hpdGUiIC8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSI4IiBmaWxsPSJibGFjayIvPgogIDwvbWFzaz4KCiAgPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxyZWN0IGhlaWdodD0iMTgiIHdpZHRoPSIyIiB4PSIxMSIgeT0iMyIgdHJhbnNmb3JtPSJyb3RhdGUoMzE1LCAxMiwgMTIpIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIxMCIgbWFzaz0idXJsKCNkb251dEhvbGUpIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-close: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1ub25lIGpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIGpwLWljb24zLWhvdmVyIiBmaWxsPSJub25lIj4KICAgIDxjaXJjbGUgY3g9IjEyIiBjeT0iMTIiIHI9IjExIi8+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIGpwLWljb24tYWNjZW50Mi1ob3ZlciIgZmlsbD0iIzYxNjE2MSI+CiAgICA8cGF0aCBkPSJNMTkgNi40MUwxNy41OSA1IDEyIDEwLjU5IDYuNDEgNSA1IDYuNDEgMTAuNTkgMTIgNSAxNy41OSA2LjQxIDE5IDEyIDEzLjQxIDE3LjU5IDE5IDE5IDE3LjU5IDEzLjQxIDEyeiIvPgogIDwvZz4KCiAgPGcgY2xhc3M9ImpwLWljb24tbm9uZSBqcC1pY29uLWJ1c3kiIGZpbGw9Im5vbmUiPgogICAgPGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iNyIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-code-check: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBzaGFwZS1yZW5kZXJpbmc9Imdlb21ldHJpY1ByZWNpc2lvbiI+CiAgICA8cGF0aCBkPSJNNi41OSwzLjQxTDIsOEw2LjU5LDEyLjZMOCwxMS4xOEw0LjgyLDhMOCw0LjgyTDYuNTksMy40MU0xMi40MSwzLjQxTDExLDQuODJMMTQuMTgsOEwxMSwxMS4xOEwxMi40MSwxMi42TDE3LDhMMTIuNDEsMy40MU0yMS41OSwxMS41OUwxMy41LDE5LjY4TDkuODMsMTZMOC40MiwxNy40MUwxMy41LDIyLjVMMjMsMTNMMjEuNTksMTEuNTlaIiAvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-code: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTExLjQgMTguNkw2LjggMTRMMTEuNCA5LjRMMTAgOEw0IDE0TDEwIDIwTDExLjQgMTguNlpNMTYuNiAxOC42TDIxLjIgMTRMMTYuNiA5LjRMMTggOEwyNCAxNEwxOCAyMEwxNi42IDE4LjZWMTguNloiLz4KCTwvZz4KPC9zdmc+Cg==);
  --jp-icon-collapse-all: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTggMmMxIDAgMTEgMCAxMiAwczIgMSAyIDJjMCAxIDAgMTEgMCAxMnMwIDItMiAyQzIwIDE0IDIwIDQgMjAgNFMxMCA0IDYgNGMwLTIgMS0yIDItMnoiIC8+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTE4IDhjMC0xLTEtMi0yLTJTNSA2IDQgNnMtMiAxLTIgMmMwIDEgMCAxMSAwIDEyczEgMiAyIDJjMSAwIDExIDAgMTIgMHMyLTEgMi0yYzAtMSAwLTExIDAtMTJ6bS0yIDB2MTJINFY4eiIgLz4KICAgICAgICA8cGF0aCBkPSJNNiAxM3YyaDh2LTJ6IiAvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-console: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwMCAyMDAiPgogIDxnIGNsYXNzPSJqcC1jb25zb2xlLWljb24tYmFja2dyb3VuZC1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMjg4RDEiPgogICAgPHBhdGggZD0iTTIwIDE5LjhoMTYwdjE1OS45SDIweiIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtY29uc29sZS1pY29uLWNvbG9yIGpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIiBmaWxsPSIjZmZmIj4KICAgIDxwYXRoIGQ9Ik0xMDUgMTI3LjNoNDB2MTIuOGgtNDB6TTUxLjEgNzdMNzQgOTkuOWwtMjMuMyAyMy4zIDEwLjUgMTAuNSAyMy4zLTIzLjNMOTUgOTkuOSA4NC41IDg5LjQgNjEuNiA2Ni41eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-copy: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTExLjksMUgzLjJDMi40LDEsMS43LDEuNywxLjcsMi41djEwLjJoMS41VjIuNWg4LjdWMXogTTE0LjEsMy45aC04Yy0wLjgsMC0xLjUsMC43LTEuNSwxLjV2MTAuMmMwLDAuOCwwLjcsMS41LDEuNSwxLjVoOCBjMC44LDAsMS41LTAuNywxLjUtMS41VjUuNEMxNS41LDQuNiwxNC45LDMuOSwxNC4xLDMuOXogTTE0LjEsMTUuNWgtOFY1LjRoOFYxNS41eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-copyright: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGVuYWJsZS1iYWNrZ3JvdW5kPSJuZXcgMCAwIDI0IDI0IiBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCI+CiAgPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0xMS44OCw5LjE0YzEuMjgsMC4wNiwxLjYxLDEuMTUsMS42MywxLjY2aDEuNzljLTAuMDgtMS45OC0xLjQ5LTMuMTktMy40NS0zLjE5QzkuNjQsNy42MSw4LDksOCwxMi4xNCBjMCwxLjk0LDAuOTMsNC4yNCwzLjg0LDQuMjRjMi4yMiwwLDMuNDEtMS42NSwzLjQ0LTIuOTVoLTEuNzljLTAuMDMsMC41OS0wLjQ1LDEuMzgtMS42MywxLjQ0QzEwLjU1LDE0LjgzLDEwLDEzLjgxLDEwLDEyLjE0IEMxMCw5LjI1LDExLjI4LDkuMTYsMTEuODgsOS4xNHogTTEyLDJDNi40OCwyLDIsNi40OCwyLDEyczQuNDgsMTAsMTAsMTBzMTAtNC40OCwxMC0xMFMxNy41MiwyLDEyLDJ6IE0xMiwyMGMtNC40MSwwLTgtMy41OS04LTggczMuNTktOCw4LThzOCwzLjU5LDgsOFMxNi40MSwyMCwxMiwyMHoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-cut: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkuNjQgNy42NGMuMjMtLjUuMzYtMS4wNS4zNi0xLjY0IDAtMi4yMS0xLjc5LTQtNC00UzIgMy43OSAyIDZzMS43OSA0IDQgNGMuNTkgMCAxLjE0LS4xMyAxLjY0LS4zNkwxMCAxMmwtMi4zNiAyLjM2QzcuMTQgMTQuMTMgNi41OSAxNCA2IDE0Yy0yLjIxIDAtNCAxLjc5LTQgNHMxLjc5IDQgNCA0IDQtMS43OSA0LTRjMC0uNTktLjEzLTEuMTQtLjM2LTEuNjRMMTIgMTRsNyA3aDN2LTFMOS42NCA3LjY0ek02IDhjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTAgMTJjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTYtNy41Yy0uMjggMC0uNS0uMjItLjUtLjVzLjIyLS41LjUtLjUuNS4yMi41LjUtLjIyLjUtLjUuNXpNMTkgM2wtNiA2IDIgMiA3LTdWM3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-delete: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2cHgiIGhlaWdodD0iMTZweCI+CiAgICA8cGF0aCBkPSJNMCAwaDI0djI0SDB6IiBmaWxsPSJub25lIiAvPgogICAgPHBhdGggY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjI2MjYyIiBkPSJNNiAxOWMwIDEuMS45IDIgMiAyaDhjMS4xIDAgMi0uOSAyLTJWN0g2djEyek0xOSA0aC0zLjVsLTEtMWgtNWwtMSAxSDV2MmgxNFY0eiIgLz4KPC9zdmc+Cg==);
  --jp-icon-download: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDloLTRWM0g5djZINWw3IDcgNy03ek01IDE4djJoMTR2LTJINXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-duplicate: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGNsaXAtcnVsZT0iZXZlbm9kZCIgZD0iTTIuNzk5OTggMC44NzVIOC44OTU4MkM5LjIwMDYxIDAuODc1IDkuNDQ5OTggMS4xMzkxNCA5LjQ0OTk4IDEuNDYxOThDOS40NDk5OCAxLjc4NDgyIDkuMjAwNjEgMi4wNDg5NiA4Ljg5NTgyIDIuMDQ4OTZIMy4zNTQxNUMzLjA0OTM2IDIuMDQ4OTYgMi43OTk5OCAyLjMxMzEgMi43OTk5OCAyLjYzNTk0VjkuNjc5NjlDMi43OTk5OCAxMC4wMDI1IDIuNTUwNjEgMTAuMjY2NyAyLjI0NTgyIDEwLjI2NjdDMS45NDEwMyAxMC4yNjY3IDEuNjkxNjUgMTAuMDAyNSAxLjY5MTY1IDkuNjc5NjlWMi4wNDg5NkMxLjY5MTY1IDEuNDAzMjggMi4xOTA0IDAuODc1IDIuNzk5OTggMC44NzVaTTUuMzY2NjUgMTEuOVY0LjU1SDExLjA4MzNWMTEuOUg1LjM2NjY1Wk00LjE0MTY1IDQuMTQxNjdDNC4xNDE2NSAzLjY5MDYzIDQuNTA3MjggMy4zMjUgNC45NTgzMiAzLjMyNUgxMS40OTE3QzExLjk0MjcgMy4zMjUgMTIuMzA4MyAzLjY5MDYzIDEyLjMwODMgNC4xNDE2N1YxMi4zMDgzQzEyLjMwODMgMTIuNzU5NCAxMS45NDI3IDEzLjEyNSAxMS40OTE3IDEzLjEyNUg0Ljk1ODMyQzQuNTA3MjggMTMuMTI1IDQuMTQxNjUgMTIuNzU5NCA0LjE0MTY1IDEyLjMwODNWNC4xNDE2N1oiIGZpbGw9IiM2MTYxNjEiLz4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBkPSJNOS40MzU3NCA4LjI2NTA3SDguMzY0MzFWOS4zMzY1QzguMzY0MzEgOS40NTQzNSA4LjI2Nzg4IDkuNTUwNzggOC4xNTAwMiA5LjU1MDc4QzguMDMyMTcgOS41NTA3OCA3LjkzNTc0IDkuNDU0MzUgNy45MzU3NCA5LjMzNjVWOC4yNjUwN0g2Ljg2NDMxQzYuNzQ2NDUgOC4yNjUwNyA2LjY1MDAyIDguMTY4NjQgNi42NTAwMiA4LjA1MDc4QzYuNjUwMDIgNy45MzI5MiA2Ljc0NjQ1IDcuODM2NSA2Ljg2NDMxIDcuODM2NUg3LjkzNTc0VjYuNzY1MDdDNy45MzU3NCA2LjY0NzIxIDguMDMyMTcgNi41NTA3OCA4LjE1MDAyIDYuNTUwNzhDOC4yNjc4OCA2LjU1MDc4IDguMzY0MzEgNi42NDcyMSA4LjM2NDMxIDYuNzY1MDdWNy44MzY1SDkuNDM1NzRDOS41NTM2IDcuODM2NSA5LjY1MDAyIDcuOTMyOTIgOS42NTAwMiA4LjA1MDc4QzkuNjUwMDIgOC4xNjg2NCA5LjU1MzYgOC4yNjUwNyA5LjQzNTc0IDguMjY1MDdaIiBmaWxsPSIjNjE2MTYxIiBzdHJva2U9IiM2MTYxNjEiIHN0cm9rZS13aWR0aD0iMC41Ii8+Cjwvc3ZnPgo=);
  --jp-icon-edit: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMgMTcuMjVWMjFoMy43NUwxNy44MSA5Ljk0bC0zLjc1LTMuNzVMMyAxNy4yNXpNMjAuNzEgNy4wNGMuMzktLjM5LjM5LTEuMDIgMC0xLjQxbC0yLjM0LTIuMzRjLS4zOS0uMzktMS4wMi0uMzktMS40MSAwbC0xLjgzIDEuODMgMy43NSAzLjc1IDEuODMtMS44M3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-ellipses: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iNSIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxOSIgY3k9IjEyIiByPSIyIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-error: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj48Y2lyY2xlIGN4PSIxMiIgY3k9IjE5IiByPSIyIi8+PHBhdGggZD0iTTEwIDNoNHYxMmgtNHoiLz48L2c+CjxwYXRoIGZpbGw9Im5vbmUiIGQ9Ik0wIDBoMjR2MjRIMHoiLz4KPC9zdmc+Cg==);
  --jp-icon-expand-all: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTggMmMxIDAgMTEgMCAxMiAwczIgMSAyIDJjMCAxIDAgMTEgMCAxMnMwIDItMiAyQzIwIDE0IDIwIDQgMjAgNFMxMCA0IDYgNGMwLTIgMS0yIDItMnoiIC8+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTE4IDhjMC0xLTEtMi0yLTJTNSA2IDQgNnMtMiAxLTIgMmMwIDEgMCAxMSAwIDEyczEgMiAyIDJjMSAwIDExIDAgMTIgMHMyLTEgMi0yYzAtMSAwLTExIDAtMTJ6bS0yIDB2MTJINFY4eiIgLz4KICAgICAgICA8cGF0aCBkPSJNMTEgMTBIOXYzSDZ2MmgzdjNoMnYtM2gzdi0yaC0zeiIgLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-extension: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwLjUgMTFIMTlWN2MwLTEuMS0uOS0yLTItMmgtNFYzLjVDMTMgMi4xMiAxMS44OCAxIDEwLjUgMVM4IDIuMTIgOCAzLjVWNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAydjMuOEgzLjVjMS40OSAwIDIuNyAxLjIxIDIuNyAyLjdzLTEuMjEgMi43LTIuNyAyLjdIMlYyMGMwIDEuMS45IDIgMiAyaDMuOHYtMS41YzAtMS40OSAxLjIxLTIuNyAyLjctMi43IDEuNDkgMCAyLjcgMS4yMSAyLjcgMi43VjIySDE3YzEuMSAwIDItLjkgMi0ydi00aDEuNWMxLjM4IDAgMi41LTEuMTIgMi41LTIuNVMyMS44OCAxMSAyMC41IDExeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-fast-forward: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTQgMThsOC41LTZMNCA2djEyem05LTEydjEybDguNS02TDEzIDZ6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-file-upload: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkgMTZoNnYtNmg0bC03LTctNyA3aDR6bS00IDJoMTR2Mkg1eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-file: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuMyA4LjJsLTUuNS01LjVjLS4zLS4zLS43LS41LTEuMi0uNUgzLjljLS44LjEtMS42LjktMS42IDEuOHYxNC4xYzAgLjkuNyAxLjYgMS42IDEuNmgxNC4yYy45IDAgMS42LS43IDEuNi0xLjZWOS40Yy4xLS41LS4xLS45LS40LTEuMnptLTUuOC0zLjNsMy40IDMuNmgtMy40VjQuOXptMy45IDEyLjdINC43Yy0uMSAwLS4yIDAtLjItLjJWNC43YzAtLjIuMS0uMy4yLS4zaDcuMnY0LjRzMCAuOC4zIDEuMWMuMy4zIDEuMS4zIDEuMS4zaDQuM3Y3LjJzLS4xLjItLjIuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-filter-dot: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTE0LDEyVjE5Ljg4QzE0LjA0LDIwLjE4IDEzLjk0LDIwLjUgMTMuNzEsMjAuNzFDMTMuMzIsMjEuMSAxMi42OSwyMS4xIDEyLjMsMjAuNzFMMTAuMjksMTguN0MxMC4wNiwxOC40NyA5Ljk2LDE4LjE2IDEwLDE3Ljg3VjEySDkuOTdMNC4yMSw0LjYyQzMuODcsNC4xOSAzLjk1LDMuNTYgNC4zOCwzLjIyQzQuNTcsMy4wOCA0Ljc4LDMgNSwzVjNIMTlWM0MxOS4yMiwzIDE5LjQzLDMuMDggMTkuNjIsMy4yMkMyMC4wNSwzLjU2IDIwLjEzLDQuMTkgMTkuNzksNC42MkwxNC4wMywxMkgxNFoiIC8+CiAgPC9nPgogIDxnIGNsYXNzPSJqcC1pY29uLWRvdCIgZmlsbD0iI0ZGRiI+CiAgICA8Y2lyY2xlIGN4PSIxOCIgY3k9IjE3IiByPSIzIj48L2NpcmNsZT4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-filter-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEwIDE4aDR2LTJoLTR2MnpNMyA2djJoMThWNkgzem0zIDdoMTJ2LTJINnYyeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-filter: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTE0LDEyVjE5Ljg4QzE0LjA0LDIwLjE4IDEzLjk0LDIwLjUgMTMuNzEsMjAuNzFDMTMuMzIsMjEuMSAxMi42OSwyMS4xIDEyLjMsMjAuNzFMMTAuMjksMTguN0MxMC4wNiwxOC40NyA5Ljk2LDE4LjE2IDEwLDE3Ljg3VjEySDkuOTdMNC4yMSw0LjYyQzMuODcsNC4xOSAzLjk1LDMuNTYgNC4zOCwzLjIyQzQuNTcsMy4wOCA0Ljc4LDMgNSwzVjNIMTlWM0MxOS4yMiwzIDE5LjQzLDMuMDggMTkuNjIsMy4yMkMyMC4wNSwzLjU2IDIwLjEzLDQuMTkgMTkuNzksNC42MkwxNC4wMywxMkgxNFoiIC8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-folder-favorite: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjRweCIgdmlld0JveD0iMCAwIDI0IDI0IiB3aWR0aD0iMjRweCIgZmlsbD0iIzAwMDAwMCI+CiAgPHBhdGggZD0iTTAgMGgyNHYyNEgwVjB6IiBmaWxsPSJub25lIi8+PHBhdGggY2xhc3M9ImpwLWljb24zIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzYxNjE2MSIgZD0iTTIwIDZoLThsLTItMkg0Yy0xLjEgMC0yIC45LTIgMnYxMmMwIDEuMS45IDIgMiAyaDE2YzEuMSAwIDItLjkgMi0yVjhjMC0xLjEtLjktMi0yLTJ6bS0yLjA2IDExTDE1IDE1LjI4IDEyLjA2IDE3bC43OC0zLjMzLTIuNTktMi4yNCAzLjQxLS4yOUwxNSA4bDEuMzQgMy4xNCAzLjQxLjI5LTIuNTkgMi4yNC43OCAzLjMzeiIvPgo8L3N2Zz4K);
  --jp-icon-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY4YzAtMS4xLS45LTItMi0yaC04bC0yLTJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-home: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjRweCIgdmlld0JveD0iMCAwIDI0IDI0IiB3aWR0aD0iMjRweCIgZmlsbD0iIzAwMDAwMCI+CiAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPjxwYXRoIGNsYXNzPSJqcC1pY29uMyBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xMCAyMHYtNmg0djZoNXYtOGgzTDEyIDMgMiAxMmgzdjh6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-html5: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uMCBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMDAiIGQ9Ik0xMDguNCAwaDIzdjIyLjhoMjEuMlYwaDIzdjY5aC0yM1Y0NmgtMjF2MjNoLTIzLjJNMjA2IDIzaC0yMC4zVjBoNjMuN3YyM0gyMjl2NDZoLTIzbTUzLjUtNjloMjQuMWwxNC44IDI0LjNMMzEzLjIgMGgyNC4xdjY5aC0yM1YzNC44bC0xNi4xIDI0LjgtMTYuMS0yNC44VjY5aC0yMi42bTg5LjItNjloMjN2NDYuMmgzMi42VjY5aC01NS42Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI2U0NGQyNiIgZD0iTTEwNy42IDQ3MWwtMzMtMzcwLjRoMzYyLjhsLTMzIDM3MC4yTDI1NS43IDUxMiIvPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNmMTY1MjkiIGQ9Ik0yNTYgNDgwLjVWMTMxaDE0OC4zTDM3NiA0NDciLz4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNlYmViZWIiIGQ9Ik0xNDIgMTc2LjNoMTE0djQ1LjRoLTY0LjJsNC4yIDQ2LjVoNjB2NDUuM0gxNTQuNG0yIDIyLjhIMjAybDMuMiAzNi4zIDUwLjggMTMuNnY0Ny40bC05My4yLTI2Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIiBmaWxsPSIjZmZmIiBkPSJNMzY5LjYgMTc2LjNIMjU1Ljh2NDUuNGgxMDkuNm0tNC4xIDQ2LjVIMjU1Ljh2NDUuNGg1NmwtNS4zIDU5LTUwLjcgMTMuNnY0Ny4ybDkzLTI1LjgiLz4KPC9zdmc+Cg==);
  --jp-icon-image: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1icmFuZDQganAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNGRkYiIGQ9Ik0yLjIgMi4yaDE3LjV2MTcuNUgyLjJ6Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzNGNTFCNSIgZD0iTTIuMiAyLjJ2MTcuNWgxNy41bC4xLTE3LjVIMi4yem0xMi4xIDIuMmMxLjIgMCAyLjIgMSAyLjIgMi4ycy0xIDIuMi0yLjIgMi4yLTIuMi0xLTIuMi0yLjIgMS0yLjIgMi4yLTIuMnpNNC40IDE3LjZsMy4zLTguOCAzLjMgNi42IDIuMi0zLjIgNC40IDUuNEg0LjR6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-info: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUwLjk3OCA1MC45NzgiPgoJPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KCQk8cGF0aCBkPSJNNDMuNTIsNy40NThDMzguNzExLDIuNjQ4LDMyLjMwNywwLDI1LjQ4OSwwQzE4LjY3LDAsMTIuMjY2LDIuNjQ4LDcuNDU4LDcuNDU4CgkJCWMtOS45NDMsOS45NDEtOS45NDMsMjYuMTE5LDAsMzYuMDYyYzQuODA5LDQuODA5LDExLjIxMiw3LjQ1NiwxOC4wMzEsNy40NThjMCwwLDAuMDAxLDAsMC4wMDIsMAoJCQljNi44MTYsMCwxMy4yMjEtMi42NDgsMTguMDI5LTcuNDU4YzQuODA5LTQuODA5LDcuNDU3LTExLjIxMiw3LjQ1Ny0xOC4wM0M1MC45NzcsMTguNjcsNDguMzI4LDEyLjI2Niw0My41Miw3LjQ1OHoKCQkJIE00Mi4xMDYsNDIuMTA1Yy00LjQzMiw0LjQzMS0xMC4zMzIsNi44NzItMTYuNjE1LDYuODcyaC0wLjAwMmMtNi4yODUtMC4wMDEtMTIuMTg3LTIuNDQxLTE2LjYxNy02Ljg3MgoJCQljLTkuMTYyLTkuMTYzLTkuMTYyLTI0LjA3MSwwLTMzLjIzM0MxMy4zMDMsNC40NCwxOS4yMDQsMiwyNS40ODksMmM2LjI4NCwwLDEyLjE4NiwyLjQ0LDE2LjYxNyw2Ljg3MgoJCQljNC40MzEsNC40MzEsNi44NzEsMTAuMzMyLDYuODcxLDE2LjYxN0M0OC45NzcsMzEuNzcyLDQ2LjUzNiwzNy42NzUsNDIuMTA2LDQyLjEwNXoiLz4KCQk8cGF0aCBkPSJNMjMuNTc4LDMyLjIxOGMtMC4wMjMtMS43MzQsMC4xNDMtMy4wNTksMC40OTYtMy45NzJjMC4zNTMtMC45MTMsMS4xMS0xLjk5NywyLjI3Mi0zLjI1MwoJCQljMC40NjgtMC41MzYsMC45MjMtMS4wNjIsMS4zNjctMS41NzVjMC42MjYtMC43NTMsMS4xMDQtMS40NzgsMS40MzYtMi4xNzVjMC4zMzEtMC43MDcsMC40OTUtMS41NDEsMC40OTUtMi41CgkJCWMwLTEuMDk2LTAuMjYtMi4wODgtMC43NzktMi45NzljLTAuNTY1LTAuODc5LTEuNTAxLTEuMzM2LTIuODA2LTEuMzY5Yy0xLjgwMiwwLjA1Ny0yLjk4NSwwLjY2Ny0zLjU1LDEuODMyCgkJCWMtMC4zMDEsMC41MzUtMC41MDMsMS4xNDEtMC42MDcsMS44MTRjLTAuMTM5LDAuNzA3LTAuMjA3LDEuNDMyLTAuMjA3LDIuMTc0aC0yLjkzN2MtMC4wOTEtMi4yMDgsMC40MDctNC4xMTQsMS40OTMtNS43MTkKCQkJYzEuMDYyLTEuNjQsMi44NTUtMi40ODEsNS4zNzgtMi41MjdjMi4xNiwwLjAyMywzLjg3NCwwLjYwOCw1LjE0MSwxLjc1OGMxLjI3OCwxLjE2LDEuOTI5LDIuNzY0LDEuOTUsNC44MTEKCQkJYzAsMS4xNDItMC4xMzcsMi4xMTEtMC40MSwyLjkxMWMtMC4zMDksMC44NDUtMC43MzEsMS41OTMtMS4yNjgsMi4yNDNjLTAuNDkyLDAuNjUtMS4wNjgsMS4zMTgtMS43MywyLjAwMgoJCQljLTAuNjUsMC42OTctMS4zMTMsMS40NzktMS45ODcsMi4zNDZjLTAuMjM5LDAuMzc3LTAuNDI5LDAuNzc3LTAuNTY1LDEuMTk5Yy0wLjE2LDAuOTU5LTAuMjE3LDEuOTUxLTAuMTcxLDIuOTc5CgkJCUMyNi41ODksMzIuMjE4LDIzLjU3OCwzMi4yMTgsMjMuNTc4LDMyLjIxOHogTTIzLjU3OCwzOC4yMnYtMy40ODRoMy4wNzZ2My40ODRIMjMuNTc4eiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-inspector: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaW5zcGVjdG9yLWljb24tY29sb3IganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY2YzAtMS4xLS45LTItMi0yem0tNSAxNEg0di00aDExdjR6bTAtNUg0VjloMTF2NHptNSA1aC00VjloNHY5eiIvPgo8L3N2Zz4K);
  --jp-icon-json: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtanNvbi1pY29uLWNvbG9yIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI0Y5QTgyNSI+CiAgICA8cGF0aCBkPSJNMjAuMiAxMS44Yy0xLjYgMC0xLjcuNS0xLjcgMSAwIC40LjEuOS4xIDEuMy4xLjUuMS45LjEgMS4zIDAgMS43LTEuNCAyLjMtMy41IDIuM2gtLjl2LTEuOWguNWMxLjEgMCAxLjQgMCAxLjQtLjggMC0uMyAwLS42LS4xLTEgMC0uNC0uMS0uOC0uMS0xLjIgMC0xLjMgMC0xLjggMS4zLTItMS4zLS4yLTEuMy0uNy0xLjMtMiAwLS40LjEtLjguMS0xLjIuMS0uNC4xLS43LjEtMSAwLS44LS40LS43LTEuNC0uOGgtLjVWNC4xaC45YzIuMiAwIDMuNS43IDMuNSAyLjMgMCAuNC0uMS45LS4xIDEuMy0uMS41LS4xLjktLjEgMS4zIDAgLjUuMiAxIDEuNyAxdjEuOHpNMS44IDEwLjFjMS42IDAgMS43LS41IDEuNy0xIDAtLjQtLjEtLjktLjEtMS4zLS4xLS41LS4xLS45LS4xLTEuMyAwLTEuNiAxLjQtMi4zIDMuNS0yLjNoLjl2MS45aC0uNWMtMSAwLTEuNCAwLTEuNC44IDAgLjMgMCAuNi4xIDEgMCAuMi4xLjYuMSAxIDAgMS4zIDAgMS44LTEuMyAyQzYgMTEuMiA2IDExLjcgNiAxM2MwIC40LS4xLjgtLjEgMS4yLS4xLjMtLjEuNy0uMSAxIDAgLjguMy44IDEuNC44aC41djEuOWgtLjljLTIuMSAwLTMuNS0uNi0zLjUtMi4zIDAtLjQuMS0uOS4xLTEuMy4xLS41LjEtLjkuMS0xLjMgMC0uNS0uMi0xLTEuNy0xdi0xLjl6Ii8+CiAgICA8Y2lyY2xlIGN4PSIxMSIgY3k9IjEzLjgiIHI9IjIuMSIvPgogICAgPGNpcmNsZSBjeD0iMTEiIGN5PSI4LjIiIHI9IjIuMSIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-julia: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDMyNSAzMDAiPgogIDxnIGNsYXNzPSJqcC1icmFuZDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjY2IzYzMzIj4KICAgIDxwYXRoIGQ9Ik0gMTUwLjg5ODQzOCAyMjUgQyAxNTAuODk4NDM4IDI2Ni40MjE4NzUgMTE3LjMyMDMxMiAzMDAgNzUuODk4NDM4IDMwMCBDIDM0LjQ3NjU2MiAzMDAgMC44OTg0MzggMjY2LjQyMTg3NSAwLjg5ODQzOCAyMjUgQyAwLjg5ODQzOCAxODMuNTc4MTI1IDM0LjQ3NjU2MiAxNTAgNzUuODk4NDM4IDE1MCBDIDExNy4zMjAzMTIgMTUwIDE1MC44OTg0MzggMTgzLjU3ODEyNSAxNTAuODk4NDM4IDIyNSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzM4OTgyNiI+CiAgICA8cGF0aCBkPSJNIDIzNy41IDc1IEMgMjM3LjUgMTE2LjQyMTg3NSAyMDMuOTIxODc1IDE1MCAxNjIuNSAxNTAgQyAxMjEuMDc4MTI1IDE1MCA4Ny41IDExNi40MjE4NzUgODcuNSA3NSBDIDg3LjUgMzMuNTc4MTI1IDEyMS4wNzgxMjUgMCAxNjIuNSAwIEMgMjAzLjkyMTg3NSAwIDIzNy41IDMzLjU3ODEyNSAyMzcuNSA3NSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzk1NThiMiI+CiAgICA8cGF0aCBkPSJNIDMyNC4xMDE1NjIgMjI1IEMgMzI0LjEwMTU2MiAyNjYuNDIxODc1IDI5MC41MjM0MzggMzAwIDI0OS4xMDE1NjIgMzAwIEMgMjA3LjY3OTY4OCAzMDAgMTc0LjEwMTU2MiAyNjYuNDIxODc1IDE3NC4xMDE1NjIgMjI1IEMgMTc0LjEwMTU2MiAxODMuNTc4MTI1IDIwNy42Nzk2ODggMTUwIDI0OS4xMDE1NjIgMTUwIEMgMjkwLjUyMzQzOCAxNTAgMzI0LjEwMTU2MiAxODMuNTc4MTI1IDMyNC4xMDE1NjIgMjI1Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-jupyter-favicon: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTUyIiBoZWlnaHQ9IjE2NSIgdmlld0JveD0iMCAwIDE1MiAxNjUiIHZlcnNpb249IjEuMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgPGcgY2xhc3M9ImpwLWp1cHl0ZXItaWNvbi1jb2xvciIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA3ODk0NywgMTEwLjU4MjkyNykiIGQ9Ik03NS45NDIyODQyLDI5LjU4MDQ1NjEgQzQzLjMwMjM5NDcsMjkuNTgwNDU2MSAxNC43OTY3ODMyLDE3LjY1MzQ2MzQgMCwwIEM1LjUxMDgzMjExLDE1Ljg0MDY4MjkgMTUuNzgxNTM4OSwyOS41NjY3NzMyIDI5LjM5MDQ5NDcsMzkuMjc4NDE3MSBDNDIuOTk5Nyw0OC45ODk4NTM3IDU5LjI3MzcsNTQuMjA2NzgwNSA3NS45NjA1Nzg5LDU0LjIwNjc4MDUgQzkyLjY0NzQ1NzksNTQuMjA2NzgwNSAxMDguOTIxNDU4LDQ4Ljk4OTg1MzcgMTIyLjUzMDY2MywzOS4yNzg0MTcxIEMxMzYuMTM5NDUzLDI5LjU2Njc3MzIgMTQ2LjQxMDI4NCwxNS44NDA2ODI5IDE1MS45MjExNTgsMCBDMTM3LjA4Nzg2OCwxNy42NTM0NjM0IDEwOC41ODI1ODksMjkuNTgwNDU2MSA3NS45NDIyODQyLDI5LjU4MDQ1NjEgTDc1Ljk0MjI4NDIsMjkuNTgwNDU2MSBaIiAvPgogICAgPHBhdGggdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMzczNjgsIDAuNzA0ODc4KSIgZD0iTTc1Ljk3ODQ1NzksMjQuNjI2NDA3MyBDMTA4LjYxODc2MywyNC42MjY0MDczIDEzNy4xMjQ0NTgsMzYuNTUzNDQxNSAxNTEuOTIxMTU4LDU0LjIwNjc4MDUgQzE0Ni40MTAyODQsMzguMzY2MjIyIDEzNi4xMzk0NTMsMjQuNjQwMTMxNyAxMjIuNTMwNjYzLDE0LjkyODQ4NzggQzEwOC45MjE0NTgsNS4yMTY4NDM5IDkyLjY0NzQ1NzksMCA3NS45NjA1Nzg5LDAgQzU5LjI3MzcsMCA0Mi45OTk3LDUuMjE2ODQzOSAyOS4zOTA0OTQ3LDE0LjkyODQ4NzggQzE1Ljc4MTUzODksMjQuNjQwMTMxNyA1LjUxMDgzMjExLDM4LjM2NjIyMiAwLDU0LjIwNjc4MDUgQzE0LjgzMzA4MTYsMzYuNTg5OTI5MyA0My4zMzg1Njg0LDI0LjYyNjQwNzMgNzUuOTc4NDU3OSwyNC42MjY0MDczIEw3NS45Nzg0NTc5LDI0LjYyNjQwNzMgWiIgLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-jupyter: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMzkiIGhlaWdodD0iNTEiIHZpZXdCb3g9IjAgMCAzOSA1MSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtMTYzOCAtMjI4MSkiPgogICAgIDxnIGNsYXNzPSJqcC1qdXB5dGVyLWljb24tY29sb3IiIGZpbGw9IiNGMzc3MjYiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5Ljc0IDIzMTEuOTgpIiBkPSJNIDE4LjI2NDYgNy4xMzQxMUMgMTAuNDE0NSA3LjEzNDExIDMuNTU4NzIgNC4yNTc2IDAgMEMgMS4zMjUzOSAzLjgyMDQgMy43OTU1NiA3LjEzMDgxIDcuMDY4NiA5LjQ3MzAzQyAxMC4zNDE3IDExLjgxNTIgMTQuMjU1NyAxMy4wNzM0IDE4LjI2OSAxMy4wNzM0QyAyMi4yODIzIDEzLjA3MzQgMjYuMTk2MyAxMS44MTUyIDI5LjQ2OTQgOS40NzMwM0MgMzIuNzQyNCA3LjEzMDgxIDM1LjIxMjYgMy44MjA0IDM2LjUzOCAwQyAzMi45NzA1IDQuMjU3NiAyNi4xMTQ4IDcuMTM0MTEgMTguMjY0NiA3LjEzNDExWiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5LjczIDIyODUuNDgpIiBkPSJNIDE4LjI3MzMgNS45MzkzMUMgMjYuMTIzNSA1LjkzOTMxIDMyLjk3OTMgOC44MTU4MyAzNi41MzggMTMuMDczNEMgMzUuMjEyNiA5LjI1MzAzIDMyLjc0MjQgNS45NDI2MiAyOS40Njk0IDMuNjAwNEMgMjYuMTk2MyAxLjI1ODE4IDIyLjI4MjMgMCAxOC4yNjkgMEMgMTQuMjU1NyAwIDEwLjM0MTcgMS4yNTgxOCA3LjA2ODYgMy42MDA0QyAzLjc5NTU2IDUuOTQyNjIgMS4zMjUzOSA5LjI1MzAzIDAgMTMuMDczNEMgMy41Njc0NSA4LjgyNDYzIDEwLjQyMzIgNS45MzkzMSAxOC4yNzMzIDUuOTM5MzFaIi8+CiAgICA8L2c+CiAgICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjY5LjMgMjI4MS4zMSkiIGQ9Ik0gNS44OTM1MyAyLjg0NEMgNS45MTg4OSAzLjQzMTY1IDUuNzcwODUgNC4wMTM2NyA1LjQ2ODE1IDQuNTE2NDVDIDUuMTY1NDUgNS4wMTkyMiA0LjcyMTY4IDUuNDIwMTUgNC4xOTI5OSA1LjY2ODUxQyAzLjY2NDMgNS45MTY4OCAzLjA3NDQ0IDYuMDAxNTEgMi40OTgwNSA1LjkxMTcxQyAxLjkyMTY2IDUuODIxOSAxLjM4NDYzIDUuNTYxNyAwLjk1NDg5OCA1LjE2NDAxQyAwLjUyNTE3IDQuNzY2MzMgMC4yMjIwNTYgNC4yNDkwMyAwLjA4MzkwMzcgMy42Nzc1N0MgLTAuMDU0MjQ4MyAzLjEwNjExIC0wLjAyMTIzIDIuNTA2MTcgMC4xNzg3ODEgMS45NTM2NEMgMC4zNzg3OTMgMS40MDExIDAuNzM2ODA5IDAuOTIwODE3IDEuMjA3NTQgMC41NzM1MzhDIDEuNjc4MjYgMC4yMjYyNTkgMi4yNDA1NSAwLjAyNzU5MTkgMi44MjMyNiAwLjAwMjY3MjI5QyAzLjYwMzg5IC0wLjAzMDcxMTUgNC4zNjU3MyAwLjI0OTc4OSA0Ljk0MTQyIDAuNzgyNTUxQyA1LjUxNzExIDEuMzE1MzEgNS44NTk1NiAyLjA1Njc2IDUuODkzNTMgMi44NDRaIi8+CiAgICAgIDxwYXRoIHRyYW5zZm9ybT0idHJhbnNsYXRlKDE2MzkuOCAyMzIzLjgxKSIgZD0iTSA3LjQyNzg5IDMuNTgzMzhDIDcuNDYwMDggNC4zMjQzIDcuMjczNTUgNS4wNTgxOSA2Ljg5MTkzIDUuNjkyMTNDIDYuNTEwMzEgNi4zMjYwNyA1Ljk1MDc1IDYuODMxNTYgNS4yODQxMSA3LjE0NDZDIDQuNjE3NDcgNy40NTc2MyAzLjg3MzcxIDcuNTY0MTQgMy4xNDcwMiA3LjQ1MDYzQyAyLjQyMDMyIDcuMzM3MTIgMS43NDMzNiA3LjAwODcgMS4yMDE4NCA2LjUwNjk1QyAwLjY2MDMyOCA2LjAwNTIgMC4yNzg2MSA1LjM1MjY4IDAuMTA1MDE3IDQuNjMyMDJDIC0wLjA2ODU3NTcgMy45MTEzNSAtMC4wMjYyMzYxIDMuMTU0OTQgMC4yMjY2NzUgMi40NTg1NkMgMC40Nzk1ODcgMS43NjIxNyAwLjkzMTY5NyAxLjE1NzEzIDEuNTI1NzYgMC43MjAwMzNDIDIuMTE5ODMgMC4yODI5MzUgMi44MjkxNCAwLjAzMzQzOTUgMy41NjM4OSAwLjAwMzEzMzQ0QyA0LjU0NjY3IC0wLjAzNzQwMzMgNS41MDUyOSAwLjMxNjcwNiA2LjIyOTYxIDAuOTg3ODM1QyA2Ljk1MzkzIDEuNjU4OTYgNy4zODQ4NCAyLjU5MjM1IDcuNDI3ODkgMy41ODMzOEwgNy40Mjc4OSAzLjU4MzM4WiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM4LjM2IDIyODYuMDYpIiBkPSJNIDIuMjc0NzEgNC4zOTYyOUMgMS44NDM2MyA0LjQxNTA4IDEuNDE2NzEgNC4zMDQ0NSAxLjA0Nzk5IDQuMDc4NDNDIDAuNjc5MjY4IDMuODUyNCAwLjM4NTMyOCAzLjUyMTE0IDAuMjAzMzcxIDMuMTI2NTZDIDAuMDIxNDEzNiAyLjczMTk4IC0wLjA0MDM3OTggMi4yOTE4MyAwLjAyNTgxMTYgMS44NjE4MUMgMC4wOTIwMDMxIDEuNDMxOCAwLjI4MzIwNCAxLjAzMTI2IDAuNTc1MjEzIDAuNzEwODgzQyAwLjg2NzIyMiAwLjM5MDUxIDEuMjQ2OTEgMC4xNjQ3MDggMS42NjYyMiAwLjA2MjA1OTJDIDIuMDg1NTMgLTAuMDQwNTg5NyAyLjUyNTYxIC0wLjAxNTQ3MTQgMi45MzA3NiAwLjEzNDIzNUMgMy4zMzU5MSAwLjI4Mzk0MSAzLjY4NzkyIDAuNTUxNTA1IDMuOTQyMjIgMC45MDMwNkMgNC4xOTY1MiAxLjI1NDYyIDQuMzQxNjkgMS42NzQzNiA0LjM1OTM1IDIuMTA5MTZDIDQuMzgyOTkgMi42OTEwNyA0LjE3Njc4IDMuMjU4NjkgMy43ODU5NyAzLjY4NzQ2QyAzLjM5NTE2IDQuMTE2MjQgMi44NTE2NiA0LjM3MTE2IDIuMjc0NzEgNC4zOTYyOUwgMi4yNzQ3MSA0LjM5NjI5WiIvPgogICAgPC9nPgogIDwvZz4+Cjwvc3ZnPgo=);
  --jp-icon-jupyterlab-wordmark: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyMDAiIHZpZXdCb3g9IjAgMCAxODYwLjggNDc1Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0RTRFNEUiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDQ4MC4xMzY0MDEsIDY0LjI3MTQ5MykiPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMDAwMDAsIDU4Ljg3NTU2NikiPgogICAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA4NzYwMywgMC4xNDAyOTQpIj4KICAgICAgICA8cGF0aCBkPSJNLTQyNi45LDE2OS44YzAsNDguNy0zLjcsNjQuNy0xMy42LDc2LjRjLTEwLjgsMTAtMjUsMTUuNS0zOS43LDE1LjVsMy43LDI5IGMyMi44LDAuMyw0NC44LTcuOSw2MS45LTIzLjFjMTcuOC0xOC41LDI0LTQ0LjEsMjQtODMuM1YwSC00Mjd2MTcwLjFMLTQyNi45LDE2OS44TC00MjYuOSwxNjkuOHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMTU1LjA0NTI5NiwgNTYuODM3MTA0KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuNTYyNDUzLCAxLjc5OTg0MikiPgogICAgICAgIDxwYXRoIGQ9Ik0tMzEyLDE0OGMwLDIxLDAsMzkuNSwxLjcsNTUuNGgtMzEuOGwtMi4xLTMzLjNoLTAuOGMtNi43LDExLjYtMTYuNCwyMS4zLTI4LDI3LjkgYy0xMS42LDYuNi0yNC44LDEwLTM4LjIsOS44Yy0zMS40LDAtNjktMTcuNy02OS04OVYwaDM2LjR2MTEyLjdjMCwzOC43LDExLjYsNjQuNyw0NC42LDY0LjdjMTAuMy0wLjIsMjAuNC0zLjUsMjguOS05LjQgYzguNS01LjksMTUuMS0xNC4zLDE4LjktMjMuOWMyLjItNi4xLDMuMy0xMi41LDMuMy0xOC45VjAuMmgzNi40VjE0OEgtMzEyTC0zMTIsMTQ4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgzOTAuMDEzMzIyLCA1My40Nzk2MzgpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS43MDY0NTgsIDAuMjMxNDI1KSI+CiAgICAgICAgPHBhdGggZD0iTS00NzguNiw3MS40YzAtMjYtMC44LTQ3LTEuNy02Ni43aDMyLjdsMS43LDM0LjhoMC44YzcuMS0xMi41LDE3LjUtMjIuOCwzMC4xLTI5LjcgYzEyLjUtNywyNi43LTEwLjMsNDEtOS44YzQ4LjMsMCw4NC43LDQxLjcsODQuNywxMDMuM2MwLDczLjEtNDMuNywxMDkuMi05MSwxMDkuMmMtMTIuMSwwLjUtMjQuMi0yLjItMzUtNy44IGMtMTAuOC01LjYtMTkuOS0xMy45LTI2LjYtMjQuMmgtMC44VjI5MWgtMzZ2LTIyMEwtNDc4LjYsNzEuNEwtNDc4LjYsNzEuNHogTS00NDIuNiwxMjUuNmMwLjEsNS4xLDAuNiwxMC4xLDEuNywxNS4xIGMzLDEyLjMsOS45LDIzLjMsMTkuOCwzMS4xYzkuOSw3LjgsMjIuMSwxMi4xLDM0LjcsMTIuMWMzOC41LDAsNjAuNy0zMS45LDYwLjctNzguNWMwLTQwLjctMjEuMS03NS42LTU5LjUtNzUuNiBjLTEyLjksMC40LTI1LjMsNS4xLTM1LjMsMTMuNGMtOS45LDguMy0xNi45LDE5LjctMTkuNiwzMi40Yy0xLjUsNC45LTIuMywxMC0yLjUsMTUuMVYxMjUuNkwtNDQyLjYsMTI1LjZMLTQ0Mi42LDEyNS42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSg2MDYuNzQwNzI2LCA1Ni44MzcxMDQpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC43NTEyMjYsIDEuOTg5Mjk5KSI+CiAgICAgICAgPHBhdGggZD0iTS00NDAuOCwwbDQzLjcsMTIwLjFjNC41LDEzLjQsOS41LDI5LjQsMTIuOCw0MS43aDAuOGMzLjctMTIuMiw3LjktMjcuNywxMi44LTQyLjQgbDM5LjctMTE5LjJoMzguNUwtMzQ2LjksMTQ1Yy0yNiw2OS43LTQzLjcsMTA1LjQtNjguNiwxMjcuMmMtMTIuNSwxMS43LTI3LjksMjAtNDQuNiwyMy45bC05LjEtMzEuMSBjMTEuNy0zLjksMjIuNS0xMC4xLDMxLjgtMTguMWMxMy4yLTExLjEsMjMuNy0yNS4yLDMwLjYtNDEuMmMxLjUtMi44LDIuNS01LjcsMi45LTguOGMtMC4zLTMuMy0xLjItNi42LTIuNS05LjdMLTQ4MC4yLDAuMSBoMzkuN0wtNDQwLjgsMEwtNDQwLjgsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoODIyLjc0ODEwNCwgMC4wMDAwMDApIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS40NjQwNTAsIDAuMzc4OTE0KSI+CiAgICAgICAgPHBhdGggZD0iTS00MTMuNywwdjU4LjNoNTJ2MjguMmgtNTJWMTk2YzAsMjUsNywzOS41LDI3LjMsMzkuNWM3LjEsMC4xLDE0LjItMC43LDIxLjEtMi41IGwxLjcsMjcuN2MtMTAuMywzLjctMjEuMyw1LjQtMzIuMiw1Yy03LjMsMC40LTE0LjYtMC43LTIxLjMtMy40Yy02LjgtMi43LTEyLjktNi44LTE3LjktMTIuMWMtMTAuMy0xMC45LTE0LjEtMjktMTQuMS01Mi45IFY4Ni41aC0zMVY1OC4zaDMxVjkuNkwtNDEzLjcsMEwtNDEzLjcsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOTc0LjQzMzI4NiwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDAuOTkwMDM0LCAwLjYxMDMzOSkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDQ1LjgsMTEzYzAuOCw1MCwzMi4yLDcwLjYsNjguNiw3MC42YzE5LDAuNiwzNy45LTMsNTUuMy0xMC41bDYuMiwyNi40IGMtMjAuOSw4LjktNDMuNSwxMy4xLTY2LjIsMTIuNmMtNjEuNSwwLTk4LjMtNDEuMi05OC4zLTEwMi41Qy00ODAuMiw0OC4yLTQ0NC43LDAtMzg2LjUsMGM2NS4yLDAsODIuNyw1OC4zLDgyLjcsOTUuNyBjLTAuMSw1LjgtMC41LDExLjUtMS4yLDE3LjJoLTE0MC42SC00NDUuOEwtNDQ1LjgsMTEzeiBNLTMzOS4yLDg2LjZjMC40LTIzLjUtOS41LTYwLjEtNTAuNC02MC4xIGMtMzYuOCwwLTUyLjgsMzQuNC01NS43LDYwLjFILTMzOS4yTC0zMzkuMiw4Ni42TC0zMzkuMiw4Ni42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxMjAxLjk2MTA1OCwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuMTc5NjQwLCAwLjcwNTA2OCkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDc4LjYsNjhjMC0yMy45LTAuNC00NC41LTEuNy02My40aDMxLjhsMS4yLDM5LjloMS43YzkuMS0yNy4zLDMxLTQ0LjUsNTUuMy00NC41IGMzLjUtMC4xLDcsMC40LDEwLjMsMS4ydjM0LjhjLTQuMS0wLjktOC4yLTEuMy0xMi40LTEuMmMtMjUuNiwwLTQzLjcsMTkuNy00OC43LDQ3LjRjLTEsNS43LTEuNiwxMS41LTEuNywxNy4ydjEwOC4zaC0zNlY2OCBMLTQ3OC42LDY4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCBkPSJNMTM1Mi4zLDMyNi4yaDM3VjI4aC0zN1YzMjYuMnogTTE2MDQuOCwzMjYuMmMtMi41LTEzLjktMy40LTMxLjEtMy40LTQ4Ljd2LTc2IGMwLTQwLjctMTUuMS04My4xLTc3LjMtODMuMWMtMjUuNiwwLTUwLDcuMS02Ni44LDE4LjFsOC40LDI0LjRjMTQuMy05LjIsMzQtMTUuMSw1My0xNS4xYzQxLjYsMCw0Ni4yLDMwLjIsNDYuMiw0N3Y0LjIgYy03OC42LTAuNC0xMjIuMywyNi41LTEyMi4zLDc1LjZjMCwyOS40LDIxLDU4LjQsNjIuMiw1OC40YzI5LDAsNTAuOS0xNC4zLDYyLjItMzAuMmgxLjNsMi45LDI1LjZIMTYwNC44eiBNMTU2NS43LDI1Ny43IGMwLDMuOC0wLjgsOC0yLjEsMTEuOGMtNS45LDE3LjItMjIuNywzNC00OS4yLDM0Yy0xOC45LDAtMzQuOS0xMS4zLTM0LjktMzUuM2MwLTM5LjUsNDUuOC00Ni42LDg2LjItNDUuOFYyNTcuN3ogTTE2OTguNSwzMjYuMiBsMS43LTMzLjZoMS4zYzE1LjEsMjYuOSwzOC43LDM4LjIsNjguMSwzOC4yYzQ1LjQsMCw5MS4yLTM2LjEsOTEuMi0xMDguOGMwLjQtNjEuNy0zNS4zLTEwMy43LTg1LjctMTAzLjcgYy0zMi44LDAtNTYuMywxNC43LTY5LjMsMzcuNGgtMC44VjI4aC0zNi42djI0NS43YzAsMTguMS0wLjgsMzguNi0xLjcsNTIuNUgxNjk4LjV6IE0xNzA0LjgsMjA4LjJjMC01LjksMS4zLTEwLjksMi4xLTE1LjEgYzcuNi0yOC4xLDMxLjEtNDUuNCw1Ni4zLTQ1LjRjMzkuNSwwLDYwLjUsMzQuOSw2MC41LDc1LjZjMCw0Ni42LTIzLjEsNzguMS02MS44LDc4LjFjLTI2LjksMC00OC4zLTE3LjYtNTUuNS00My4zIGMtMC44LTQuMi0xLjctOC44LTEuNy0xMy40VjIwOC4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgZmlsbD0iIzYxNjE2MSIgZD0iTTE1IDlIOXY2aDZWOXptLTIgNGgtMnYtMmgydjJ6bTgtMlY5aC0yVjdjMC0xLjEtLjktMi0yLTJoLTJWM2gtMnYyaC0yVjNIOXYySDdjLTEuMSAwLTIgLjktMiAydjJIM3YyaDJ2MkgzdjJoMnYyYzAgMS4xLjkgMiAyIDJoMnYyaDJ2LTJoMnYyaDJ2LTJoMmMxLjEgMCAyLS45IDItMnYtMmgydi0yaC0ydi0yaDJ6bS00IDZIN1Y3aDEwdjEweiIvPgo8L3N2Zz4K);
  --jp-icon-keyboard: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMTdjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY3YzAtMS4xLS45LTItMi0yem0tOSAzaDJ2MmgtMlY4em0wIDNoMnYyaC0ydi0yek04IDhoMnYySDhWOHptMCAzaDJ2Mkg4di0yem0tMSAySDV2LTJoMnYyem0wLTNINVY4aDJ2MnptOSA3SDh2LTJoOHYyem0wLTRoLTJ2LTJoMnYyem0wLTNoLTJWOGgydjJ6bTMgM2gtMnYtMmgydjJ6bTAtM2gtMlY4aDJ2MnoiLz4KPC9zdmc+Cg==);
  --jp-icon-launch: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMzIgMzIiIHdpZHRoPSIzMiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0yNiwyOEg2YTIuMDAyNywyLjAwMjcsMCwwLDEtMi0yVjZBMi4wMDI3LDIuMDAyNywwLDAsMSw2LDRIMTZWNkg2VjI2SDI2VjE2aDJWMjZBMi4wMDI3LDIuMDAyNywwLDAsMSwyNiwyOFoiLz4KICAgIDxwb2x5Z29uIHBvaW50cz0iMjAgMiAyMCA0IDI2LjU4NiA0IDE4IDEyLjU4NiAxOS40MTQgMTQgMjggNS40MTQgMjggMTIgMzAgMTIgMzAgMiAyMCAyIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-launcher: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkgMTlINVY1aDdWM0g1YTIgMiAwIDAwLTIgMnYxNGEyIDIgMCAwMDIgMmgxNGMxLjEgMCAyLS45IDItMnYtN2gtMnY3ek0xNCAzdjJoMy41OWwtOS44MyA5LjgzIDEuNDEgMS40MUwxOSA2LjQxVjEwaDJWM2gtN3oiLz4KPC9zdmc+Cg==);
  --jp-icon-line-form: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGZpbGw9IndoaXRlIiBkPSJNNS44OCA0LjEyTDEzLjc2IDEybC03Ljg4IDcuODhMOCAyMmwxMC0xMEw4IDJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-link: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMuOSAxMmMwLTEuNzEgMS4zOS0zLjEgMy4xLTMuMWg0VjdIN2MtMi43NiAwLTUgMi4yNC01IDVzMi4yNCA1IDUgNWg0di0xLjlIN2MtMS43MSAwLTMuMS0xLjM5LTMuMS0zLjF6TTggMTNoOHYtMkg4djJ6bTktNmgtNHYxLjloNGMxLjcxIDAgMy4xIDEuMzkgMy4xIDMuMXMtMS4zOSAzLjEtMy4xIDMuMWgtNFYxN2g0YzIuNzYgMCA1LTIuMjQgNS01cy0yLjI0LTUtNS01eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xOSA1djE0SDVWNWgxNG0xLjEtMkgzLjljLS41IDAtLjkuNC0uOS45djE2LjJjMCAuNC40LjkuOS45aDE2LjJjLjQgMCAuOS0uNS45LS45VjMuOWMwLS41LS41LS45LS45LS45ek0xMSA3aDZ2MmgtNlY3em0wIDRoNnYyaC02di0yem0wIDRoNnYyaC02ek03IDdoMnYySDd6bTAgNGgydjJIN3ptMCA0aDJ2Mkg3eiIvPgo8L3N2Zz4K);
  --jp-icon-markdown: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjN0IxRkEyIiBkPSJNNSAxNC45aDEybC02LjEgNnptOS40LTYuOGMwLTEuMy0uMS0yLjktLjEtNC41LS40IDEuNC0uOSAyLjktMS4zIDQuM2wtMS4zIDQuM2gtMkw4LjUgNy45Yy0uNC0xLjMtLjctMi45LTEtNC4zLS4xIDEuNi0uMSAzLjItLjIgNC42TDcgMTIuNEg0LjhsLjctMTFoMy4zTDEwIDVjLjQgMS4yLjcgMi43IDEgMy45LjMtMS4yLjctMi42IDEtMy45bDEuMi0zLjdoMy4zbC42IDExaC0yLjRsLS4zLTQuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-move-down: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBkPSJNMTIuNDcxIDcuNTI4OTlDMTIuNzYzMiA3LjIzNjg0IDEyLjc2MzIgNi43NjMxNiAxMi40NzEgNi40NzEwMVY2LjQ3MTAxQzEyLjE3OSA2LjE3OTA1IDExLjcwNTcgNi4xNzg4NCAxMS40MTM1IDYuNDcwNTRMNy43NSAxMC4xMjc1VjEuNzVDNy43NSAxLjMzNTc5IDcuNDE0MjEgMSA3IDFWMUM2LjU4NTc5IDEgNi4yNSAxLjMzNTc5IDYuMjUgMS43NVYxMC4xMjc1TDIuNTk3MjYgNi40NjgyMkMyLjMwMzM4IDYuMTczODEgMS44MjY0MSA2LjE3MzU5IDEuNTMyMjYgNi40Njc3NFY2LjQ2Nzc0QzEuMjM4MyA2Ljc2MTcgMS4yMzgzIDcuMjM4MyAxLjUzMjI2IDcuNTMyMjZMNi4yOTI4OSAxMi4yOTI5QzYuNjgzNDIgMTIuNjgzNCA3LjMxNjU4IDEyLjY4MzQgNy43MDcxMSAxMi4yOTI5TDEyLjQ3MSA3LjUyODk5WiIgZmlsbD0iIzYxNjE2MSIvPgo8L3N2Zz4K);
  --jp-icon-move-up: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBkPSJNMS41Mjg5OSA2LjQ3MTAxQzEuMjM2ODQgNi43NjMxNiAxLjIzNjg0IDcuMjM2ODQgMS41Mjg5OSA3LjUyODk5VjcuNTI4OTlDMS44MjA5NSA3LjgyMDk1IDIuMjk0MjYgNy44MjExNiAyLjU4NjQ5IDcuNTI5NDZMNi4yNSAzLjg3MjVWMTIuMjVDNi4yNSAxMi42NjQyIDYuNTg1NzkgMTMgNyAxM1YxM0M3LjQxNDIxIDEzIDcuNzUgMTIuNjY0MiA3Ljc1IDEyLjI1VjMuODcyNUwxMS40MDI3IDcuNTMxNzhDMTEuNjk2NiA3LjgyNjE5IDEyLjE3MzYgNy44MjY0MSAxMi40Njc3IDcuNTMyMjZWNy41MzIyNkMxMi43NjE3IDcuMjM4MyAxMi43NjE3IDYuNzYxNyAxMi40Njc3IDYuNDY3NzRMNy43MDcxMSAxLjcwNzExQzcuMzE2NTggMS4zMTY1OCA2LjY4MzQyIDEuMzE2NTggNi4yOTI4OSAxLjcwNzExTDEuNTI4OTkgNi40NzEwMVoiIGZpbGw9IiM2MTYxNjEiLz4KPC9zdmc+Cg==);
  --jp-icon-new-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwIDZoLThsLTItMkg0Yy0xLjExIDAtMS45OS44OS0xLjk5IDJMMiAxOGMwIDEuMTEuODkgMiAyIDJoMTZjMS4xMSAwIDItLjg5IDItMlY4YzAtMS4xMS0uODktMi0yLTJ6bS0xIDhoLTN2M2gtMnYtM2gtM3YtMmgzVjloMnYzaDN2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-not-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI1IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDMgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMTkgMTcuMTg0NCAyLjk2OTY4IDE0LjMwMzIgMS44NjA5NCAxMS40NDA5WiIvPgogICAgPHBhdGggY2xhc3M9ImpwLWljb24yIiBzdHJva2U9IiMzMzMzMzMiIHN0cm9rZS13aWR0aD0iMiIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOS4zMTU5MiA5LjMyMDMxKSIgZD0iTTcuMzY4NDIgMEwwIDcuMzY0NzkiLz4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDkuMzE1OTIgMTYuNjgzNikgc2NhbGUoMSAtMSkiIGQ9Ik03LjM2ODQyIDBMMCA3LjM2NDc5Ii8+Cjwvc3ZnPgo=);
  --jp-icon-notebook: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtbm90ZWJvb2staWNvbi1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNFRjZDMDAiPgogICAgPHBhdGggZD0iTTE4LjcgMy4zdjE1LjRIMy4zVjMuM2gxNS40bTEuNS0xLjVIMS44djE4LjNoMTguM2wuMS0xOC4zeiIvPgogICAgPHBhdGggZD0iTTE2LjUgMTYuNWwtNS40LTQuMy01LjYgNC4zdi0xMWgxMXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-numbering: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTQgMTlINlYxOS41SDVWMjAuNUg2VjIxSDRWMjJIN1YxOEg0VjE5Wk01IDEwSDZWNkg0VjdINVYxMFpNNCAxM0g1LjhMNCAxNS4xVjE2SDdWMTVINS4yTDcgMTIuOVYxMkg0VjEzWk05IDdWOUgyM1Y3SDlaTTkgMjFIMjNWMTlIOVYyMVpNOSAxNUgyM1YxM0g5VjE1WiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-offline-bolt: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyIDIuMDJjLTUuNTEgMC05Ljk4IDQuNDctOS45OCA5Ljk4czQuNDcgOS45OCA5Ljk4IDkuOTggOS45OC00LjQ3IDkuOTgtOS45OFMxNy41MSAyLjAyIDEyIDIuMDJ6TTExLjQ4IDIwdi02LjI2SDhMMTMgNHY2LjI2aDMuMzVMMTEuNDggMjB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-palette: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE4IDEzVjIwSDRWNkg5LjAyQzkuMDcgNS4yOSA5LjI0IDQuNjIgOS41IDRINEMyLjkgNCAyIDQuOSAyIDZWMjBDMiAyMS4xIDIuOSAyMiA0IDIySDE4QzE5LjEgMjIgMjAgMjEuMSAyMCAyMFYxNUwxOCAxM1pNMTkuMyA4Ljg5QzE5Ljc0IDguMTkgMjAgNy4zOCAyMCA2LjVDMjAgNC4wMSAxNy45OSAyIDE1LjUgMkMxMy4wMSAyIDExIDQuMDEgMTEgNi41QzExIDguOTkgMTMuMDEgMTEgMTUuNDkgMTFDMTYuMzcgMTEgMTcuMTkgMTAuNzQgMTcuODggMTAuM0wyMSAxMy40MkwyMi40MiAxMkwxOS4zIDguODlaTTE1LjUgOUMxNC4xMiA5IDEzIDcuODggMTMgNi41QzEzIDUuMTIgMTQuMTIgNCAxNS41IDRDMTYuODggNCAxOCA1LjEyIDE4IDYuNUMxOCA3Ljg4IDE2Ljg4IDkgMTUuNSA5WiIvPgogICAgPHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik00IDZIOS4wMTg5NEM5LjAwNjM5IDYuMTY1MDIgOSA2LjMzMTc2IDkgNi41QzkgOC44MTU3NyAxMC4yMTEgMTAuODQ4NyAxMi4wMzQzIDEySDlWMTRIMTZWMTIuOTgxMUMxNi41NzAzIDEyLjkzNzcgMTcuMTIgMTIuODIwNyAxNy42Mzk2IDEyLjYzOTZMMTggMTNWMjBINFY2Wk04IDhINlYxMEg4VjhaTTYgMTJIOFYxNEg2VjEyWk04IDE2SDZWMThIOFYxNlpNOSAxNkgxNlYxOEg5VjE2WiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-paste: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE5IDJoLTQuMThDMTQuNC44NCAxMy4zIDAgMTIgMGMtMS4zIDAtMi40Ljg0LTIuODIgMkg1Yy0xLjEgMC0yIC45LTIgMnYxNmMwIDEuMS45IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjRjMC0xLjEtLjktMi0yLTJ6bS03IDBjLjU1IDAgMSAuNDUgMSAxcy0uNDUgMS0xIDEtMS0uNDUtMS0xIC40NS0xIDEtMXptNyAxOEg1VjRoMnYzaDEwVjRoMnYxNnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-pdf: url(data:image/svg+xml;base64,PHN2ZwogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyMiAyMiIgd2lkdGg9IjE2Ij4KICAgIDxwYXRoIHRyYW5zZm9ybT0icm90YXRlKDQ1KSIgY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI0ZGMkEyQSIKICAgICAgIGQ9Im0gMjIuMzQ0MzY5LC0zLjAxNjM2NDIgaCA1LjYzODYwNCB2IDEuNTc5MjQzMyBoIC0zLjU0OTIyNyB2IDEuNTA4NjkyOTkgaCAzLjMzNzU3NiBWIDEuNjUwODE1NCBoIC0zLjMzNzU3NiB2IDMuNDM1MjYxMyBoIC0yLjA4OTM3NyB6IG0gLTcuMTM2NDQ0LDEuNTc5MjQzMyB2IDQuOTQzOTU0MyBoIDAuNzQ4OTIgcSAxLjI4MDc2MSwwIDEuOTUzNzAzLC0wLjYzNDk1MzUgMC42NzgzNjksLTAuNjM0OTUzNSAwLjY3ODM2OSwtMS44NDUxNjQxIDAsLTEuMjA0NzgzNTUgLTAuNjcyOTQyLC0xLjgzNDMxMDExIC0wLjY3Mjk0MiwtMC42Mjk1MjY1OSAtMS45NTkxMywtMC42Mjk1MjY1OSB6IG0gLTIuMDg5Mzc3LC0xLjU3OTI0MzMgaCAyLjIwMzM0MyBxIDEuODQ1MTY0LDAgMi43NDYwMzksMC4yNjU5MjA3IDAuOTA2MzAxLDAuMjYwNDkzNyAxLjU1MjEwOCwwLjg5MDAyMDMgMC41Njk4MywwLjU0ODEyMjMgMC44NDY2MDUsMS4yNjQ0ODAwNiAwLjI3Njc3NCwwLjcxNjM1NzgxIDAuMjc2Nzc0LDEuNjIyNjU4OTQgMCwwLjkxNzE1NTEgLTAuMjc2Nzc0LDEuNjM4OTM5OSAtMC4yNzY3NzUsMC43MTYzNTc4IC0wLjg0NjYwNSwxLjI2NDQ4IC0wLjY1MTIzNCwwLjYyOTUyNjYgLTEuNTYyOTYyLDAuODk1NDQ3MyAtMC45MTE3MjgsMC4yNjA0OTM3IC0yLjczNTE4NSwwLjI2MDQ5MzcgaCAtMi4yMDMzNDMgeiBtIC04LjE0NTg1NjUsMCBoIDMuNDY3ODIzIHEgMS41NDY2ODE2LDAgMi4zNzE1Nzg1LDAuNjg5MjIzIDAuODMwMzI0LDAuNjgzNzk2MSAwLjgzMDMyNCwxLjk1MzcwMzE0IDAsMS4yNzUzMzM5NyAtMC44MzAzMjQsMS45NjQ1NTcwNiBRIDkuOTg3MTk2MSwyLjI3NDkxNSA4LjQ0MDUxNDUsMi4yNzQ5MTUgSCA3LjA2MjA2ODQgViA1LjA4NjA3NjcgSCA0Ljk3MjY5MTUgWiBtIDIuMDg5Mzc2OSwxLjUxNDExOTkgdiAyLjI2MzAzOTQzIGggMS4xNTU5NDEgcSAwLjYwNzgxODgsMCAwLjkzODg2MjksLTAuMjkzMDU1NDcgMC4zMzEwNDQxLC0wLjI5ODQ4MjQxIDAuMzMxMDQ0MSwtMC44NDExNzc3MiAwLC0wLjU0MjY5NTMxIC0wLjMzMTA0NDEsLTAuODM1NzUwNzQgLTAuMzMxMDQ0MSwtMC4yOTMwNTU1IC0wLjkzODg2MjksLTAuMjkzMDU1NSB6IgovPgo8L3N2Zz4K);
  --jp-icon-python: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iLTEwIC0xMCAxMzEuMTYxMzYxNjk0MzM1OTQgMTMyLjM4ODk5OTkzODk2NDg0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMzA2OTk4IiBkPSJNIDU0LjkxODc4NSw5LjE5Mjc0MjFlLTQgQyA1MC4zMzUxMzIsMC4wMjIyMTcyNyA0NS45NTc4NDYsMC40MTMxMzY5NyA0Mi4xMDYyODUsMS4wOTQ2NjkzIDMwLjc2MDA2OSwzLjA5OTE3MzEgMjguNzAwMDM2LDcuMjk0NzcxNCAyOC43MDAwMzUsMTUuMDMyMTY5IHYgMTAuMjE4NzUgaCAyNi44MTI1IHYgMy40MDYyNSBoIC0yNi44MTI1IC0xMC4wNjI1IGMgLTcuNzkyNDU5LDAgLTE0LjYxNTc1ODgsNC42ODM3MTcgLTE2Ljc0OTk5OTgsMTMuNTkzNzUgLTIuNDYxODE5OTgsMTAuMjEyOTY2IC0yLjU3MTAxNTA4LDE2LjU4NjAyMyAwLDI3LjI1IDEuOTA1OTI4Myw3LjkzNzg1MiA2LjQ1NzU0MzIsMTMuNTkzNzQ4IDE0LjI0OTk5OTgsMTMuNTkzNzUgaCA5LjIxODc1IHYgLTEyLjI1IGMgMCwtOC44NDk5MDIgNy42NTcxNDQsLTE2LjY1NjI0OCAxNi43NSwtMTYuNjU2MjUgaCAyNi43ODEyNSBjIDcuNDU0OTUxLDAgMTMuNDA2MjUzLC02LjEzODE2NCAxMy40MDYyNSwtMTMuNjI1IHYgLTI1LjUzMTI1IGMgMCwtNy4yNjYzMzg2IC02LjEyOTk4LC0xMi43MjQ3NzcxIC0xMy40MDYyNSwtMTMuOTM3NDk5NyBDIDY0LjI4MTU0OCwwLjMyNzk0Mzk3IDU5LjUwMjQzOCwtMC4wMjAzNzkwMyA1NC45MTg3ODUsOS4xOTI3NDIxZS00IFogbSAtMTQuNSw4LjIxODc1MDEyNTc5IGMgMi43Njk1NDcsMCA1LjAzMTI1LDIuMjk4NjQ1NiA1LjAzMTI1LDUuMTI0OTk5NiAtMmUtNiwyLjgxNjMzNiAtMi4yNjE3MDMsNS4wOTM3NSAtNS4wMzEyNSw1LjA5Mzc1IC0yLjc3OTQ3NiwtMWUtNiAtNS4wMzEyNSwtMi4yNzc0MTUgLTUuMDMxMjUsLTUuMDkzNzUgLTEwZS03LC0yLjgyNjM1MyAyLjI1MTc3NCwtNS4xMjQ5OTk2IDUuMDMxMjUsLTUuMTI0OTk5NiB6Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI2ZmZDQzYiIgZD0ibSA4NS42Mzc1MzUsMjguNjU3MTY5IHYgMTEuOTA2MjUgYyAwLDkuMjMwNzU1IC03LjgyNTg5NSwxNi45OTk5OTkgLTE2Ljc1LDE3IGggLTI2Ljc4MTI1IGMgLTcuMzM1ODMzLDAgLTEzLjQwNjI0OSw2LjI3ODQ4MyAtMTMuNDA2MjUsMTMuNjI1IHYgMjUuNTMxMjQ3IGMgMCw3LjI2NjM0NCA2LjMxODU4OCwxMS41NDAzMjQgMTMuNDA2MjUsMTMuNjI1MDA0IDguNDg3MzMxLDIuNDk1NjEgMTYuNjI2MjM3LDIuOTQ2NjMgMjYuNzgxMjUsMCA2Ljc1MDE1NSwtMS45NTQzOSAxMy40MDYyNTMsLTUuODg3NjEgMTMuNDA2MjUsLTEzLjYyNTAwNCBWIDg2LjUwMDkxOSBoIC0yNi43ODEyNSB2IC0zLjQwNjI1IGggMjYuNzgxMjUgMTMuNDA2MjU0IGMgNy43OTI0NjEsMCAxMC42OTYyNTEsLTUuNDM1NDA4IDEzLjQwNjI0MSwtMTMuNTkzNzUgMi43OTkzMywtOC4zOTg4ODYgMi42ODAyMiwtMTYuNDc1Nzc2IDAsLTI3LjI1IC0xLjkyNTc4LC03Ljc1NzQ0MSAtNS42MDM4NywtMTMuNTkzNzUgLTEzLjQwNjI0MSwtMTMuNTkzNzUgeiBtIC0xNS4wNjI1LDY0LjY1NjI1IGMgMi43Nzk0NzgsM2UtNiA1LjAzMTI1LDIuMjc3NDE3IDUuMDMxMjUsNS4wOTM3NDcgLTJlLTYsMi44MjYzNTQgLTIuMjUxNzc1LDUuMTI1MDA0IC01LjAzMTI1LDUuMTI1MDA0IC0yLjc2OTU1LDAgLTUuMDMxMjUsLTIuMjk4NjUgLTUuMDMxMjUsLTUuMTI1MDA0IDJlLTYsLTIuODE2MzMgMi4yNjE2OTcsLTUuMDkzNzQ3IDUuMDMxMjUsLTUuMDkzNzQ3IHoiLz4KPC9zdmc+Cg==);
  --jp-icon-r-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjE5NkYzIiBkPSJNNC40IDIuNWMxLjItLjEgMi45LS4zIDQuOS0uMyAyLjUgMCA0LjEuNCA1LjIgMS4zIDEgLjcgMS41IDEuOSAxLjUgMy41IDAgMi0xLjQgMy41LTIuOSA0LjEgMS4yLjQgMS43IDEuNiAyLjIgMyAuNiAxLjkgMSAzLjkgMS4zIDQuNmgtMy44Yy0uMy0uNC0uOC0xLjctMS4yLTMuN3MtMS4yLTIuNi0yLjYtMi42aC0uOXY2LjRINC40VjIuNXptMy43IDYuOWgxLjRjMS45IDAgMi45LS45IDIuOS0yLjNzLTEtMi4zLTIuOC0yLjNjLS43IDAtMS4zIDAtMS42LjJ2NC41aC4xdi0uMXoiLz4KPC9zdmc+Cg==);
  --jp-icon-react: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMTUwIDE1MCA1NDEuOSAyOTUuMyI+CiAgPGcgY2xhc3M9ImpwLWljb24tYnJhbmQyIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzYxREFGQiI+CiAgICA8cGF0aCBkPSJNNjY2LjMgMjk2LjVjMC0zMi41LTQwLjctNjMuMy0xMDMuMS04Mi40IDE0LjQtNjMuNiA4LTExNC4yLTIwLjItMTMwLjQtNi41LTMuOC0xNC4xLTUuNi0yMi40LTUuNnYyMi4zYzQuNiAwIDguMy45IDExLjQgMi42IDEzLjYgNy44IDE5LjUgMzcuNSAxNC45IDc1LjctMS4xIDkuNC0yLjkgMTkuMy01LjEgMjkuNC0xOS42LTQuOC00MS04LjUtNjMuNS0xMC45LTEzLjUtMTguNS0yNy41LTM1LjMtNDEuNi01MCAzMi42LTMwLjMgNjMuMi00Ni45IDg0LTQ2LjlWNzhjLTI3LjUgMC02My41IDE5LjYtOTkuOSA1My42LTM2LjQtMzMuOC03Mi40LTUzLjItOTkuOS01My4ydjIyLjNjMjAuNyAwIDUxLjQgMTYuNSA4NCA0Ni42LTE0IDE0LjctMjggMzEuNC00MS4zIDQ5LjktMjIuNiAyLjQtNDQgNi4xLTYzLjYgMTEtMi4zLTEwLTQtMTkuNy01LjItMjktNC43LTM4LjIgMS4xLTY3LjkgMTQuNi03NS44IDMtMS44IDYuOS0yLjYgMTEuNS0yLjZWNzguNWMtOC40IDAtMTYgMS44LTIyLjYgNS42LTI4LjEgMTYuMi0zNC40IDY2LjctMTkuOSAxMzAuMS02Mi4yIDE5LjItMTAyLjcgNDkuOS0xMDIuNyA4Mi4zIDAgMzIuNSA0MC43IDYzLjMgMTAzLjEgODIuNC0xNC40IDYzLjYtOCAxMTQuMiAyMC4yIDEzMC40IDYuNSAzLjggMTQuMSA1LjYgMjIuNSA1LjYgMjcuNSAwIDYzLjUtMTkuNiA5OS45LTUzLjYgMzYuNCAzMy44IDcyLjQgNTMuMiA5OS45IDUzLjIgOC40IDAgMTYtMS44IDIyLjYtNS42IDI4LjEtMTYuMiAzNC40LTY2LjcgMTkuOS0xMzAuMSA2Mi0xOS4xIDEwMi41LTQ5LjkgMTAyLjUtODIuM3ptLTEzMC4yLTY2LjdjLTMuNyAxMi45LTguMyAyNi4yLTEzLjUgMzkuNS00LjEtOC04LjQtMTYtMTMuMS0yNC00LjYtOC05LjUtMTUuOC0xNC40LTIzLjQgMTQuMiAyLjEgMjcuOSA0LjcgNDEgNy45em0tNDUuOCAxMDYuNWMtNy44IDEzLjUtMTUuOCAyNi4zLTI0LjEgMzguMi0xNC45IDEuMy0zMCAyLTQ1LjIgMi0xNS4xIDAtMzAuMi0uNy00NS0xLjktOC4zLTExLjktMTYuNC0yNC42LTI0LjItMzgtNy42LTEzLjEtMTQuNS0yNi40LTIwLjgtMzkuOCA2LjItMTMuNCAxMy4yLTI2LjggMjAuNy0zOS45IDcuOC0xMy41IDE1LjgtMjYuMyAyNC4xLTM4LjIgMTQuOS0xLjMgMzAtMiA0NS4yLTIgMTUuMSAwIDMwLjIuNyA0NSAxLjkgOC4zIDExLjkgMTYuNCAyNC42IDI0LjIgMzggNy42IDEzLjEgMTQuNSAyNi40IDIwLjggMzkuOC02LjMgMTMuNC0xMy4yIDI2LjgtMjAuNyAzOS45em0zMi4zLTEzYzUuNCAxMy40IDEwIDI2LjggMTMuOCAzOS44LTEzLjEgMy4yLTI2LjkgNS45LTQxLjIgOCA0LjktNy43IDkuOC0xNS42IDE0LjQtMjMuNyA0LjYtOCA4LjktMTYuMSAxMy0yNC4xek00MjEuMiA0MzBjLTkuMy05LjYtMTguNi0yMC4zLTI3LjgtMzIgOSAuNCAxOC4yLjcgMjcuNS43IDkuNCAwIDE4LjctLjIgMjcuOC0uNy05IDExLjctMTguMyAyMi40LTI3LjUgMzJ6bS03NC40LTU4LjljLTE0LjItMi4xLTI3LjktNC43LTQxLTcuOSAzLjctMTIuOSA4LjMtMjYuMiAxMy41LTM5LjUgNC4xIDggOC40IDE2IDEzLjEgMjQgNC43IDggOS41IDE1LjggMTQuNCAyMy40ek00MjAuNyAxNjNjOS4zIDkuNiAxOC42IDIwLjMgMjcuOCAzMi05LS40LTE4LjItLjctMjcuNS0uNy05LjQgMC0xOC43LjItMjcuOC43IDktMTEuNyAxOC4zLTIyLjQgMjcuNS0zMnptLTc0IDU4LjljLTQuOSA3LjctOS44IDE1LjYtMTQuNCAyMy43LTQuNiA4LTguOSAxNi0xMyAyNC01LjQtMTMuNC0xMC0yNi44LTEzLjgtMzkuOCAxMy4xLTMuMSAyNi45LTUuOCA0MS4yLTcuOXptLTkwLjUgMTI1LjJjLTM1LjQtMTUuMS01OC4zLTM0LjktNTguMy01MC42IDAtMTUuNyAyMi45LTM1LjYgNTguMy01MC42IDguNi0zLjcgMTgtNyAyNy43LTEwLjEgNS43IDE5LjYgMTMuMiA0MCAyMi41IDYwLjktOS4yIDIwLjgtMTYuNiA0MS4xLTIyLjIgNjAuNi05LjktMy4xLTE5LjMtNi41LTI4LTEwLjJ6TTMxMCA0OTBjLTEzLjYtNy44LTE5LjUtMzcuNS0xNC45LTc1LjcgMS4xLTkuNCAyLjktMTkuMyA1LjEtMjkuNCAxOS42IDQuOCA0MSA4LjUgNjMuNSAxMC45IDEzLjUgMTguNSAyNy41IDM1LjMgNDEuNiA1MC0zMi42IDMwLjMtNjMuMiA0Ni45LTg0IDQ2LjktNC41LS4xLTguMy0xLTExLjMtMi43em0yMzcuMi03Ni4yYzQuNyAzOC4yLTEuMSA2Ny45LTE0LjYgNzUuOC0zIDEuOC02LjkgMi42LTExLjUgMi42LTIwLjcgMC01MS40LTE2LjUtODQtNDYuNiAxNC0xNC43IDI4LTMxLjQgNDEuMy00OS45IDIyLjYtMi40IDQ0LTYuMSA2My42LTExIDIuMyAxMC4xIDQuMSAxOS44IDUuMiAyOS4xem0zOC41LTY2LjdjLTguNiAzLjctMTggNy0yNy43IDEwLjEtNS43LTE5LjYtMTMuMi00MC0yMi41LTYwLjkgOS4yLTIwLjggMTYuNi00MS4xIDIyLjItNjAuNiA5LjkgMy4xIDE5LjMgNi41IDI4LjEgMTAuMiAzNS40IDE1LjEgNTguMyAzNC45IDU4LjMgNTAuNi0uMSAxNS43LTIzIDM1LjYtNTguNCA1MC42ek0zMjAuOCA3OC40eiIvPgogICAgPGNpcmNsZSBjeD0iNDIwLjkiIGN5PSIyOTYuNSIgcj0iNDUuNyIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-redo: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgICA8cGF0aCBkPSJNMCAwaDI0djI0SDB6IiBmaWxsPSJub25lIi8+PHBhdGggZD0iTTE4LjQgMTAuNkMxNi41NSA4Ljk5IDE0LjE1IDggMTEuNSA4Yy00LjY1IDAtOC41OCAzLjAzLTkuOTYgNy4yMkwzLjkgMTZjMS4wNS0zLjE5IDQuMDUtNS41IDcuNi01LjUgMS45NSAwIDMuNzMuNzIgNS4xMiAxLjg4TDEzIDE2aDlWN2wtMy42IDMuNnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-refresh: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTkgMTMuNWMtMi40OSAwLTQuNS0yLjAxLTQuNS00LjVTNi41MSA0LjUgOSA0LjVjMS4yNCAwIDIuMzYuNTIgMy4xNyAxLjMzTDEwIDhoNVYzbC0xLjc2IDEuNzZDMTIuMTUgMy42OCAxMC42NiAzIDkgMyA1LjY5IDMgMy4wMSA1LjY5IDMuMDEgOVM1LjY5IDE1IDkgMTVjMi45NyAwIDUuNDMtMi4xNiA1LjktNWgtMS41MmMtLjQ2IDItMi4yNCAzLjUtNC4zOCAzLjV6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-regex: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0MTQxNDEiPgogICAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi1hY2NlbnQyIiBmaWxsPSIjRkZGIj4KICAgIDxjaXJjbGUgY2xhc3M9InN0MiIgY3g9IjUuNSIgY3k9IjE0LjUiIHI9IjEuNSIvPgogICAgPHJlY3QgeD0iMTIiIHk9IjQiIGNsYXNzPSJzdDIiIHdpZHRoPSIxIiBoZWlnaHQ9IjgiLz4KICAgIDxyZWN0IHg9IjguNSIgeT0iNy41IiB0cmFuc2Zvcm09Im1hdHJpeCgwLjg2NiAtMC41IDAuNSAwLjg2NiAtMi4zMjU1IDcuMzIxOSkiIGNsYXNzPSJzdDIiIHdpZHRoPSI4IiBoZWlnaHQ9IjEiLz4KICAgIDxyZWN0IHg9IjEyIiB5PSI0IiB0cmFuc2Zvcm09Im1hdHJpeCgwLjUgLTAuODY2IDAuODY2IDAuNSAtMC42Nzc5IDE0LjgyNTIpIiBjbGFzcz0ic3QyIiB3aWR0aD0iMSIgaGVpZ2h0PSI4Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-run: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTggNXYxNGwxMS03eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-running: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICA8cGF0aCBkPSJNMjU2IDhDMTE5IDggOCAxMTkgOCAyNTZzMTExIDI0OCAyNDggMjQ4IDI0OC0xMTEgMjQ4LTI0OFMzOTMgOCAyNTYgOHptOTYgMzI4YzAgOC44LTcuMiAxNi0xNiAxNkgxNzZjLTguOCAwLTE2LTcuMi0xNi0xNlYxNzZjMC04LjggNy4yLTE2IDE2LTE2aDE2MGM4LjggMCAxNiA3LjIgMTYgMTZ2MTYweiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-save: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE3IDNINWMtMS4xMSAwLTIgLjktMiAydjE0YzAgMS4xLjg5IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjdsLTQtNHptLTUgMTZjLTEuNjYgMC0zLTEuMzQtMy0zczEuMzQtMyAzLTMgMyAxLjM0IDMgMy0xLjM0IDMtMyAzem0zLTEwSDVWNWgxMHY0eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-search: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjEsMTAuOWgtMC43bC0wLjItMC4yYzAuOC0wLjksMS4zLTIuMiwxLjMtMy41YzAtMy0yLjQtNS40LTUuNC01LjRTMS44LDQuMiwxLjgsNy4xczIuNCw1LjQsNS40LDUuNCBjMS4zLDAsMi41LTAuNSwzLjUtMS4zbDAuMiwwLjJ2MC43bDQuMSw0LjFsMS4yLTEuMkwxMi4xLDEwLjl6IE03LjEsMTAuOWMtMi4xLDAtMy43LTEuNy0zLjctMy43czEuNy0zLjcsMy43LTMuN3MzLjcsMS43LDMuNywzLjcgUzkuMiwxMC45LDcuMSwxMC45eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-settings: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuNDMgMTIuOThjLjA0LS4zMi4wNy0uNjQuMDctLjk4cy0uMDMtLjY2LS4wNy0uOThsMi4xMS0xLjY1Yy4xOS0uMTUuMjQtLjQyLjEyLS42NGwtMi0zLjQ2Yy0uMTItLjIyLS4zOS0uMy0uNjEtLjIybC0yLjQ5IDFjLS41Mi0uNC0xLjA4LS43My0xLjY5LS45OGwtLjM4LTIuNjVBLjQ4OC40ODggMCAwMDE0IDJoLTRjLS4yNSAwLS40Ni4xOC0uNDkuNDJsLS4zOCAyLjY1Yy0uNjEuMjUtMS4xNy41OS0xLjY5Ljk4bC0yLjQ5LTFjLS4yMy0uMDktLjQ5IDAtLjYxLjIybC0yIDMuNDZjLS4xMy4yMi0uMDcuNDkuMTIuNjRsMi4xMSAxLjY1Yy0uMDQuMzItLjA3LjY1LS4wNy45OHMuMDMuNjYuMDcuOThsLTIuMTEgMS42NWMtLjE5LjE1LS4yNC40Mi0uMTIuNjRsMiAzLjQ2Yy4xMi4yMi4zOS4zLjYxLjIybDIuNDktMWMuNTIuNCAxLjA4LjczIDEuNjkuOThsLjM4IDIuNjVjLjAzLjI0LjI0LjQyLjQ5LjQyaDRjLjI1IDAgLjQ2LS4xOC40OS0uNDJsLjM4LTIuNjVjLjYxLS4yNSAxLjE3LS41OSAxLjY5LS45OGwyLjQ5IDFjLjIzLjA5LjQ5IDAgLjYxLS4yMmwyLTMuNDZjLjEyLS4yMi4wNy0uNDktLjEyLS42NGwtMi4xMS0xLjY1ek0xMiAxNS41Yy0xLjkzIDAtMy41LTEuNTctMy41LTMuNXMxLjU3LTMuNSAzLjUtMy41IDMuNSAxLjU3IDMuNSAzLjUtMS41NyAzLjUtMy41IDMuNXoiLz4KPC9zdmc+Cg==);
  --jp-icon-share: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTSAxOCAyIEMgMTYuMzU0OTkgMiAxNSAzLjM1NDk5MDQgMTUgNSBDIDE1IDUuMTkwOTUyOSAxNS4wMjE3OTEgNS4zNzcxMjI0IDE1LjA1NjY0MSA1LjU1ODU5MzggTCA3LjkyMTg3NSA5LjcyMDcwMzEgQyA3LjM5ODUzOTkgOS4yNzc4NTM5IDYuNzMyMDc3MSA5IDYgOSBDIDQuMzU0OTkwNCA5IDMgMTAuMzU0OTkgMyAxMiBDIDMgMTMuNjQ1MDEgNC4zNTQ5OTA0IDE1IDYgMTUgQyA2LjczMjA3NzEgMTUgNy4zOTg1Mzk5IDE0LjcyMjE0NiA3LjkyMTg3NSAxNC4yNzkyOTcgTCAxNS4wNTY2NDEgMTguNDM5NDUzIEMgMTUuMDIxNTU1IDE4LjYyMTUxNCAxNSAxOC44MDgzODYgMTUgMTkgQyAxNSAyMC42NDUwMSAxNi4zNTQ5OSAyMiAxOCAyMiBDIDE5LjY0NTAxIDIyIDIxIDIwLjY0NTAxIDIxIDE5IEMgMjEgMTcuMzU0OTkgMTkuNjQ1MDEgMTYgMTggMTYgQyAxNy4yNjc0OCAxNiAxNi42MDE1OTMgMTYuMjc5MzI4IDE2LjA3ODEyNSAxNi43MjI2NTYgTCA4Ljk0MzM1OTQgMTIuNTU4NTk0IEMgOC45NzgyMDk1IDEyLjM3NzEyMiA5IDEyLjE5MDk1MyA5IDEyIEMgOSAxMS44MDkwNDcgOC45NzgyMDk1IDExLjYyMjg3OCA4Ljk0MzM1OTQgMTEuNDQxNDA2IEwgMTYuMDc4MTI1IDcuMjc5Mjk2OSBDIDE2LjYwMTQ2IDcuNzIyMTQ2MSAxNy4yNjc5MjMgOCAxOCA4IEMgMTkuNjQ1MDEgOCAyMSA2LjY0NTAwOTYgMjEgNSBDIDIxIDMuMzU0OTkwNCAxOS42NDUwMSAyIDE4IDIgeiBNIDE4IDQgQyAxOC41NjQxMjkgNCAxOSA0LjQzNTg3MDYgMTkgNSBDIDE5IDUuNTY0MTI5NCAxOC41NjQxMjkgNiAxOCA2IEMgMTcuNDM1ODcxIDYgMTcgNS41NjQxMjk0IDE3IDUgQyAxNyA0LjQzNTg3MDYgMTcuNDM1ODcxIDQgMTggNCB6IE0gNiAxMSBDIDYuNTY0MTI5NCAxMSA3IDExLjQzNTg3MSA3IDEyIEMgNyAxMi41NjQxMjkgNi41NjQxMjk0IDEzIDYgMTMgQyA1LjQzNTg3MDYgMTMgNSAxMi41NjQxMjkgNSAxMiBDIDUgMTEuNDM1ODcxIDUuNDM1ODcwNiAxMSA2IDExIHogTSAxOCAxOCBDIDE4LjU2NDEyOSAxOCAxOSAxOC40MzU4NzEgMTkgMTkgQyAxOSAxOS41NjQxMjkgMTguNTY0MTI5IDIwIDE4IDIwIEMgMTcuNDM1ODcxIDIwIDE3IDE5LjU2NDEyOSAxNyAxOSBDIDE3IDE4LjQzNTg3MSAxNy40MzU4NzEgMTggMTggMTggeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-spreadsheet: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNENBRjUwIiBkPSJNMi4yIDIuMnYxNy42aDE3LjZWMi4ySDIuMnptMTUuNCA3LjdoLTUuNVY0LjRoNS41djUuNXpNOS45IDQuNHY1LjVINC40VjQuNGg1LjV6bS01LjUgNy43aDUuNXY1LjVINC40di01LjV6bTcuNyA1LjV2LTUuNWg1LjV2NS41aC01LjV6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-stop: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik02IDZoMTJ2MTJINnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-tab: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIxIDNIM2MtMS4xIDAtMiAuOS0yIDJ2MTRjMCAxLjEuOSAyIDIgMmgxOGMxLjEgMCAyLS45IDItMlY1YzAtMS4xLS45LTItMi0yem0wIDE2SDNWNWgxMHY0aDh2MTB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-table-rows: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMSw4SDNWNGgxOFY4eiBNMjEsMTBIM3Y0aDE4VjEweiBNMjEsMTZIM3Y0aDE4VjE2eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-tag: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjgiIGhlaWdodD0iMjgiIHZpZXdCb3g9IjAgMCA0MyAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTI4LjgzMzIgMTIuMzM0TDMyLjk5OTggMTYuNTAwN0wzNy4xNjY1IDEyLjMzNEgyOC44MzMyWiIvPgoJCTxwYXRoIGQ9Ik0xNi4yMDk1IDIxLjYxMDRDMTUuNjg3MyAyMi4xMjk5IDE0Ljg0NDMgMjIuMTI5OSAxNC4zMjQ4IDIxLjYxMDRMNi45ODI5IDE0LjcyNDVDNi41NzI0IDE0LjMzOTQgNi4wODMxMyAxMy42MDk4IDYuMDQ3ODYgMTMuMDQ4MkM1Ljk1MzQ3IDExLjUyODggNi4wMjAwMiA4LjYxOTQ0IDYuMDY2MjEgNy4wNzY5NUM2LjA4MjgxIDYuNTE0NzcgNi41NTU0OCA2LjA0MzQ3IDcuMTE4MDQgNi4wMzA1NUM5LjA4ODYzIDUuOTg0NzMgMTMuMjYzOCA1LjkzNTc5IDEzLjY1MTggNi4zMjQyNUwyMS43MzY5IDEzLjYzOUMyMi4yNTYgMTQuMTU4NSAyMS43ODUxIDE1LjQ3MjQgMjEuMjYyIDE1Ljk5NDZMMTYuMjA5NSAyMS42MTA0Wk05Ljc3NTg1IDguMjY1QzkuMzM1NTEgNy44MjU2NiA4LjYyMzUxIDcuODI1NjYgOC4xODI4IDguMjY1QzcuNzQzNDYgOC43MDU3MSA3Ljc0MzQ2IDkuNDE3MzMgOC4xODI4IDkuODU2NjdDOC42MjM4MiAxMC4yOTY0IDkuMzM1ODIgMTAuMjk2NCA5Ljc3NTg1IDkuODU2NjdDMTAuMjE1NiA5LjQxNzMzIDEwLjIxNTYgOC43MDUzMyA5Ljc3NTg1IDguMjY1WiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-terminal: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0IiA+CiAgICA8cmVjdCBjbGFzcz0ianAtdGVybWluYWwtaWNvbi1iYWNrZ3JvdW5kLWNvbG9yIGpwLWljb24tc2VsZWN0YWJsZSIgd2lkdGg9IjIwIiBoZWlnaHQ9IjIwIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgyIDIpIiBmaWxsPSIjMzMzMzMzIi8+CiAgICA8cGF0aCBjbGFzcz0ianAtdGVybWluYWwtaWNvbi1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUtaW52ZXJzZSIgZD0iTTUuMDU2NjQgOC43NjE3MkM1LjA1NjY0IDguNTk3NjYgNS4wMzEyNSA4LjQ1MzEyIDQuOTgwNDcgOC4zMjgxMkM0LjkzMzU5IDguMTk5MjIgNC44NTU0NyA4LjA4MjAzIDQuNzQ2MDkgNy45NzY1NkM0LjY0MDYyIDcuODcxMDkgNC41IDcuNzc1MzkgNC4zMjQyMiA3LjY4OTQ1QzQuMTUyMzQgNy41OTk2MSAzLjk0MzM2IDcuNTExNzIgMy42OTcyNyA3LjQyNTc4QzMuMzAyNzMgNy4yODUxNiAyLjk0MzM2IDcuMTM2NzIgMi42MTkxNCA2Ljk4MDQ3QzIuMjk0OTIgNi44MjQyMiAyLjAxNzU4IDYuNjQyNTggMS43ODcxMSA2LjQzNTU1QzEuNTYwNTUgNi4yMjg1MiAxLjM4NDc3IDUuOTg4MjggMS4yNTk3NyA1LjcxNDg0QzEuMTM0NzcgNS40Mzc1IDEuMDcyMjcgNS4xMDkzOCAxLjA3MjI3IDQuNzMwNDdDMS4wNzIyNyA0LjM5ODQ0IDEuMTI4OTEgNC4wOTU3IDEuMjQyMTkgMy44MjIyN0MxLjM1NTQ3IDMuNTQ0OTIgMS41MTU2MiAzLjMwNDY5IDEuNzIyNjYgMy4xMDE1NkMxLjkyOTY5IDIuODk4NDQgMi4xNzk2OSAyLjczNDM3IDIuNDcyNjYgMi42MDkzOEMyLjc2NTYyIDIuNDg0MzggMy4wOTE4IDIuNDA0MyAzLjQ1MTE3IDIuMzY5MTRWMS4xMDkzOEg0LjM4ODY3VjIuMzgwODZDNC43NDAyMyAyLjQyNzczIDUuMDU2NjQgMi41MjM0NCA1LjMzNzg5IDIuNjY3OTdDNS42MTkxNCAyLjgxMjUgNS44NTc0MiAzLjAwMTk1IDYuMDUyNzMgMy4yMzYzM0M2LjI1MTk1IDMuNDY2OCA2LjQwNDMgMy43NDAyMyA2LjUwOTc3IDQuMDU2NjRDNi42MTkxNCA0LjM2OTE0IDYuNjczODMgNC43MjA3IDYuNjczODMgNS4xMTEzM0g1LjA0NDkyQzUuMDQ0OTIgNC42Mzg2NyA0LjkzNzUgNC4yODEyNSA0LjcyMjY2IDQuMDM5MDZDNC41MDc4MSAzLjc5Mjk3IDQuMjE2OCAzLjY2OTkyIDMuODQ5NjEgMy42Njk5MkMzLjY1MDM5IDMuNjY5OTIgMy40NzY1NiAzLjY5NzI3IDMuMzI4MTIgMy43NTE5NUMzLjE4MzU5IDMuODAyNzMgMy4wNjQ0NSAzLjg3Njk1IDIuOTcwNyAzLjk3NDYxQzIuODc2OTUgNC4wNjgzNiAyLjgwNjY0IDQuMTc5NjkgMi43NTk3NyA0LjMwODU5QzIuNzE2OCA0LjQzNzUgMi42OTUzMSA0LjU3ODEyIDIuNjk1MzEgNC43MzA0N0MyLjY5NTMxIDQuODgyODEgMi43MTY4IDUuMDE5NTMgMi43NTk3NyA1LjE0MDYyQzIuODA2NjQgNS4yNTc4MSAyLjg4MjgxIDUuMzY3MTkgMi45ODgyOCA1LjQ2ODc1QzMuMDk3NjYgNS41NzAzMSAzLjI0MDIzIDUuNjY3OTcgMy40MTYwMiA1Ljc2MTcyQzMuNTkxOCA1Ljg1MTU2IDMuODEwNTUgNS45NDMzNiA0LjA3MjI3IDYuMDM3MTFDNC40NjY4IDYuMTg1NTUgNC44MjQyMiA2LjMzOTg0IDUuMTQ0NTMgNi41QzUuNDY0ODQgNi42NTYyNSA1LjczODI4IDYuODM5ODQgNS45NjQ4NCA3LjA1MDc4QzYuMTk1MzEgNy4yNTc4MSA2LjM3MTA5IDcuNSA2LjQ5MjE5IDcuNzc3MzRDNi42MTcxOSA4LjA1MDc4IDYuNjc5NjkgOC4zNzUgNi42Nzk2OSA4Ljc1QzYuNjc5NjkgOS4wOTM3NSA2LjYyMzA1IDkuNDA0MyA2LjUwOTc3IDkuNjgxNjRDNi4zOTY0OCA5Ljk1NTA4IDYuMjM0MzggMTAuMTkxNCA2LjAyMzQ0IDEwLjM5MDZDNS44MTI1IDEwLjU4OTggNS41NTg1OSAxMC43NSA1LjI2MTcyIDEwLjg3MTFDNC45NjQ4NCAxMC45ODgzIDQuNjMyODEgMTEuMDY0NSA0LjI2NTYyIDExLjA5OTZWMTIuMjQ4SDMuMzMzOThWMTEuMDk5NkMzLjAwMTk1IDExLjA2ODQgMi42Nzk2OSAxMC45OTYxIDIuMzY3MTkgMTAuODgyOEMyLjA1NDY5IDEwLjc2NTYgMS43NzczNCAxMC41OTc3IDEuNTM1MTYgMTAuMzc4OUMxLjI5Njg4IDEwLjE2MDIgMS4xMDU0NyA5Ljg4NDc3IDAuOTYwOTM4IDkuNTUyNzNDMC44MTY0MDYgOS4yMTY4IDAuNzQ0MTQxIDguODE0NDUgMC43NDQxNDEgOC4zNDU3SDIuMzc4OTFDMi4zNzg5MSA4LjYyNjk1IDIuNDE5OTIgOC44NjMyOCAyLjUwMTk1IDkuMDU0NjlDMi41ODM5OCA5LjI0MjE5IDIuNjg5NDUgOS4zOTI1OCAyLjgxODM2IDkuNTA1ODZDMi45NTExNyA5LjYxNTIzIDMuMTAxNTYgOS42OTMzNiAzLjI2OTUzIDkuNzQwMjNDMy40Mzc1IDkuNzg3MTEgMy42MDkzOCA5LjgxMDU1IDMuNzg1MTYgOS44MTA1NUM0LjIwMzEyIDkuODEwNTUgNC41MTk1MyA5LjcxMjg5IDQuNzM0MzggOS41MTc1OEM0Ljk0OTIyIDkuMzIyMjcgNS4wNTY2NCA5LjA3MDMxIDUuMDU2NjQgOC43NjE3MlpNMTMuNDE4IDEyLjI3MTVIOC4wNzQyMlYxMUgxMy40MThWMTIuMjcxNVoiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDMuOTUyNjQgNikiIGZpbGw9IndoaXRlIi8+Cjwvc3ZnPgo=);
  --jp-icon-text-editor: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtdGV4dC1lZGl0b3ItaWNvbi1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xNSAxNUgzdjJoMTJ2LTJ6bTAtOEgzdjJoMTJWN3pNMyAxM2gxOHYtMkgzdjJ6bTAgOGgxOHYtMkgzdjJ6TTMgM3YyaDE4VjNIM3oiLz4KPC9zdmc+Cg==);
  --jp-icon-toc: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik03LDVIMjFWN0g3VjVNNywxM1YxMUgyMVYxM0g3TTQsNC41QTEuNSwxLjUgMCAwLDEgNS41LDZBMS41LDEuNSAwIDAsMSA0LDcuNUExLjUsMS41IDAgMCwxIDIuNSw2QTEuNSwxLjUgMCAwLDEgNCw0LjVNNCwxMC41QTEuNSwxLjUgMCAwLDEgNS41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMy41QTEuNSwxLjUgMCAwLDEgMi41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMC41TTcsMTlWMTdIMjFWMTlIN000LDE2LjVBMS41LDEuNSAwIDAsMSA1LjUsMThBMS41LDEuNSAwIDAsMSA0LDE5LjVBMS41LDEuNSAwIDAsMSAyLjUsMThBMS41LDEuNSAwIDAsMSA0LDE2LjVaIiAvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-tree-view: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMiAxMVYzaC03djNIOVYzSDJ2OGg3VjhoMnYxMGg0djNoN3YtOGgtN3YzaC0yVjhoMnYzeiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMiAxNy4xODQ0IDIuOTY5NjggMTQuMzAzMiAxLjg2MDk0IDExLjQ0MDlaIi8+CiAgICA8cGF0aCBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiMzMzMzMzMiIHN0cm9rZT0iIzMzMzMzMyIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOCA5Ljg2NzE5KSIgZD0iTTIuODYwMTUgNC44NjUzNUwwLjcyNjU0OSAyLjk5OTU5TDAgMy42MzA0NUwyLjg2MDE1IDYuMTMxNTdMOCAwLjYzMDg3Mkw3LjI3ODU3IDBMMi44NjAxNSA0Ljg2NTM1WiIvPgo8L3N2Zz4K);
  --jp-icon-undo: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjUgOGMtMi42NSAwLTUuMDUuOTktNi45IDIuNkwyIDd2OWg5bC0zLjYyLTMuNjJjMS4zOS0xLjE2IDMuMTYtMS44OCA1LjEyLTEuODggMy41NCAwIDYuNTUgMi4zMSA3LjYgNS41bDIuMzctLjc4QzIxLjA4IDExLjAzIDE3LjE1IDggMTIuNSA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-user: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE2IDdhNCA0IDAgMTEtOCAwIDQgNCAwIDAxOCAwek0xMiAxNGE3IDcgMCAwMC03IDdoMTRhNyA3IDAgMDAtNy03eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-users: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZlcnNpb249IjEuMSIgdmlld0JveD0iMCAwIDM2IDI0IiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogPGcgY2xhc3M9ImpwLWljb24zIiB0cmFuc2Zvcm09Im1hdHJpeCgxLjczMjcgMCAwIDEuNzMyNyAtMy42MjgyIC4wOTk1NzcpIiBmaWxsPSIjNjE2MTYxIj4KICA8cGF0aCB0cmFuc2Zvcm09Im1hdHJpeCgxLjUsMCwwLDEuNSwwLC02KSIgZD0ibTEyLjE4NiA3LjUwOThjLTEuMDUzNSAwLTEuOTc1NyAwLjU2NjUtMi40Nzg1IDEuNDEwMiAwLjc1MDYxIDAuMzEyNzcgMS4zOTc0IDAuODI2NDggMS44NzMgMS40NzI3aDMuNDg2M2MwLTEuNTkyLTEuMjg4OS0yLjg4MjgtMi44ODA5LTIuODgyOHoiLz4KICA8cGF0aCBkPSJtMjAuNDY1IDIuMzg5NWEyLjE4ODUgMi4xODg1IDAgMCAxLTIuMTg4NCAyLjE4ODUgMi4xODg1IDIuMTg4NSAwIDAgMS0yLjE4ODUtMi4xODg1IDIuMTg4NSAyLjE4ODUgMCAwIDEgMi4xODg1LTIuMTg4NSAyLjE4ODUgMi4xODg1IDAgMCAxIDIuMTg4NCAyLjE4ODV6Ii8+CiAgPHBhdGggdHJhbnNmb3JtPSJtYXRyaXgoMS41LDAsMCwxLjUsMCwtNikiIGQ9Im0zLjU4OTggOC40MjE5Yy0xLjExMjYgMC0yLjAxMzcgMC45MDExMS0yLjAxMzcgMi4wMTM3aDIuODE0NWMwLjI2Nzk3LTAuMzczMDkgMC41OTA3LTAuNzA0MzUgMC45NTg5OC0wLjk3ODUyLTAuMzQ0MzMtMC42MTY4OC0xLjAwMzEtMS4wMzUyLTEuNzU5OC0xLjAzNTJ6Ii8+CiAgPHBhdGggZD0ibTYuOTE1NCA0LjYyM2ExLjUyOTQgMS41Mjk0IDAgMCAxLTEuNTI5NCAxLjUyOTQgMS41Mjk0IDEuNTI5NCAwIDAgMS0xLjUyOTQtMS41Mjk0IDEuNTI5NCAxLjUyOTQgMCAwIDEgMS41Mjk0LTEuNTI5NCAxLjUyOTQgMS41Mjk0IDAgMCAxIDEuNTI5NCAxLjUyOTR6Ii8+CiAgPHBhdGggZD0ibTYuMTM1IDEzLjUzNWMwLTMuMjM5MiAyLjYyNTktNS44NjUgNS44NjUtNS44NjUgMy4yMzkyIDAgNS44NjUgMi42MjU5IDUuODY1IDUuODY1eiIvPgogIDxjaXJjbGUgY3g9IjEyIiBjeT0iMy43Njg1IiByPSIyLjk2ODUiLz4KIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-vega: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbjEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjEyMTIxIj4KICAgIDxwYXRoIGQ9Ik0xMC42IDUuNGwyLjItMy4ySDIuMnY3LjNsNC02LjZ6Ii8+CiAgICA8cGF0aCBkPSJNMTUuOCAyLjJsLTQuNCA2LjZMNyA2LjNsLTQuOCA4djUuNWgxNy42VjIuMmgtNHptLTcgMTUuNEg1LjV2LTQuNGgzLjN2NC40em00LjQgMEg5LjhWOS44aDMuNHY3Ljh6bTQuNCAwaC0zLjRWNi41aDMuNHYxMS4xeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-word: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KIDxnIGNsYXNzPSJqcC1pY29uMiIgZmlsbD0iIzQxNDE0MSI+CiAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiA8L2c+CiA8ZyBjbGFzcz0ianAtaWNvbi1hY2NlbnQyIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSguNDMgLjA0MDEpIiBmaWxsPSIjZmZmIj4KICA8cGF0aCBkPSJtNC4xNCA4Ljc2cTAuMDY4Mi0xLjg5IDIuNDItMS44OSAxLjE2IDAgMS42OCAwLjQyIDAuNTY3IDAuNDEgMC41NjcgMS4xNnYzLjQ3cTAgMC40NjIgMC41MTQgMC40NjIgMC4xMDMgMCAwLjItMC4wMjMxdjAuNzE0cS0wLjM5OSAwLjEwMy0wLjY1MSAwLjEwMy0wLjQ1MiAwLTAuNjkzLTAuMjItMC4yMzEtMC4yLTAuMjg0LTAuNjYyLTAuOTU2IDAuODcyLTIgMC44NzItMC45MDMgMC0xLjQ3LTAuNDcyLTAuNTI1LTAuNDcyLTAuNTI1LTEuMjYgMC0wLjI2MiAwLjA0NTItMC40NzIgMC4wNTY3LTAuMjIgMC4xMTYtMC4zNzggMC4wNjgyLTAuMTY4IDAuMjMxLTAuMzA0IDAuMTU4LTAuMTQ3IDAuMjYyLTAuMjQyIDAuMTE2LTAuMDkxNCAwLjM2OC0wLjE2OCAwLjI2Mi0wLjA5MTQgMC4zOTktMC4xMjYgMC4xMzYtMC4wNDUyIDAuNDcyLTAuMTAzIDAuMzM2LTAuMDU3OCAwLjUwNC0wLjA3OTggMC4xNTgtMC4wMjMxIDAuNTY3LTAuMDc5OCAwLjU1Ni0wLjA2ODIgMC43NzctMC4yMjEgMC4yMi0wLjE1MiAwLjIyLTAuNDQxdi0wLjI1MnEwLTAuNDMtMC4zNTctMC42NjItMC4zMzYtMC4yMzEtMC45NzYtMC4yMzEtMC42NjIgMC0wLjk5OCAwLjI2Mi0wLjMzNiAwLjI1Mi0wLjM5OSAwLjc5OHptMS44OSAzLjY4cTAuNzg4IDAgMS4yNi0wLjQxIDAuNTA0LTAuNDIgMC41MDQtMC45MDN2LTEuMDVxLTAuMjg0IDAuMTM2LTAuODYxIDAuMjMxLTAuNTY3IDAuMDkxNC0wLjk4NyAwLjE1OC0wLjQyIDAuMDY4Mi0wLjc2NiAwLjMyNi0wLjMzNiAwLjI1Mi0wLjMzNiAwLjcwNHQwLjMwNCAwLjcwNCAwLjg2MSAwLjI1MnoiIHN0cm9rZS13aWR0aD0iMS4wNSIvPgogIDxwYXRoIGQ9Im0xMCA0LjU2aDAuOTQ1djMuMTVxMC42NTEtMC45NzYgMS44OS0wLjk3NiAxLjE2IDAgMS44OSAwLjg0IDAuNjgyIDAuODQgMC42ODIgMi4zMSAwIDEuNDctMC43MDQgMi40Mi0wLjcwNCAwLjg4Mi0xLjg5IDAuODgyLTEuMjYgMC0xLjg5LTEuMDJ2MC43NjZoLTAuODV6bTIuNjIgMy4wNHEtMC43NDYgMC0xLjE2IDAuNjQtMC40NTIgMC42My0wLjQ1MiAxLjY4IDAgMS4wNSAwLjQ1MiAxLjY4dDEuMTYgMC42M3EwLjc3NyAwIDEuMjYtMC42MyAwLjQ5NC0wLjY0IDAuNDk0LTEuNjggMC0xLjA1LTAuNDcyLTEuNjgtMC40NjItMC42NC0xLjI2LTAuNjR6IiBzdHJva2Utd2lkdGg9IjEuMDUiLz4KICA8cGF0aCBkPSJtMi43MyAxNS44IDEzLjYgMC4wMDgxYzAuMDA2OSAwIDAtMi42IDAtMi42IDAtMC4wMDc4LTEuMTUgMC0xLjE1IDAtMC4wMDY5IDAtMC4wMDgzIDEuNS0wLjAwODMgMS41LTJlLTMgLTAuMDAxNC0xMS4zLTAuMDAxNC0xMS4zLTAuMDAxNGwtMC4wMDU5Mi0xLjVjMC0wLjAwNzgtMS4xNyAwLjAwMTMtMS4xNyAwLjAwMTN6IiBzdHJva2Utd2lkdGg9Ii45NzUiLz4KIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-yaml: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1jb250cmFzdDIganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjRDgxQjYwIj4KICAgIDxwYXRoIGQ9Ik03LjIgMTguNnYtNS40TDMgNS42aDMuM2wxLjQgMy4xYy4zLjkuNiAxLjYgMSAyLjUuMy0uOC42LTEuNiAxLTIuNWwxLjQtMy4xaDMuNGwtNC40IDcuNnY1LjVsLTIuOS0uMXoiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxNi41IiByPSIyLjEiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxMSIgcj0iMi4xIi8+CiAgPC9nPgo8L3N2Zz4K);
}

/* Icon CSS class declarations */

.jp-AddAboveIcon {
  background-image: var(--jp-icon-add-above);
}

.jp-AddBelowIcon {
  background-image: var(--jp-icon-add-below);
}

.jp-AddIcon {
  background-image: var(--jp-icon-add);
}

.jp-BellIcon {
  background-image: var(--jp-icon-bell);
}

.jp-BugDotIcon {
  background-image: var(--jp-icon-bug-dot);
}

.jp-BugIcon {
  background-image: var(--jp-icon-bug);
}

.jp-BuildIcon {
  background-image: var(--jp-icon-build);
}

.jp-CaretDownEmptyIcon {
  background-image: var(--jp-icon-caret-down-empty);
}

.jp-CaretDownEmptyThinIcon {
  background-image: var(--jp-icon-caret-down-empty-thin);
}

.jp-CaretDownIcon {
  background-image: var(--jp-icon-caret-down);
}

.jp-CaretLeftIcon {
  background-image: var(--jp-icon-caret-left);
}

.jp-CaretRightIcon {
  background-image: var(--jp-icon-caret-right);
}

.jp-CaretUpEmptyThinIcon {
  background-image: var(--jp-icon-caret-up-empty-thin);
}

.jp-CaretUpIcon {
  background-image: var(--jp-icon-caret-up);
}

.jp-CaseSensitiveIcon {
  background-image: var(--jp-icon-case-sensitive);
}

.jp-CheckIcon {
  background-image: var(--jp-icon-check);
}

.jp-CircleEmptyIcon {
  background-image: var(--jp-icon-circle-empty);
}

.jp-CircleIcon {
  background-image: var(--jp-icon-circle);
}

.jp-ClearIcon {
  background-image: var(--jp-icon-clear);
}

.jp-CloseIcon {
  background-image: var(--jp-icon-close);
}

.jp-CodeCheckIcon {
  background-image: var(--jp-icon-code-check);
}

.jp-CodeIcon {
  background-image: var(--jp-icon-code);
}

.jp-CollapseAllIcon {
  background-image: var(--jp-icon-collapse-all);
}

.jp-ConsoleIcon {
  background-image: var(--jp-icon-console);
}

.jp-CopyIcon {
  background-image: var(--jp-icon-copy);
}

.jp-CopyrightIcon {
  background-image: var(--jp-icon-copyright);
}

.jp-CutIcon {
  background-image: var(--jp-icon-cut);
}

.jp-DeleteIcon {
  background-image: var(--jp-icon-delete);
}

.jp-DownloadIcon {
  background-image: var(--jp-icon-download);
}

.jp-DuplicateIcon {
  background-image: var(--jp-icon-duplicate);
}

.jp-EditIcon {
  background-image: var(--jp-icon-edit);
}

.jp-EllipsesIcon {
  background-image: var(--jp-icon-ellipses);
}

.jp-ErrorIcon {
  background-image: var(--jp-icon-error);
}

.jp-ExpandAllIcon {
  background-image: var(--jp-icon-expand-all);
}

.jp-ExtensionIcon {
  background-image: var(--jp-icon-extension);
}

.jp-FastForwardIcon {
  background-image: var(--jp-icon-fast-forward);
}

.jp-FileIcon {
  background-image: var(--jp-icon-file);
}

.jp-FileUploadIcon {
  background-image: var(--jp-icon-file-upload);
}

.jp-FilterDotIcon {
  background-image: var(--jp-icon-filter-dot);
}

.jp-FilterIcon {
  background-image: var(--jp-icon-filter);
}

.jp-FilterListIcon {
  background-image: var(--jp-icon-filter-list);
}

.jp-FolderFavoriteIcon {
  background-image: var(--jp-icon-folder-favorite);
}

.jp-FolderIcon {
  background-image: var(--jp-icon-folder);
}

.jp-HomeIcon {
  background-image: var(--jp-icon-home);
}

.jp-Html5Icon {
  background-image: var(--jp-icon-html5);
}

.jp-ImageIcon {
  background-image: var(--jp-icon-image);
}

.jp-InfoIcon {
  background-image: var(--jp-icon-info);
}

.jp-InspectorIcon {
  background-image: var(--jp-icon-inspector);
}

.jp-JsonIcon {
  background-image: var(--jp-icon-json);
}

.jp-JuliaIcon {
  background-image: var(--jp-icon-julia);
}

.jp-JupyterFaviconIcon {
  background-image: var(--jp-icon-jupyter-favicon);
}

.jp-JupyterIcon {
  background-image: var(--jp-icon-jupyter);
}

.jp-JupyterlabWordmarkIcon {
  background-image: var(--jp-icon-jupyterlab-wordmark);
}

.jp-KernelIcon {
  background-image: var(--jp-icon-kernel);
}

.jp-KeyboardIcon {
  background-image: var(--jp-icon-keyboard);
}

.jp-LaunchIcon {
  background-image: var(--jp-icon-launch);
}

.jp-LauncherIcon {
  background-image: var(--jp-icon-launcher);
}

.jp-LineFormIcon {
  background-image: var(--jp-icon-line-form);
}

.jp-LinkIcon {
  background-image: var(--jp-icon-link);
}

.jp-ListIcon {
  background-image: var(--jp-icon-list);
}

.jp-MarkdownIcon {
  background-image: var(--jp-icon-markdown);
}

.jp-MoveDownIcon {
  background-image: var(--jp-icon-move-down);
}

.jp-MoveUpIcon {
  background-image: var(--jp-icon-move-up);
}

.jp-NewFolderIcon {
  background-image: var(--jp-icon-new-folder);
}

.jp-NotTrustedIcon {
  background-image: var(--jp-icon-not-trusted);
}

.jp-NotebookIcon {
  background-image: var(--jp-icon-notebook);
}

.jp-NumberingIcon {
  background-image: var(--jp-icon-numbering);
}

.jp-OfflineBoltIcon {
  background-image: var(--jp-icon-offline-bolt);
}

.jp-PaletteIcon {
  background-image: var(--jp-icon-palette);
}

.jp-PasteIcon {
  background-image: var(--jp-icon-paste);
}

.jp-PdfIcon {
  background-image: var(--jp-icon-pdf);
}

.jp-PythonIcon {
  background-image: var(--jp-icon-python);
}

.jp-RKernelIcon {
  background-image: var(--jp-icon-r-kernel);
}

.jp-ReactIcon {
  background-image: var(--jp-icon-react);
}

.jp-RedoIcon {
  background-image: var(--jp-icon-redo);
}

.jp-RefreshIcon {
  background-image: var(--jp-icon-refresh);
}

.jp-RegexIcon {
  background-image: var(--jp-icon-regex);
}

.jp-RunIcon {
  background-image: var(--jp-icon-run);
}

.jp-RunningIcon {
  background-image: var(--jp-icon-running);
}

.jp-SaveIcon {
  background-image: var(--jp-icon-save);
}

.jp-SearchIcon {
  background-image: var(--jp-icon-search);
}

.jp-SettingsIcon {
  background-image: var(--jp-icon-settings);
}

.jp-ShareIcon {
  background-image: var(--jp-icon-share);
}

.jp-SpreadsheetIcon {
  background-image: var(--jp-icon-spreadsheet);
}

.jp-StopIcon {
  background-image: var(--jp-icon-stop);
}

.jp-TabIcon {
  background-image: var(--jp-icon-tab);
}

.jp-TableRowsIcon {
  background-image: var(--jp-icon-table-rows);
}

.jp-TagIcon {
  background-image: var(--jp-icon-tag);
}

.jp-TerminalIcon {
  background-image: var(--jp-icon-terminal);
}

.jp-TextEditorIcon {
  background-image: var(--jp-icon-text-editor);
}

.jp-TocIcon {
  background-image: var(--jp-icon-toc);
}

.jp-TreeViewIcon {
  background-image: var(--jp-icon-tree-view);
}

.jp-TrustedIcon {
  background-image: var(--jp-icon-trusted);
}

.jp-UndoIcon {
  background-image: var(--jp-icon-undo);
}

.jp-UserIcon {
  background-image: var(--jp-icon-user);
}

.jp-UsersIcon {
  background-image: var(--jp-icon-users);
}

.jp-VegaIcon {
  background-image: var(--jp-icon-vega);
}

.jp-WordIcon {
  background-image: var(--jp-icon-word);
}

.jp-YamlIcon {
  background-image: var(--jp-icon-yaml);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * (DEPRECATED) Support for consuming icons as CSS background images
 */

.jp-Icon,
.jp-MaterialIcon {
  background-position: center;
  background-repeat: no-repeat;
  background-size: 16px;
  min-width: 16px;
  min-height: 16px;
}

.jp-Icon-cover {
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

/**
 * (DEPRECATED) Support for specific CSS icon sizes
 */

.jp-Icon-16 {
  background-size: 16px;
  min-width: 16px;
  min-height: 16px;
}

.jp-Icon-18 {
  background-size: 18px;
  min-width: 18px;
  min-height: 18px;
}

.jp-Icon-20 {
  background-size: 20px;
  min-width: 20px;
  min-height: 20px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.lm-TabBar .lm-TabBar-addButton {
  align-items: center;
  display: flex;
  padding: 4px;
  padding-bottom: 5px;
  margin-right: 1px;
  background-color: var(--jp-layout-color2);
}

.lm-TabBar .lm-TabBar-addButton:hover {
  background-color: var(--jp-layout-color1);
}

.lm-DockPanel-tabBar .lm-TabBar-tab {
  width: var(--jp-private-horizontal-tab-width);
}

.lm-DockPanel-tabBar .lm-TabBar-content {
  flex: unset;
}

.lm-DockPanel-tabBar[data-orientation='horizontal'] {
  flex: 1 1 auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * Support for icons as inline SVG HTMLElements
 */

/* recolor the primary elements of an icon */
.jp-icon0[fill] {
  fill: var(--jp-inverse-layout-color0);
}

.jp-icon1[fill] {
  fill: var(--jp-inverse-layout-color1);
}

.jp-icon2[fill] {
  fill: var(--jp-inverse-layout-color2);
}

.jp-icon3[fill] {
  fill: var(--jp-inverse-layout-color3);
}

.jp-icon4[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon0[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}

.jp-icon1[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}

.jp-icon2[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}

.jp-icon3[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}

.jp-icon4[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/* recolor the accent elements of an icon */
.jp-icon-accent0[fill] {
  fill: var(--jp-layout-color0);
}

.jp-icon-accent1[fill] {
  fill: var(--jp-layout-color1);
}

.jp-icon-accent2[fill] {
  fill: var(--jp-layout-color2);
}

.jp-icon-accent3[fill] {
  fill: var(--jp-layout-color3);
}

.jp-icon-accent4[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-accent0[stroke] {
  stroke: var(--jp-layout-color0);
}

.jp-icon-accent1[stroke] {
  stroke: var(--jp-layout-color1);
}

.jp-icon-accent2[stroke] {
  stroke: var(--jp-layout-color2);
}

.jp-icon-accent3[stroke] {
  stroke: var(--jp-layout-color3);
}

.jp-icon-accent4[stroke] {
  stroke: var(--jp-layout-color4);
}

/* set the color of an icon to transparent */
.jp-icon-none[fill] {
  fill: none;
}

.jp-icon-none[stroke] {
  stroke: none;
}

/* brand icon colors. Same for light and dark */
.jp-icon-brand0[fill] {
  fill: var(--jp-brand-color0);
}

.jp-icon-brand1[fill] {
  fill: var(--jp-brand-color1);
}

.jp-icon-brand2[fill] {
  fill: var(--jp-brand-color2);
}

.jp-icon-brand3[fill] {
  fill: var(--jp-brand-color3);
}

.jp-icon-brand4[fill] {
  fill: var(--jp-brand-color4);
}

.jp-icon-brand0[stroke] {
  stroke: var(--jp-brand-color0);
}

.jp-icon-brand1[stroke] {
  stroke: var(--jp-brand-color1);
}

.jp-icon-brand2[stroke] {
  stroke: var(--jp-brand-color2);
}

.jp-icon-brand3[stroke] {
  stroke: var(--jp-brand-color3);
}

.jp-icon-brand4[stroke] {
  stroke: var(--jp-brand-color4);
}

/* warn icon colors. Same for light and dark */
.jp-icon-warn0[fill] {
  fill: var(--jp-warn-color0);
}

.jp-icon-warn1[fill] {
  fill: var(--jp-warn-color1);
}

.jp-icon-warn2[fill] {
  fill: var(--jp-warn-color2);
}

.jp-icon-warn3[fill] {
  fill: var(--jp-warn-color3);
}

.jp-icon-warn0[stroke] {
  stroke: var(--jp-warn-color0);
}

.jp-icon-warn1[stroke] {
  stroke: var(--jp-warn-color1);
}

.jp-icon-warn2[stroke] {
  stroke: var(--jp-warn-color2);
}

.jp-icon-warn3[stroke] {
  stroke: var(--jp-warn-color3);
}

/* icon colors that contrast well with each other and most backgrounds */
.jp-icon-contrast0[fill] {
  fill: var(--jp-icon-contrast-color0);
}

.jp-icon-contrast1[fill] {
  fill: var(--jp-icon-contrast-color1);
}

.jp-icon-contrast2[fill] {
  fill: var(--jp-icon-contrast-color2);
}

.jp-icon-contrast3[fill] {
  fill: var(--jp-icon-contrast-color3);
}

.jp-icon-contrast0[stroke] {
  stroke: var(--jp-icon-contrast-color0);
}

.jp-icon-contrast1[stroke] {
  stroke: var(--jp-icon-contrast-color1);
}

.jp-icon-contrast2[stroke] {
  stroke: var(--jp-icon-contrast-color2);
}

.jp-icon-contrast3[stroke] {
  stroke: var(--jp-icon-contrast-color3);
}

.jp-icon-dot[fill] {
  fill: var(--jp-warn-color0);
}

.jp-jupyter-icon-color[fill] {
  fill: var(--jp-jupyter-icon-color, var(--jp-warn-color0));
}

.jp-notebook-icon-color[fill] {
  fill: var(--jp-notebook-icon-color, var(--jp-warn-color0));
}

.jp-json-icon-color[fill] {
  fill: var(--jp-json-icon-color, var(--jp-warn-color1));
}

.jp-console-icon-color[fill] {
  fill: var(--jp-console-icon-color, white);
}

.jp-console-icon-background-color[fill] {
  fill: var(--jp-console-icon-background-color, var(--jp-brand-color1));
}

.jp-terminal-icon-color[fill] {
  fill: var(--jp-terminal-icon-color, var(--jp-layout-color2));
}

.jp-terminal-icon-background-color[fill] {
  fill: var(
    --jp-terminal-icon-background-color,
    var(--jp-inverse-layout-color2)
  );
}

.jp-text-editor-icon-color[fill] {
  fill: var(--jp-text-editor-icon-color, var(--jp-inverse-layout-color3));
}

.jp-inspector-icon-color[fill] {
  fill: var(--jp-inspector-icon-color, var(--jp-inverse-layout-color3));
}

/* CSS for icons in selected filebrowser listing items */
.jp-DirListing-item.jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}

.jp-DirListing-item.jp-mod-selected .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}

/* stylelint-disable selector-max-class, selector-max-compound-selectors */

/**
* TODO: come up with non css-hack solution for showing the busy icon on top
*  of the close icon
* CSS for complex behavior of close icon of tabs in the main area tabbar
*/
.lm-DockPanel-tabBar
  .lm-TabBar-tab.lm-mod-closable.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon3[fill] {
  fill: none;
}

.lm-DockPanel-tabBar
  .lm-TabBar-tab.lm-mod-closable.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon-busy[fill] {
  fill: var(--jp-inverse-layout-color3);
}

/* stylelint-enable selector-max-class, selector-max-compound-selectors */

/* CSS for icons in status bar */
#jp-main-statusbar .jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}

#jp-main-statusbar .jp-mod-selected .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}

/* special handling for splash icon CSS. While the theme CSS reloads during
   splash, the splash icon can loose theming. To prevent that, we set a
   default for its color variable */
:root {
  --jp-warn-color0: var(--md-orange-700);
}

/* not sure what to do with this one, used in filebrowser listing */
.jp-DragIcon {
  margin-right: 4px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * Support for alt colors for icons as inline SVG HTMLElements
 */

/* alt recolor the primary elements of an icon */
.jp-icon-alt .jp-icon0[fill] {
  fill: var(--jp-layout-color0);
}

.jp-icon-alt .jp-icon1[fill] {
  fill: var(--jp-layout-color1);
}

.jp-icon-alt .jp-icon2[fill] {
  fill: var(--jp-layout-color2);
}

.jp-icon-alt .jp-icon3[fill] {
  fill: var(--jp-layout-color3);
}

.jp-icon-alt .jp-icon4[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-alt .jp-icon0[stroke] {
  stroke: var(--jp-layout-color0);
}

.jp-icon-alt .jp-icon1[stroke] {
  stroke: var(--jp-layout-color1);
}

.jp-icon-alt .jp-icon2[stroke] {
  stroke: var(--jp-layout-color2);
}

.jp-icon-alt .jp-icon3[stroke] {
  stroke: var(--jp-layout-color3);
}

.jp-icon-alt .jp-icon4[stroke] {
  stroke: var(--jp-layout-color4);
}

/* alt recolor the accent elements of an icon */
.jp-icon-alt .jp-icon-accent0[fill] {
  fill: var(--jp-inverse-layout-color0);
}

.jp-icon-alt .jp-icon-accent1[fill] {
  fill: var(--jp-inverse-layout-color1);
}

.jp-icon-alt .jp-icon-accent2[fill] {
  fill: var(--jp-inverse-layout-color2);
}

.jp-icon-alt .jp-icon-accent3[fill] {
  fill: var(--jp-inverse-layout-color3);
}

.jp-icon-alt .jp-icon-accent4[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-alt .jp-icon-accent0[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}

.jp-icon-alt .jp-icon-accent1[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}

.jp-icon-alt .jp-icon-accent2[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}

.jp-icon-alt .jp-icon-accent3[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}

.jp-icon-alt .jp-icon-accent4[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-icon-hoverShow:not(:hover) .jp-icon-hoverShow-content {
  display: none !important;
}

/**
 * Support for hover colors for icons as inline SVG HTMLElements
 */

/**
 * regular colors
 */

/* recolor the primary elements of an icon */
.jp-icon-hover :hover .jp-icon0-hover[fill] {
  fill: var(--jp-inverse-layout-color0);
}

.jp-icon-hover :hover .jp-icon1-hover[fill] {
  fill: var(--jp-inverse-layout-color1);
}

.jp-icon-hover :hover .jp-icon2-hover[fill] {
  fill: var(--jp-inverse-layout-color2);
}

.jp-icon-hover :hover .jp-icon3-hover[fill] {
  fill: var(--jp-inverse-layout-color3);
}

.jp-icon-hover :hover .jp-icon4-hover[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-hover :hover .jp-icon0-hover[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}

.jp-icon-hover :hover .jp-icon1-hover[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}

.jp-icon-hover :hover .jp-icon2-hover[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}

.jp-icon-hover :hover .jp-icon3-hover[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}

.jp-icon-hover :hover .jp-icon4-hover[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/* recolor the accent elements of an icon */
.jp-icon-hover :hover .jp-icon-accent0-hover[fill] {
  fill: var(--jp-layout-color0);
}

.jp-icon-hover :hover .jp-icon-accent1-hover[fill] {
  fill: var(--jp-layout-color1);
}

.jp-icon-hover :hover .jp-icon-accent2-hover[fill] {
  fill: var(--jp-layout-color2);
}

.jp-icon-hover :hover .jp-icon-accent3-hover[fill] {
  fill: var(--jp-layout-color3);
}

.jp-icon-hover :hover .jp-icon-accent4-hover[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-hover :hover .jp-icon-accent0-hover[stroke] {
  stroke: var(--jp-layout-color0);
}

.jp-icon-hover :hover .jp-icon-accent1-hover[stroke] {
  stroke: var(--jp-layout-color1);
}

.jp-icon-hover :hover .jp-icon-accent2-hover[stroke] {
  stroke: var(--jp-layout-color2);
}

.jp-icon-hover :hover .jp-icon-accent3-hover[stroke] {
  stroke: var(--jp-layout-color3);
}

.jp-icon-hover :hover .jp-icon-accent4-hover[stroke] {
  stroke: var(--jp-layout-color4);
}

/* set the color of an icon to transparent */
.jp-icon-hover :hover .jp-icon-none-hover[fill] {
  fill: none;
}

.jp-icon-hover :hover .jp-icon-none-hover[stroke] {
  stroke: none;
}

/**
 * inverse colors
 */

/* inverse recolor the primary elements of an icon */
.jp-icon-hover.jp-icon-alt :hover .jp-icon0-hover[fill] {
  fill: var(--jp-layout-color0);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon1-hover[fill] {
  fill: var(--jp-layout-color1);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon2-hover[fill] {
  fill: var(--jp-layout-color2);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon3-hover[fill] {
  fill: var(--jp-layout-color3);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon4-hover[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon0-hover[stroke] {
  stroke: var(--jp-layout-color0);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon1-hover[stroke] {
  stroke: var(--jp-layout-color1);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon2-hover[stroke] {
  stroke: var(--jp-layout-color2);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon3-hover[stroke] {
  stroke: var(--jp-layout-color3);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon4-hover[stroke] {
  stroke: var(--jp-layout-color4);
}

/* inverse recolor the accent elements of an icon */
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent0-hover[fill] {
  fill: var(--jp-inverse-layout-color0);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent1-hover[fill] {
  fill: var(--jp-inverse-layout-color1);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent2-hover[fill] {
  fill: var(--jp-inverse-layout-color2);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent3-hover[fill] {
  fill: var(--jp-inverse-layout-color3);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent4-hover[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent0-hover[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent1-hover[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent2-hover[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent3-hover[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent4-hover[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-IFrame {
  width: 100%;
  height: 100%;
}

.jp-IFrame > iframe {
  border: none;
}

/*
When drag events occur, `lm-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-IFrame {
  position: relative;
}

body.lm-mod-override-cursor .jp-IFrame::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-HoverBox {
  position: fixed;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-FormGroup-content fieldset {
  border: none;
  padding: 0;
  min-width: 0;
  width: 100%;
}

/* stylelint-disable selector-max-type */

.jp-FormGroup-content fieldset .jp-inputFieldWrapper input,
.jp-FormGroup-content fieldset .jp-inputFieldWrapper select,
.jp-FormGroup-content fieldset .jp-inputFieldWrapper textarea {
  font-size: var(--jp-content-font-size2);
  border-color: var(--jp-input-border-color);
  border-style: solid;
  border-radius: var(--jp-border-radius);
  border-width: 1px;
  padding: 6px 8px;
  background: none;
  color: var(--jp-ui-font-color0);
  height: inherit;
}

.jp-FormGroup-content fieldset input[type='checkbox'] {
  position: relative;
  top: 2px;
  margin-left: 0;
}

.jp-FormGroup-content button.jp-mod-styled {
  cursor: pointer;
}

.jp-FormGroup-content .checkbox label {
  cursor: pointer;
  font-size: var(--jp-content-font-size1);
}

.jp-FormGroup-content .jp-root > fieldset > legend {
  display: none;
}

.jp-FormGroup-content .jp-root > fieldset > p {
  display: none;
}

/** copy of `input.jp-mod-styled:focus` style */
.jp-FormGroup-content fieldset input:focus,
.jp-FormGroup-content fieldset select:focus {
  -moz-outline-radius: unset;
  outline: var(--jp-border-width) solid var(--md-blue-500);
  outline-offset: -1px;
  box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-FormGroup-content fieldset input:hover:not(:focus),
.jp-FormGroup-content fieldset select:hover:not(:focus) {
  background-color: var(--jp-border-color2);
}

/* stylelint-enable selector-max-type */

.jp-FormGroup-content .checkbox .field-description {
  /* Disable default description field for checkbox:
   because other widgets do not have description fields,
   we add descriptions to each widget on the field level.
  */
  display: none;
}

.jp-FormGroup-content #root__description {
  display: none;
}

.jp-FormGroup-content .jp-modifiedIndicator {
  width: 5px;
  background-color: var(--jp-brand-color2);
  margin-top: 0;
  margin-left: calc(var(--jp-private-settingeditor-modifier-indent) * -1);
  flex-shrink: 0;
}

.jp-FormGroup-content .jp-modifiedIndicator.jp-errorIndicator {
  background-color: var(--jp-error-color0);
  margin-right: 0.5em;
}

/* RJSF ARRAY style */

.jp-arrayFieldWrapper legend {
  font-size: var(--jp-content-font-size2);
  color: var(--jp-ui-font-color0);
  flex-basis: 100%;
  padding: 4px 0;
  font-weight: var(--jp-content-heading-font-weight);
  border-bottom: 1px solid var(--jp-border-color2);
}

.jp-arrayFieldWrapper .field-description {
  padding: 4px 0;
  white-space: pre-wrap;
}

.jp-arrayFieldWrapper .array-item {
  width: 100%;
  border: 1px solid var(--jp-border-color2);
  border-radius: 4px;
  margin: 4px;
}

.jp-ArrayOperations {
  display: flex;
  margin-left: 8px;
}

.jp-ArrayOperationsButton {
  margin: 2px;
}

.jp-ArrayOperationsButton .jp-icon3[fill] {
  fill: var(--jp-ui-font-color0);
}

button.jp-ArrayOperationsButton.jp-mod-styled:disabled {
  cursor: not-allowed;
  opacity: 0.5;
}

/* RJSF form validation error */

.jp-FormGroup-content .validationErrors {
  color: var(--jp-error-color0);
}

/* Hide panel level error as duplicated the field level error */
.jp-FormGroup-content .panel.errors {
  display: none;
}

/* RJSF normal content (settings-editor) */

.jp-FormGroup-contentNormal {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

.jp-FormGroup-contentNormal .jp-FormGroup-contentItem {
  margin-left: 7px;
  color: var(--jp-ui-font-color0);
}

.jp-FormGroup-contentNormal .jp-FormGroup-description {
  flex-basis: 100%;
  padding: 4px 7px;
}

.jp-FormGroup-contentNormal .jp-FormGroup-default {
  flex-basis: 100%;
  padding: 4px 7px;
}

.jp-FormGroup-contentNormal .jp-FormGroup-fieldLabel {
  font-size: var(--jp-content-font-size1);
  font-weight: normal;
  min-width: 120px;
}

.jp-FormGroup-contentNormal fieldset:not(:first-child) {
  margin-left: 7px;
}

.jp-FormGroup-contentNormal .field-array-of-string .array-item {
  /* Display `jp-ArrayOperations` buttons side-by-side with content except
    for small screens where flex-wrap will place them one below the other.
  */
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

.jp-FormGroup-contentNormal .jp-objectFieldWrapper .form-group {
  padding: 2px 8px 2px var(--jp-private-settingeditor-modifier-indent);
  margin-top: 2px;
}

/* RJSF compact content (metadata-form) */

.jp-FormGroup-content.jp-FormGroup-contentCompact {
  width: 100%;
}

.jp-FormGroup-contentCompact .form-group {
  display: flex;
  padding: 0.5em 0.2em 0.5em 0;
}

.jp-FormGroup-contentCompact
  .jp-FormGroup-compactTitle
  .jp-FormGroup-description {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color2);
}

.jp-FormGroup-contentCompact .jp-FormGroup-fieldLabel {
  padding-bottom: 0.3em;
}

.jp-FormGroup-contentCompact .jp-inputFieldWrapper .form-control {
  width: 100%;
  box-sizing: border-box;
}

.jp-FormGroup-contentCompact .jp-arrayFieldWrapper .jp-FormGroup-compactTitle {
  padding-bottom: 7px;
}

.jp-FormGroup-contentCompact
  .jp-objectFieldWrapper
  .jp-objectFieldWrapper
  .form-group {
  padding: 2px 8px 2px var(--jp-private-settingeditor-modifier-indent);
  margin-top: 2px;
}

.jp-FormGroup-contentCompact ul.error-detail {
  margin-block-start: 0.5em;
  margin-block-end: 0.5em;
  padding-inline-start: 1em;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-SidePanel {
  display: flex;
  flex-direction: column;
  min-width: var(--jp-sidebar-min-width);
  overflow-y: auto;
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);
  font-size: var(--jp-ui-font-size1);
}

.jp-SidePanel-header {
  flex: 0 0 auto;
  display: flex;
  border-bottom: var(--jp-border-width) solid var(--jp-border-color2);
  font-size: var(--jp-ui-font-size0);
  font-weight: 600;
  letter-spacing: 1px;
  margin: 0;
  padding: 2px;
  text-transform: uppercase;
}

.jp-SidePanel-toolbar {
  flex: 0 0 auto;
}

.jp-SidePanel-content {
  flex: 1 1 auto;
}

.jp-SidePanel-toolbar,
.jp-AccordionPanel-toolbar {
  height: var(--jp-private-toolbar-height);
}

.jp-SidePanel-toolbar.jp-Toolbar-micro {
  display: none;
}

.lm-AccordionPanel .jp-AccordionPanel-title {
  box-sizing: border-box;
  line-height: 25px;
  margin: 0;
  display: flex;
  align-items: center;
  background: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  box-shadow: var(--jp-toolbar-box-shadow);
  font-size: var(--jp-ui-font-size0);
}

.jp-AccordionPanel-title {
  cursor: pointer;
  user-select: none;
  -moz-user-select: none;
  -webkit-user-select: none;
  text-transform: uppercase;
}

.lm-AccordionPanel[data-orientation='horizontal'] > .jp-AccordionPanel-title {
  /* Title is rotated for horizontal accordion panel using CSS */
  display: block;
  transform-origin: top left;
  transform: rotate(-90deg) translate(-100%);
}

.jp-AccordionPanel-title .lm-AccordionPanel-titleLabel {
  user-select: none;
  text-overflow: ellipsis;
  white-space: nowrap;
  overflow: hidden;
}

.jp-AccordionPanel-title .lm-AccordionPanel-titleCollapser {
  transform: rotate(-90deg);
  margin: auto 0;
  height: 16px;
}

.jp-AccordionPanel-title.lm-mod-expanded .lm-AccordionPanel-titleCollapser {
  transform: rotate(0deg);
}

.lm-AccordionPanel .jp-AccordionPanel-toolbar {
  background: none;
  box-shadow: none;
  border: none;
  margin-left: auto;
}

.lm-AccordionPanel .lm-SplitPanel-handle:hover {
  background: var(--jp-layout-color3);
}

.jp-text-truncated {
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Spinner {
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 10;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background: var(--jp-layout-color0);
  outline: none;
}

.jp-SpinnerContent {
  font-size: 10px;
  margin: 50px auto;
  text-indent: -9999em;
  width: 3em;
  height: 3em;
  border-radius: 50%;
  background: var(--jp-brand-color3);
  background: linear-gradient(
    to right,
    #f37626 10%,
    rgba(255, 255, 255, 0) 42%
  );
  position: relative;
  animation: load3 1s infinite linear, fadeIn 1s;
}

.jp-SpinnerContent::before {
  width: 50%;
  height: 50%;
  background: #f37626;
  border-radius: 100% 0 0;
  position: absolute;
  top: 0;
  left: 0;
  content: '';
}

.jp-SpinnerContent::after {
  background: var(--jp-layout-color0);
  width: 75%;
  height: 75%;
  border-radius: 50%;
  content: '';
  margin: auto;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }

  100% {
    opacity: 1;
  }
}

@keyframes load3 {
  0% {
    transform: rotate(0deg);
  }

  100% {
    transform: rotate(360deg);
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

button.jp-mod-styled {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  border: none;
  box-sizing: border-box;
  text-align: center;
  line-height: 32px;
  height: 32px;
  padding: 0 12px;
  letter-spacing: 0.8px;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

input.jp-mod-styled {
  background: var(--jp-input-background);
  height: 28px;
  box-sizing: border-box;
  border: var(--jp-border-width) solid var(--jp-border-color1);
  padding-left: 7px;
  padding-right: 7px;
  font-size: var(--jp-ui-font-size2);
  color: var(--jp-ui-font-color0);
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

input[type='checkbox'].jp-mod-styled {
  appearance: checkbox;
  -webkit-appearance: checkbox;
  -moz-appearance: checkbox;
  height: auto;
}

input.jp-mod-styled:focus {
  border: var(--jp-border-width) solid var(--md-blue-500);
  box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-select-wrapper {
  display: flex;
  position: relative;
  flex-direction: column;
  padding: 1px;
  background-color: var(--jp-layout-color1);
  box-sizing: border-box;
  margin-bottom: 12px;
}

.jp-select-wrapper:not(.multiple) {
  height: 28px;
}

.jp-select-wrapper.jp-mod-focused select.jp-mod-styled {
  border: var(--jp-border-width) solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
  background-color: var(--jp-input-active-background);
}

select.jp-mod-styled:hover {
  cursor: pointer;
  color: var(--jp-ui-font-color0);
  background-color: var(--jp-input-hover-background);
  box-shadow: inset 0 0 1px rgba(0, 0, 0, 0.5);
}

select.jp-mod-styled {
  flex: 1 1 auto;
  width: 100%;
  font-size: var(--jp-ui-font-size2);
  background: var(--jp-input-background);
  color: var(--jp-ui-font-color0);
  padding: 0 25px 0 8px;
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  border-radius: 0;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

select.jp-mod-styled:not([multiple]) {
  height: 32px;
}

select.jp-mod-styled[multiple] {
  max-height: 200px;
  overflow-y: auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-switch {
  display: flex;
  align-items: center;
  padding-left: 4px;
  padding-right: 4px;
  font-size: var(--jp-ui-font-size1);
  background-color: transparent;
  color: var(--jp-ui-font-color1);
  border: none;
  height: 20px;
}

.jp-switch:hover {
  background-color: var(--jp-layout-color2);
}

.jp-switch-label {
  margin-right: 5px;
  font-family: var(--jp-ui-font-family);
}

.jp-switch-track {
  cursor: pointer;
  background-color: var(--jp-switch-color, var(--jp-border-color1));
  -webkit-transition: 0.4s;
  transition: 0.4s;
  border-radius: 34px;
  height: 16px;
  width: 35px;
  position: relative;
}

.jp-switch-track::before {
  content: '';
  position: absolute;
  height: 10px;
  width: 10px;
  margin: 3px;
  left: 0;
  background-color: var(--jp-ui-inverse-font-color1);
  -webkit-transition: 0.4s;
  transition: 0.4s;
  border-radius: 50%;
}

.jp-switch[aria-checked='true'] .jp-switch-track {
  background-color: var(--jp-switch-true-position-color, var(--jp-warn-color0));
}

.jp-switch[aria-checked='true'] .jp-switch-track::before {
  /* track width (35) - margins (3 + 3) - thumb width (10) */
  left: 19px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

:root {
  --jp-private-toolbar-height: calc(
    28px + var(--jp-border-width)
  ); /* leave 28px for content */
}

.jp-Toolbar {
  color: var(--jp-ui-font-color1);
  flex: 0 0 auto;
  display: flex;
  flex-direction: row;
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  box-shadow: var(--jp-toolbar-box-shadow);
  background: var(--jp-toolbar-background);
  min-height: var(--jp-toolbar-micro-height);
  padding: 2px;
  z-index: 8;
  overflow-x: hidden;
}

/* Toolbar items */

.jp-Toolbar > .jp-Toolbar-item.jp-Toolbar-spacer {
  flex-grow: 1;
  flex-shrink: 1;
}

.jp-Toolbar-item.jp-Toolbar-kernelStatus {
  display: inline-block;
  width: 32px;
  background-repeat: no-repeat;
  background-position: center;
  background-size: 16px;
}

.jp-Toolbar > .jp-Toolbar-item {
  flex: 0 0 auto;
  display: flex;
  padding-left: 1px;
  padding-right: 1px;
  font-size: var(--jp-ui-font-size1);
  line-height: var(--jp-private-toolbar-height);
  height: 100%;
}

/* Toolbar buttons */

/* This is the div we use to wrap the react component into a Widget */
div.jp-ToolbarButton {
  color: transparent;
  border: none;
  box-sizing: border-box;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  padding: 0;
  margin: 0;
}

button.jp-ToolbarButtonComponent {
  background: var(--jp-layout-color1);
  border: none;
  box-sizing: border-box;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  padding: 0 6px;
  margin: 0;
  height: 24px;
  border-radius: var(--jp-border-radius);
  display: flex;
  align-items: center;
  text-align: center;
  font-size: 14px;
  min-width: unset;
  min-height: unset;
}

button.jp-ToolbarButtonComponent:disabled {
  opacity: 0.4;
}

button.jp-ToolbarButtonComponent > span {
  padding: 0;
  flex: 0 0 auto;
}

button.jp-ToolbarButtonComponent .jp-ToolbarButtonComponent-label {
  font-size: var(--jp-ui-font-size1);
  line-height: 100%;
  padding-left: 2px;
  color: var(--jp-ui-font-color1);
  font-family: var(--jp-ui-font-family);
}

#jp-main-dock-panel[data-mode='single-document']
  .jp-MainAreaWidget
  > .jp-Toolbar.jp-Toolbar-micro {
  padding: 0;
  min-height: 0;
}

#jp-main-dock-panel[data-mode='single-document']
  .jp-MainAreaWidget
  > .jp-Toolbar {
  border: none;
  box-shadow: none;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-WindowedPanel-outer {
  position: relative;
  overflow-y: auto;
}

.jp-WindowedPanel-inner {
  position: relative;
}

.jp-WindowedPanel-window {
  position: absolute;
  left: 0;
  right: 0;
  overflow: visible;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* Sibling imports */

body {
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
}

/* Disable native link decoration styles everywhere outside of dialog boxes */
a {
  text-decoration: unset;
  color: unset;
}

a:hover {
  text-decoration: unset;
  color: unset;
}

/* Accessibility for links inside dialog box text */
.jp-Dialog-content a {
  text-decoration: revert;
  color: var(--jp-content-link-color);
}

.jp-Dialog-content a:hover {
  text-decoration: revert;
}

/* Styles for ui-components */
.jp-Button {
  color: var(--jp-ui-font-color2);
  border-radius: var(--jp-border-radius);
  padding: 0 12px;
  font-size: var(--jp-ui-font-size1);

  /* Copy from blueprint 3 */
  display: inline-flex;
  flex-direction: row;
  border: none;
  cursor: pointer;
  align-items: center;
  justify-content: center;
  text-align: left;
  vertical-align: middle;
  min-height: 30px;
  min-width: 30px;
}

.jp-Button:disabled {
  cursor: not-allowed;
}

.jp-Button:empty {
  padding: 0 !important;
}

.jp-Button.jp-mod-small {
  min-height: 24px;
  min-width: 24px;
  font-size: 12px;
  padding: 0 7px;
}

/* Use our own theme for hover styles */
.jp-Button.jp-mod-minimal:hover {
  background-color: var(--jp-layout-color2);
}

.jp-Button.jp-mod-minimal {
  background: none;
}

.jp-InputGroup {
  display: block;
  position: relative;
}

.jp-InputGroup input {
  box-sizing: border-box;
  border: none;
  border-radius: 0;
  background-color: transparent;
  color: var(--jp-ui-font-color0);
  box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
  padding-bottom: 0;
  padding-top: 0;
  padding-left: 10px;
  padding-right: 28px;
  position: relative;
  width: 100%;
  -webkit-appearance: none;
  -moz-appearance: none;
  appearance: none;
  font-size: 14px;
  font-weight: 400;
  height: 30px;
  line-height: 30px;
  outline: none;
  vertical-align: middle;
}

.jp-InputGroup input:focus {
  box-shadow: inset 0 0 0 var(--jp-border-width)
      var(--jp-input-active-box-shadow-color),
    inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.jp-InputGroup input:disabled {
  cursor: not-allowed;
  resize: block;
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color2);
}

.jp-InputGroup input:disabled ~ span {
  cursor: not-allowed;
  color: var(--jp-ui-font-color2);
}

.jp-InputGroup input::placeholder,
input::placeholder {
  color: var(--jp-ui-font-color2);
}

.jp-InputGroupAction {
  position: absolute;
  bottom: 1px;
  right: 0;
  padding: 6px;
}

.jp-HTMLSelect.jp-DefaultStyle select {
  background-color: initial;
  border: none;
  border-radius: 0;
  box-shadow: none;
  color: var(--jp-ui-font-color0);
  display: block;
  font-size: var(--jp-ui-font-size1);
  font-family: var(--jp-ui-font-family);
  height: 24px;
  line-height: 14px;
  padding: 0 25px 0 10px;
  text-align: left;
  -moz-appearance: none;
  -webkit-appearance: none;
}

.jp-HTMLSelect.jp-DefaultStyle select:disabled {
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color2);
  cursor: not-allowed;
  resize: block;
}

.jp-HTMLSelect.jp-DefaultStyle select:disabled ~ span {
  cursor: not-allowed;
}

/* Use our own theme for hover and option styles */
/* stylelint-disable-next-line selector-max-type */
.jp-HTMLSelect.jp-DefaultStyle select:hover,
.jp-HTMLSelect.jp-DefaultStyle select > option {
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color0);
}

select {
  box-sizing: border-box;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-StatusBar-Widget {
  display: flex;
  align-items: center;
  background: var(--jp-layout-color2);
  min-height: var(--jp-statusbar-height);
  justify-content: space-between;
  padding: 0 10px;
}

.jp-StatusBar-Left {
  display: flex;
  align-items: center;
  flex-direction: row;
}

.jp-StatusBar-Middle {
  display: flex;
  align-items: center;
}

.jp-StatusBar-Right {
  display: flex;
  align-items: center;
  flex-direction: row-reverse;
}

.jp-StatusBar-Item {
  max-height: var(--jp-statusbar-height);
  margin: 0 2px;
  height: var(--jp-statusbar-height);
  white-space: nowrap;
  text-overflow: ellipsis;
  color: var(--jp-ui-font-color1);
  padding: 0 6px;
}

.jp-mod-highlighted:hover {
  background-color: var(--jp-layout-color3);
}

.jp-mod-clicked {
  background-color: var(--jp-brand-color1);
}

.jp-mod-clicked:hover {
  background-color: var(--jp-brand-color0);
}

.jp-mod-clicked .jp-StatusBar-TextItem {
  color: var(--jp-ui-inverse-font-color1);
}

.jp-StatusBar-HoverItem {
  box-shadow: '0px 4px 4px rgba(0, 0, 0, 0.25)';
}

.jp-StatusBar-TextItem {
  font-size: var(--jp-ui-font-size1);
  font-family: var(--jp-ui-font-family);
  line-height: 24px;
  color: var(--jp-ui-font-color1);
}

.jp-StatusBar-GroupItem {
  display: flex;
  align-items: center;
  flex-direction: row;
}

.jp-Statusbar-ProgressCircle svg {
  display: block;
  margin: 0 auto;
  width: 16px;
  height: 24px;
  align-self: normal;
}

.jp-Statusbar-ProgressCircle path {
  fill: var(--jp-inverse-layout-color3);
}

.jp-Statusbar-ProgressBar-progress-bar {
  height: 10px;
  width: 100px;
  border: solid 0.25px var(--jp-brand-color2);
  border-radius: 3px;
  overflow: hidden;
  align-self: center;
}

.jp-Statusbar-ProgressBar-progress-bar > div {
  background-color: var(--jp-brand-color2);
  background-image: linear-gradient(
    -45deg,
    rgba(255, 255, 255, 0.2) 25%,
    transparent 25%,
    transparent 50%,
    rgba(255, 255, 255, 0.2) 50%,
    rgba(255, 255, 255, 0.2) 75%,
    transparent 75%,
    transparent
  );
  background-size: 40px 40px;
  float: left;
  width: 0%;
  height: 100%;
  font-size: 12px;
  line-height: 14px;
  color: #fff;
  text-align: center;
  animation: jp-Statusbar-ExecutionTime-progress-bar 2s linear infinite;
}

.jp-Statusbar-ProgressBar-progress-bar p {
  color: var(--jp-ui-font-color1);
  font-family: var(--jp-ui-font-family);
  font-size: var(--jp-ui-font-size1);
  line-height: 10px;
  width: 100px;
}

@keyframes jp-Statusbar-ExecutionTime-progress-bar {
  0% {
    background-position: 0 0;
  }

  100% {
    background-position: 40px 40px;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-commandpalette-search-height: 28px;
}

/*-----------------------------------------------------------------------------
| Overall styles
|----------------------------------------------------------------------------*/

.lm-CommandPalette {
  padding-bottom: 0;
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);

  /* This is needed so that all font sizing of children done in ems is
   * relative to this base size */
  font-size: var(--jp-ui-font-size1);
}

/*-----------------------------------------------------------------------------
| Modal variant
|----------------------------------------------------------------------------*/

.jp-ModalCommandPalette {
  position: absolute;
  z-index: 10000;
  top: 38px;
  left: 30%;
  margin: 0;
  padding: 4px;
  width: 40%;
  box-shadow: var(--jp-elevation-z4);
  border-radius: 4px;
  background: var(--jp-layout-color0);
}

.jp-ModalCommandPalette .lm-CommandPalette {
  max-height: 40vh;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-close-icon::after {
  display: none;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-CommandPalette-header {
  display: none;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-CommandPalette-item {
  margin-left: 4px;
  margin-right: 4px;
}

.jp-ModalCommandPalette
  .lm-CommandPalette
  .lm-CommandPalette-item.lm-mod-disabled {
  display: none;
}

/*-----------------------------------------------------------------------------
| Search
|----------------------------------------------------------------------------*/

.lm-CommandPalette-search {
  padding: 4px;
  background-color: var(--jp-layout-color1);
  z-index: 2;
}

.lm-CommandPalette-wrapper {
  overflow: overlay;
  padding: 0 9px;
  background-color: var(--jp-input-active-background);
  height: 30px;
  box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
}

.lm-CommandPalette.lm-mod-focused .lm-CommandPalette-wrapper {
  box-shadow: inset 0 0 0 1px var(--jp-input-active-box-shadow-color),
    inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.jp-SearchIconGroup {
  color: white;
  background-color: var(--jp-brand-color1);
  position: absolute;
  top: 4px;
  right: 4px;
  padding: 5px 5px 1px;
}

.jp-SearchIconGroup svg {
  height: 20px;
  width: 20px;
}

.jp-SearchIconGroup .jp-icon3[fill] {
  fill: var(--jp-layout-color0);
}

.lm-CommandPalette-input {
  background: transparent;
  width: calc(100% - 18px);
  float: left;
  border: none;
  outline: none;
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  line-height: var(--jp-private-commandpalette-search-height);
}

.lm-CommandPalette-input::-webkit-input-placeholder,
.lm-CommandPalette-input::-moz-placeholder,
.lm-CommandPalette-input:-ms-input-placeholder {
  color: var(--jp-ui-font-color2);
  font-size: var(--jp-ui-font-size1);
}

/*-----------------------------------------------------------------------------
| Results
|----------------------------------------------------------------------------*/

.lm-CommandPalette-header:first-child {
  margin-top: 0;
}

.lm-CommandPalette-header {
  border-bottom: solid var(--jp-border-width) var(--jp-border-color2);
  color: var(--jp-ui-font-color1);
  cursor: pointer;
  display: flex;
  font-size: var(--jp-ui-font-size0);
  font-weight: 600;
  letter-spacing: 1px;
  margin-top: 8px;
  padding: 8px 0 8px 12px;
  text-transform: uppercase;
}

.lm-CommandPalette-header.lm-mod-active {
  background: var(--jp-layout-color2);
}

.lm-CommandPalette-header > mark {
  background-color: transparent;
  font-weight: bold;
  color: var(--jp-ui-font-color1);
}

.lm-CommandPalette-item {
  padding: 4px 12px 4px 4px;
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  font-weight: 400;
  display: flex;
}

.lm-CommandPalette-item.lm-mod-disabled {
  color: var(--jp-ui-font-color2);
}

.lm-CommandPalette-item.lm-mod-active {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
}

.lm-CommandPalette-item.lm-mod-active .lm-CommandPalette-itemLabel > mark {
  color: var(--jp-ui-inverse-font-color0);
}

.lm-CommandPalette-item.lm-mod-active .jp-icon-selectable[fill] {
  fill: var(--jp-layout-color0);
}

.lm-CommandPalette-item.lm-mod-active:hover:not(.lm-mod-disabled) {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
}

.lm-CommandPalette-item:hover:not(.lm-mod-active):not(.lm-mod-disabled) {
  background: var(--jp-layout-color2);
}

.lm-CommandPalette-itemContent {
  overflow: hidden;
}

.lm-CommandPalette-itemLabel > mark {
  color: var(--jp-ui-font-color0);
  background-color: transparent;
  font-weight: bold;
}

.lm-CommandPalette-item.lm-mod-disabled mark {
  color: var(--jp-ui-font-color2);
}

.lm-CommandPalette-item .lm-CommandPalette-itemIcon {
  margin: 0 4px 0 0;
  position: relative;
  width: 16px;
  top: 2px;
  flex: 0 0 auto;
}

.lm-CommandPalette-item.lm-mod-disabled .lm-CommandPalette-itemIcon {
  opacity: 0.6;
}

.lm-CommandPalette-item .lm-CommandPalette-itemShortcut {
  flex: 0 0 auto;
}

.lm-CommandPalette-itemCaption {
  display: none;
}

.lm-CommandPalette-content {
  background-color: var(--jp-layout-color1);
}

.lm-CommandPalette-content:empty::after {
  content: 'No results';
  margin: auto;
  margin-top: 20px;
  width: 100px;
  display: block;
  font-size: var(--jp-ui-font-size2);
  font-family: var(--jp-ui-font-family);
  font-weight: lighter;
}

.lm-CommandPalette-emptyMessage {
  text-align: center;
  margin-top: 24px;
  line-height: 1.32;
  padding: 0 8px;
  color: var(--jp-content-font-color3);
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Dialog {
  position: absolute;
  z-index: 10000;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  top: 0;
  left: 0;
  margin: 0;
  padding: 0;
  width: 100%;
  height: 100%;
  background: var(--jp-dialog-background);
}

.jp-Dialog-content {
  display: flex;
  flex-direction: column;
  margin-left: auto;
  margin-right: auto;
  background: var(--jp-layout-color1);
  padding: 24px 24px 12px;
  min-width: 300px;
  min-height: 150px;
  max-width: 1000px;
  max-height: 500px;
  box-sizing: border-box;
  box-shadow: var(--jp-elevation-z20);
  word-wrap: break-word;
  border-radius: var(--jp-border-radius);

  /* This is needed so that all font sizing of children done in ems is
   * relative to this base size */
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color1);
  resize: both;
}

.jp-Dialog-content.jp-Dialog-content-small {
  max-width: 500px;
}

.jp-Dialog-button {
  overflow: visible;
}

button.jp-Dialog-button:focus {
  outline: 1px solid var(--jp-brand-color1);
  outline-offset: 4px;
  -moz-outline-radius: 0;
}

button.jp-Dialog-button:focus::-moz-focus-inner {
  border: 0;
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-accept:focus,
button.jp-Dialog-button.jp-mod-styled.jp-mod-warn:focus,
button.jp-Dialog-button.jp-mod-styled.jp-mod-reject:focus {
  outline-offset: 4px;
  -moz-outline-radius: 0;
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-accept:focus {
  outline: 1px solid var(--jp-accept-color-normal, var(--jp-brand-color1));
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-warn:focus {
  outline: 1px solid var(--jp-warn-color-normal, var(--jp-error-color1));
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-reject:focus {
  outline: 1px solid var(--jp-reject-color-normal, var(--md-grey-600));
}

button.jp-Dialog-close-button {
  padding: 0;
  height: 100%;
  min-width: unset;
  min-height: unset;
}

.jp-Dialog-header {
  display: flex;
  justify-content: space-between;
  flex: 0 0 auto;
  padding-bottom: 12px;
  font-size: var(--jp-ui-font-size3);
  font-weight: 400;
  color: var(--jp-ui-font-color1);
}

.jp-Dialog-body {
  display: flex;
  flex-direction: column;
  flex: 1 1 auto;
  font-size: var(--jp-ui-font-size1);
  background: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  overflow: auto;
}

.jp-Dialog-footer {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  align-items: center;
  flex: 0 0 auto;
  margin-left: -12px;
  margin-right: -12px;
  padding: 12px;
}

.jp-Dialog-checkbox {
  padding-right: 5px;
}

.jp-Dialog-checkbox > input:focus-visible {
  outline: 1px solid var(--jp-input-active-border-color);
  outline-offset: 1px;
}

.jp-Dialog-spacer {
  flex: 1 1 auto;
}

.jp-Dialog-title {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.jp-Dialog-body > .jp-select-wrapper {
  width: 100%;
}

.jp-Dialog-body > button {
  padding: 0 16px;
}

.jp-Dialog-body > label {
  line-height: 1.4;
  color: var(--jp-ui-font-color0);
}

.jp-Dialog-button.jp-mod-styled:not(:last-child) {
  margin-right: 12px;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-Input-Boolean-Dialog {
  flex-direction: row-reverse;
  align-items: end;
  width: 100%;
}

.jp-Input-Boolean-Dialog > label {
  flex: 1 1 auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-MainAreaWidget > :focus {
  outline: none;
}

.jp-MainAreaWidget .jp-MainAreaWidget-error {
  padding: 6px;
}

.jp-MainAreaWidget .jp-MainAreaWidget-error > pre {
  width: auto;
  padding: 10px;
  background: var(--jp-error-color3);
  border: var(--jp-border-width) solid var(--jp-error-color1);
  border-radius: var(--jp-border-radius);
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  white-space: pre-wrap;
  word-wrap: break-word;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/**
 * google-material-color v1.2.6
 * https://github.com/danlevan/google-material-color
 */
:root {
  --md-red-50: #ffebee;
  --md-red-100: #ffcdd2;
  --md-red-200: #ef9a9a;
  --md-red-300: #e57373;
  --md-red-400: #ef5350;
  --md-red-500: #f44336;
  --md-red-600: #e53935;
  --md-red-700: #d32f2f;
  --md-red-800: #c62828;
  --md-red-900: #b71c1c;
  --md-red-A100: #ff8a80;
  --md-red-A200: #ff5252;
  --md-red-A400: #ff1744;
  --md-red-A700: #d50000;
  --md-pink-50: #fce4ec;
  --md-pink-100: #f8bbd0;
  --md-pink-200: #f48fb1;
  --md-pink-300: #f06292;
  --md-pink-400: #ec407a;
  --md-pink-500: #e91e63;
  --md-pink-600: #d81b60;
  --md-pink-700: #c2185b;
  --md-pink-800: #ad1457;
  --md-pink-900: #880e4f;
  --md-pink-A100: #ff80ab;
  --md-pink-A200: #ff4081;
  --md-pink-A400: #f50057;
  --md-pink-A700: #c51162;
  --md-purple-50: #f3e5f5;
  --md-purple-100: #e1bee7;
  --md-purple-200: #ce93d8;
  --md-purple-300: #ba68c8;
  --md-purple-400: #ab47bc;
  --md-purple-500: #9c27b0;
  --md-purple-600: #8e24aa;
  --md-purple-700: #7b1fa2;
  --md-purple-800: #6a1b9a;
  --md-purple-900: #4a148c;
  --md-purple-A100: #ea80fc;
  --md-purple-A200: #e040fb;
  --md-purple-A400: #d500f9;
  --md-purple-A700: #a0f;
  --md-deep-purple-50: #ede7f6;
  --md-deep-purple-100: #d1c4e9;
  --md-deep-purple-200: #b39ddb;
  --md-deep-purple-300: #9575cd;
  --md-deep-purple-400: #7e57c2;
  --md-deep-purple-500: #673ab7;
  --md-deep-purple-600: #5e35b1;
  --md-deep-purple-700: #512da8;
  --md-deep-purple-800: #4527a0;
  --md-deep-purple-900: #311b92;
  --md-deep-purple-A100: #b388ff;
  --md-deep-purple-A200: #7c4dff;
  --md-deep-purple-A400: #651fff;
  --md-deep-purple-A700: #6200ea;
  --md-indigo-50: #e8eaf6;
  --md-indigo-100: #c5cae9;
  --md-indigo-200: #9fa8da;
  --md-indigo-300: #7986cb;
  --md-indigo-400: #5c6bc0;
  --md-indigo-500: #3f51b5;
  --md-indigo-600: #3949ab;
  --md-indigo-700: #303f9f;
  --md-indigo-800: #283593;
  --md-indigo-900: #1a237e;
  --md-indigo-A100: #8c9eff;
  --md-indigo-A200: #536dfe;
  --md-indigo-A400: #3d5afe;
  --md-indigo-A700: #304ffe;
  --md-blue-50: #e3f2fd;
  --md-blue-100: #bbdefb;
  --md-blue-200: #90caf9;
  --md-blue-300: #64b5f6;
  --md-blue-400: #42a5f5;
  --md-blue-500: #2196f3;
  --md-blue-600: #1e88e5;
  --md-blue-700: #1976d2;
  --md-blue-800: #1565c0;
  --md-blue-900: #0d47a1;
  --md-blue-A100: #82b1ff;
  --md-blue-A200: #448aff;
  --md-blue-A400: #2979ff;
  --md-blue-A700: #2962ff;
  --md-light-blue-50: #e1f5fe;
  --md-light-blue-100: #b3e5fc;
  --md-light-blue-200: #81d4fa;
  --md-light-blue-300: #4fc3f7;
  --md-light-blue-400: #29b6f6;
  --md-light-blue-500: #03a9f4;
  --md-light-blue-600: #039be5;
  --md-light-blue-700: #0288d1;
  --md-light-blue-800: #0277bd;
  --md-light-blue-900: #01579b;
  --md-light-blue-A100: #80d8ff;
  --md-light-blue-A200: #40c4ff;
  --md-light-blue-A400: #00b0ff;
  --md-light-blue-A700: #0091ea;
  --md-cyan-50: #e0f7fa;
  --md-cyan-100: #b2ebf2;
  --md-cyan-200: #80deea;
  --md-cyan-300: #4dd0e1;
  --md-cyan-400: #26c6da;
  --md-cyan-500: #00bcd4;
  --md-cyan-600: #00acc1;
  --md-cyan-700: #0097a7;
  --md-cyan-800: #00838f;
  --md-cyan-900: #006064;
  --md-cyan-A100: #84ffff;
  --md-cyan-A200: #18ffff;
  --md-cyan-A400: #00e5ff;
  --md-cyan-A700: #00b8d4;
  --md-teal-50: #e0f2f1;
  --md-teal-100: #b2dfdb;
  --md-teal-200: #80cbc4;
  --md-teal-300: #4db6ac;
  --md-teal-400: #26a69a;
  --md-teal-500: #009688;
  --md-teal-600: #00897b;
  --md-teal-700: #00796b;
  --md-teal-800: #00695c;
  --md-teal-900: #004d40;
  --md-teal-A100: #a7ffeb;
  --md-teal-A200: #64ffda;
  --md-teal-A400: #1de9b6;
  --md-teal-A700: #00bfa5;
  --md-green-50: #e8f5e9;
  --md-green-100: #c8e6c9;
  --md-green-200: #a5d6a7;
  --md-green-300: #81c784;
  --md-green-400: #66bb6a;
  --md-green-500: #4caf50;
  --md-green-600: #43a047;
  --md-green-700: #388e3c;
  --md-green-800: #2e7d32;
  --md-green-900: #1b5e20;
  --md-green-A100: #b9f6ca;
  --md-green-A200: #69f0ae;
  --md-green-A400: #00e676;
  --md-green-A700: #00c853;
  --md-light-green-50: #f1f8e9;
  --md-light-green-100: #dcedc8;
  --md-light-green-200: #c5e1a5;
  --md-light-green-300: #aed581;
  --md-light-green-400: #9ccc65;
  --md-light-green-500: #8bc34a;
  --md-light-green-600: #7cb342;
  --md-light-green-700: #689f38;
  --md-light-green-800: #558b2f;
  --md-light-green-900: #33691e;
  --md-light-green-A100: #ccff90;
  --md-light-green-A200: #b2ff59;
  --md-light-green-A400: #76ff03;
  --md-light-green-A700: #64dd17;
  --md-lime-50: #f9fbe7;
  --md-lime-100: #f0f4c3;
  --md-lime-200: #e6ee9c;
  --md-lime-300: #dce775;
  --md-lime-400: #d4e157;
  --md-lime-500: #cddc39;
  --md-lime-600: #c0ca33;
  --md-lime-700: #afb42b;
  --md-lime-800: #9e9d24;
  --md-lime-900: #827717;
  --md-lime-A100: #f4ff81;
  --md-lime-A200: #eeff41;
  --md-lime-A400: #c6ff00;
  --md-lime-A700: #aeea00;
  --md-yellow-50: #fffde7;
  --md-yellow-100: #fff9c4;
  --md-yellow-200: #fff59d;
  --md-yellow-300: #fff176;
  --md-yellow-400: #ffee58;
  --md-yellow-500: #ffeb3b;
  --md-yellow-600: #fdd835;
  --md-yellow-700: #fbc02d;
  --md-yellow-800: #f9a825;
  --md-yellow-900: #f57f17;
  --md-yellow-A100: #ffff8d;
  --md-yellow-A200: #ff0;
  --md-yellow-A400: #ffea00;
  --md-yellow-A700: #ffd600;
  --md-amber-50: #fff8e1;
  --md-amber-100: #ffecb3;
  --md-amber-200: #ffe082;
  --md-amber-300: #ffd54f;
  --md-amber-400: #ffca28;
  --md-amber-500: #ffc107;
  --md-amber-600: #ffb300;
  --md-amber-700: #ffa000;
  --md-amber-800: #ff8f00;
  --md-amber-900: #ff6f00;
  --md-amber-A100: #ffe57f;
  --md-amber-A200: #ffd740;
  --md-amber-A400: #ffc400;
  --md-amber-A700: #ffab00;
  --md-orange-50: #fff3e0;
  --md-orange-100: #ffe0b2;
  --md-orange-200: #ffcc80;
  --md-orange-300: #ffb74d;
  --md-orange-400: #ffa726;
  --md-orange-500: #ff9800;
  --md-orange-600: #fb8c00;
  --md-orange-700: #f57c00;
  --md-orange-800: #ef6c00;
  --md-orange-900: #e65100;
  --md-orange-A100: #ffd180;
  --md-orange-A200: #ffab40;
  --md-orange-A400: #ff9100;
  --md-orange-A700: #ff6d00;
  --md-deep-orange-50: #fbe9e7;
  --md-deep-orange-100: #ffccbc;
  --md-deep-orange-200: #ffab91;
  --md-deep-orange-300: #ff8a65;
  --md-deep-orange-400: #ff7043;
  --md-deep-orange-500: #ff5722;
  --md-deep-orange-600: #f4511e;
  --md-deep-orange-700: #e64a19;
  --md-deep-orange-800: #d84315;
  --md-deep-orange-900: #bf360c;
  --md-deep-orange-A100: #ff9e80;
  --md-deep-orange-A200: #ff6e40;
  --md-deep-orange-A400: #ff3d00;
  --md-deep-orange-A700: #dd2c00;
  --md-brown-50: #efebe9;
  --md-brown-100: #d7ccc8;
  --md-brown-200: #bcaaa4;
  --md-brown-300: #a1887f;
  --md-brown-400: #8d6e63;
  --md-brown-500: #795548;
  --md-brown-600: #6d4c41;
  --md-brown-700: #5d4037;
  --md-brown-800: #4e342e;
  --md-brown-900: #3e2723;
  --md-grey-50: #fafafa;
  --md-grey-100: #f5f5f5;
  --md-grey-200: #eee;
  --md-grey-300: #e0e0e0;
  --md-grey-400: #bdbdbd;
  --md-grey-500: #9e9e9e;
  --md-grey-600: #757575;
  --md-grey-700: #616161;
  --md-grey-800: #424242;
  --md-grey-900: #212121;
  --md-blue-grey-50: #eceff1;
  --md-blue-grey-100: #cfd8dc;
  --md-blue-grey-200: #b0bec5;
  --md-blue-grey-300: #90a4ae;
  --md-blue-grey-400: #78909c;
  --md-blue-grey-500: #607d8b;
  --md-blue-grey-600: #546e7a;
  --md-blue-grey-700: #455a64;
  --md-blue-grey-800: #37474f;
  --md-blue-grey-900: #263238;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| RenderedText
|----------------------------------------------------------------------------*/

:root {
  /* This is the padding value to fill the gaps between lines containing spans with background color. */
  --jp-private-code-span-padding: calc(
    (var(--jp-code-line-height) - 1) * var(--jp-code-font-size) / 2
  );
}

.jp-RenderedText {
  text-align: left;
  padding-left: var(--jp-code-padding);
  line-height: var(--jp-code-line-height);
  font-family: var(--jp-code-font-family);
}

.jp-RenderedText pre,
.jp-RenderedJavaScript pre,
.jp-RenderedHTMLCommon pre {
  color: var(--jp-content-font-color1);
  font-size: var(--jp-code-font-size);
  border: none;
  margin: 0;
  padding: 0;
}

.jp-RenderedText pre a:link {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

.jp-RenderedText pre a:hover {
  text-decoration: underline;
  color: var(--jp-content-link-color);
}

.jp-RenderedText pre a:visited {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

/* console foregrounds and backgrounds */
.jp-RenderedText pre .ansi-black-fg {
  color: #3e424d;
}

.jp-RenderedText pre .ansi-red-fg {
  color: #e75c58;
}

.jp-RenderedText pre .ansi-green-fg {
  color: #00a250;
}

.jp-RenderedText pre .ansi-yellow-fg {
  color: #ddb62b;
}

.jp-RenderedText pre .ansi-blue-fg {
  color: #208ffb;
}

.jp-RenderedText pre .ansi-magenta-fg {
  color: #d160c4;
}

.jp-RenderedText pre .ansi-cyan-fg {
  color: #60c6c8;
}

.jp-RenderedText pre .ansi-white-fg {
  color: #c5c1b4;
}

.jp-RenderedText pre .ansi-black-bg {
  background-color: #3e424d;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-red-bg {
  background-color: #e75c58;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-green-bg {
  background-color: #00a250;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-yellow-bg {
  background-color: #ddb62b;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-blue-bg {
  background-color: #208ffb;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-magenta-bg {
  background-color: #d160c4;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-cyan-bg {
  background-color: #60c6c8;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-white-bg {
  background-color: #c5c1b4;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-black-intense-fg {
  color: #282c36;
}

.jp-RenderedText pre .ansi-red-intense-fg {
  color: #b22b31;
}

.jp-RenderedText pre .ansi-green-intense-fg {
  color: #007427;
}

.jp-RenderedText pre .ansi-yellow-intense-fg {
  color: #b27d12;
}

.jp-RenderedText pre .ansi-blue-intense-fg {
  color: #0065ca;
}

.jp-RenderedText pre .ansi-magenta-intense-fg {
  color: #a03196;
}

.jp-RenderedText pre .ansi-cyan-intense-fg {
  color: #258f8f;
}

.jp-RenderedText pre .ansi-white-intense-fg {
  color: #a1a6b2;
}

.jp-RenderedText pre .ansi-black-intense-bg {
  background-color: #282c36;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-red-intense-bg {
  background-color: #b22b31;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-green-intense-bg {
  background-color: #007427;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-yellow-intense-bg {
  background-color: #b27d12;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-blue-intense-bg {
  background-color: #0065ca;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-magenta-intense-bg {
  background-color: #a03196;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-cyan-intense-bg {
  background-color: #258f8f;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-white-intense-bg {
  background-color: #a1a6b2;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-default-inverse-fg {
  color: var(--jp-ui-inverse-font-color0);
}

.jp-RenderedText pre .ansi-default-inverse-bg {
  background-color: var(--jp-inverse-layout-color0);
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-bold {
  font-weight: bold;
}

.jp-RenderedText pre .ansi-underline {
  text-decoration: underline;
}

.jp-RenderedText[data-mime-type='application/vnd.jupyter.stderr'] {
  background: var(--jp-rendermime-error-background);
  padding-top: var(--jp-code-padding);
}

/*-----------------------------------------------------------------------------
| RenderedLatex
|----------------------------------------------------------------------------*/

.jp-RenderedLatex {
  color: var(--jp-content-font-color1);
  font-size: var(--jp-content-font-size1);
  line-height: var(--jp-content-line-height);
}

/* Left-justify outputs.*/
.jp-OutputArea-output.jp-RenderedLatex {
  padding: var(--jp-code-padding);
  text-align: left;
}

/*-----------------------------------------------------------------------------
| RenderedHTML
|----------------------------------------------------------------------------*/

.jp-RenderedHTMLCommon {
  color: var(--jp-content-font-color1);
  font-family: var(--jp-content-font-family);
  font-size: var(--jp-content-font-size1);
  line-height: var(--jp-content-line-height);

  /* Give a bit more R padding on Markdown text to keep line lengths reasonable */
  padding-right: 20px;
}

.jp-RenderedHTMLCommon em {
  font-style: italic;
}

.jp-RenderedHTMLCommon strong {
  font-weight: bold;
}

.jp-RenderedHTMLCommon u {
  text-decoration: underline;
}

.jp-RenderedHTMLCommon a:link {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

.jp-RenderedHTMLCommon a:hover {
  text-decoration: underline;
  color: var(--jp-content-link-color);
}

.jp-RenderedHTMLCommon a:visited {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

/* Headings */

.jp-RenderedHTMLCommon h1,
.jp-RenderedHTMLCommon h2,
.jp-RenderedHTMLCommon h3,
.jp-RenderedHTMLCommon h4,
.jp-RenderedHTMLCommon h5,
.jp-RenderedHTMLCommon h6 {
  line-height: var(--jp-content-heading-line-height);
  font-weight: var(--jp-content-heading-font-weight);
  font-style: normal;
  margin: var(--jp-content-heading-margin-top) 0
    var(--jp-content-heading-margin-bottom) 0;
}

.jp-RenderedHTMLCommon h1:first-child,
.jp-RenderedHTMLCommon h2:first-child,
.jp-RenderedHTMLCommon h3:first-child,
.jp-RenderedHTMLCommon h4:first-child,
.jp-RenderedHTMLCommon h5:first-child,
.jp-RenderedHTMLCommon h6:first-child {
  margin-top: calc(0.5 * var(--jp-content-heading-margin-top));
}

.jp-RenderedHTMLCommon h1:last-child,
.jp-RenderedHTMLCommon h2:last-child,
.jp-RenderedHTMLCommon h3:last-child,
.jp-RenderedHTMLCommon h4:last-child,
.jp-RenderedHTMLCommon h5:last-child,
.jp-RenderedHTMLCommon h6:last-child {
  margin-bottom: calc(0.5 * var(--jp-content-heading-margin-bottom));
}

.jp-RenderedHTMLCommon h1 {
  font-size: var(--jp-content-font-size5);
}

.jp-RenderedHTMLCommon h2 {
  font-size: var(--jp-content-font-size4);
}

.jp-RenderedHTMLCommon h3 {
  font-size: var(--jp-content-font-size3);
}

.jp-RenderedHTMLCommon h4 {
  font-size: var(--jp-content-font-size2);
}

.jp-RenderedHTMLCommon h5 {
  font-size: var(--jp-content-font-size1);
}

.jp-RenderedHTMLCommon h6 {
  font-size: var(--jp-content-font-size0);
}

/* Lists */

/* stylelint-disable selector-max-type, selector-max-compound-selectors */

.jp-RenderedHTMLCommon ul:not(.list-inline),
.jp-RenderedHTMLCommon ol:not(.list-inline) {
  padding-left: 2em;
}

.jp-RenderedHTMLCommon ul {
  list-style: disc;
}

.jp-RenderedHTMLCommon ul ul {
  list-style: square;
}

.jp-RenderedHTMLCommon ul ul ul {
  list-style: circle;
}

.jp-RenderedHTMLCommon ol {
  list-style: decimal;
}

.jp-RenderedHTMLCommon ol ol {
  list-style: upper-alpha;
}

.jp-RenderedHTMLCommon ol ol ol {
  list-style: lower-alpha;
}

.jp-RenderedHTMLCommon ol ol ol ol {
  list-style: lower-roman;
}

.jp-RenderedHTMLCommon ol ol ol ol ol {
  list-style: decimal;
}

.jp-RenderedHTMLCommon ol,
.jp-RenderedHTMLCommon ul {
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon ul ul,
.jp-RenderedHTMLCommon ul ol,
.jp-RenderedHTMLCommon ol ul,
.jp-RenderedHTMLCommon ol ol {
  margin-bottom: 0;
}

/* stylelint-enable selector-max-type, selector-max-compound-selectors */

.jp-RenderedHTMLCommon hr {
  color: var(--jp-border-color2);
  background-color: var(--jp-border-color1);
  margin-top: 1em;
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon > pre {
  margin: 1.5em 2em;
}

.jp-RenderedHTMLCommon pre,
.jp-RenderedHTMLCommon code {
  border: 0;
  background-color: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
  font-family: var(--jp-code-font-family);
  font-size: inherit;
  line-height: var(--jp-code-line-height);
  padding: 0;
  white-space: pre-wrap;
}

.jp-RenderedHTMLCommon :not(pre) > code {
  background-color: var(--jp-layout-color2);
  padding: 1px 5px;
}

/* Tables */

.jp-RenderedHTMLCommon table {
  border-collapse: collapse;
  border-spacing: 0;
  border: none;
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  table-layout: fixed;
  margin-left: auto;
  margin-bottom: 1em;
  margin-right: auto;
}

.jp-RenderedHTMLCommon thead {
  border-bottom: var(--jp-border-width) solid var(--jp-border-color1);
  vertical-align: bottom;
}

.jp-RenderedHTMLCommon td,
.jp-RenderedHTMLCommon th,
.jp-RenderedHTMLCommon tr {
  vertical-align: middle;
  padding: 0.5em;
  line-height: normal;
  white-space: normal;
  max-width: none;
  border: none;
}

.jp-RenderedMarkdown.jp-RenderedHTMLCommon td,
.jp-RenderedMarkdown.jp-RenderedHTMLCommon th {
  max-width: none;
}

:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon td,
:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon th,
:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon tr {
  text-align: right;
}

.jp-RenderedHTMLCommon th {
  font-weight: bold;
}

.jp-RenderedHTMLCommon tbody tr:nth-child(odd) {
  background: var(--jp-layout-color0);
}

.jp-RenderedHTMLCommon tbody tr:nth-child(even) {
  background: var(--jp-rendermime-table-row-background);
}

.jp-RenderedHTMLCommon tbody tr:hover {
  background: var(--jp-rendermime-table-row-hover-background);
}

.jp-RenderedHTMLCommon p {
  text-align: left;
  margin: 0;
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon img {
  -moz-force-broken-image-icon: 1;
}

/* Restrict to direct children as other images could be nested in other content. */
.jp-RenderedHTMLCommon > img {
  display: block;
  margin-left: 0;
  margin-right: 0;
  margin-bottom: 1em;
}

/* Change color behind transparent images if they need it... */
[data-jp-theme-light='false'] .jp-RenderedImage img.jp-needs-light-background {
  background-color: var(--jp-inverse-layout-color1);
}

[data-jp-theme-light='true'] .jp-RenderedImage img.jp-needs-dark-background {
  background-color: var(--jp-inverse-layout-color1);
}

.jp-RenderedHTMLCommon img,
.jp-RenderedImage img,
.jp-RenderedHTMLCommon svg,
.jp-RenderedSVG svg {
  max-width: 100%;
  height: auto;
}

.jp-RenderedHTMLCommon img.jp-mod-unconfined,
.jp-RenderedImage img.jp-mod-unconfined,
.jp-RenderedHTMLCommon svg.jp-mod-unconfined,
.jp-RenderedSVG svg.jp-mod-unconfined {
  max-width: none;
}

.jp-RenderedHTMLCommon .alert {
  padding: var(--jp-notebook-padding);
  border: var(--jp-border-width) solid transparent;
  border-radius: var(--jp-border-radius);
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon .alert-info {
  color: var(--jp-info-color0);
  background-color: var(--jp-info-color3);
  border-color: var(--jp-info-color2);
}

.jp-RenderedHTMLCommon .alert-info hr {
  border-color: var(--jp-info-color3);
}

.jp-RenderedHTMLCommon .alert-info > p:last-child,
.jp-RenderedHTMLCommon .alert-info > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-warning {
  color: var(--jp-warn-color0);
  background-color: var(--jp-warn-color3);
  border-color: var(--jp-warn-color2);
}

.jp-RenderedHTMLCommon .alert-warning hr {
  border-color: var(--jp-warn-color3);
}

.jp-RenderedHTMLCommon .alert-warning > p:last-child,
.jp-RenderedHTMLCommon .alert-warning > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-success {
  color: var(--jp-success-color0);
  background-color: var(--jp-success-color3);
  border-color: var(--jp-success-color2);
}

.jp-RenderedHTMLCommon .alert-success hr {
  border-color: var(--jp-success-color3);
}

.jp-RenderedHTMLCommon .alert-success > p:last-child,
.jp-RenderedHTMLCommon .alert-success > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-danger {
  color: var(--jp-error-color0);
  background-color: var(--jp-error-color3);
  border-color: var(--jp-error-color2);
}

.jp-RenderedHTMLCommon .alert-danger hr {
  border-color: var(--jp-error-color3);
}

.jp-RenderedHTMLCommon .alert-danger > p:last-child,
.jp-RenderedHTMLCommon .alert-danger > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon blockquote {
  margin: 1em 2em;
  padding: 0 1em;
  border-left: 5px solid var(--jp-border-color2);
}

a.jp-InternalAnchorLink {
  visibility: hidden;
  margin-left: 8px;
  color: var(--md-blue-800);
}

h1:hover .jp-InternalAnchorLink,
h2:hover .jp-InternalAnchorLink,
h3:hover .jp-InternalAnchorLink,
h4:hover .jp-InternalAnchorLink,
h5:hover .jp-InternalAnchorLink,
h6:hover .jp-InternalAnchorLink {
  visibility: visible;
}

.jp-RenderedHTMLCommon kbd {
  background-color: var(--jp-rendermime-table-row-background);
  border: 1px solid var(--jp-border-color0);
  border-bottom-color: var(--jp-border-color2);
  border-radius: 3px;
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.25);
  display: inline-block;
  font-size: var(--jp-ui-font-size0);
  line-height: 1em;
  padding: 0.2em 0.5em;
}

/* Most direct children of .jp-RenderedHTMLCommon have a margin-bottom of 1.0.
 * At the bottom of cells this is a bit too much as there is also spacing
 * between cells. Going all the way to 0 gets too tight between markdown and
 * code cells.
 */
.jp-RenderedHTMLCommon > *:last-child {
  margin-bottom: 0.5em;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-cursor-backdrop {
  position: fixed;
  width: 200px;
  height: 200px;
  margin-top: -100px;
  margin-left: -100px;
  will-change: transform;
  z-index: 100;
}

.lm-mod-drag-image {
  will-change: transform;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-lineFormSearch {
  padding: 4px 12px;
  background-color: var(--jp-layout-color2);
  box-shadow: var(--jp-toolbar-box-shadow);
  z-index: 2;
  font-size: var(--jp-ui-font-size1);
}

.jp-lineFormCaption {
  font-size: var(--jp-ui-font-size0);
  line-height: var(--jp-ui-font-size1);
  margin-top: 4px;
  color: var(--jp-ui-font-color0);
}

.jp-baseLineForm {
  border: none;
  border-radius: 0;
  position: absolute;
  background-size: 16px;
  background-repeat: no-repeat;
  background-position: center;
  outline: none;
}

.jp-lineFormButtonContainer {
  top: 4px;
  right: 8px;
  height: 24px;
  padding: 0 12px;
  width: 12px;
}

.jp-lineFormButtonIcon {
  top: 0;
  right: 0;
  background-color: var(--jp-brand-color1);
  height: 100%;
  width: 100%;
  box-sizing: border-box;
  padding: 4px 6px;
}

.jp-lineFormButton {
  top: 0;
  right: 0;
  background-color: transparent;
  height: 100%;
  width: 100%;
  box-sizing: border-box;
}

.jp-lineFormWrapper {
  overflow: hidden;
  padding: 0 8px;
  border: 1px solid var(--jp-border-color0);
  background-color: var(--jp-input-active-background);
  height: 22px;
}

.jp-lineFormWrapperFocusWithin {
  border: var(--jp-border-width) solid var(--md-blue-500);
  box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-lineFormInput {
  background: transparent;
  width: 200px;
  height: 100%;
  border: none;
  outline: none;
  color: var(--jp-ui-font-color0);
  line-height: 28px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-JSONEditor {
  display: flex;
  flex-direction: column;
  width: 100%;
}

.jp-JSONEditor-host {
  flex: 1 1 auto;
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  border-radius: 0;
  background: var(--jp-layout-color0);
  min-height: 50px;
  padding: 1px;
}

.jp-JSONEditor.jp-mod-error .jp-JSONEditor-host {
  border-color: red;
  outline-color: red;
}

.jp-JSONEditor-header {
  display: flex;
  flex: 1 0 auto;
  padding: 0 0 0 12px;
}

.jp-JSONEditor-header label {
  flex: 0 0 auto;
}

.jp-JSONEditor-commitButton {
  height: 16px;
  width: 16px;
  background-size: 18px;
  background-repeat: no-repeat;
  background-position: center;
}

.jp-JSONEditor-host.jp-mod-focused {
  background-color: var(--jp-input-active-background);
  border: 1px solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
}

.jp-Editor.jp-mod-dropTarget {
  border: var(--jp-border-width) solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/
.jp-DocumentSearch-input {
  border: none;
  outline: none;
  color: var(--jp-ui-font-color0);
  font-size: var(--jp-ui-font-size1);
  background-color: var(--jp-layout-color0);
  font-family: var(--jp-ui-font-family);
  padding: 2px 1px;
  resize: none;
}

.jp-DocumentSearch-overlay {
  position: absolute;
  background-color: var(--jp-toolbar-background);
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  border-left: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  top: 0;
  right: 0;
  z-index: 7;
  min-width: 405px;
  padding: 2px;
  font-size: var(--jp-ui-font-size1);

  --jp-private-document-search-button-height: 20px;
}

.jp-DocumentSearch-overlay button {
  background-color: var(--jp-toolbar-background);
  outline: 0;
}

.jp-DocumentSearch-overlay button:hover {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-overlay button:active {
  background-color: var(--jp-layout-color3);
}

.jp-DocumentSearch-overlay-row {
  display: flex;
  align-items: center;
  margin-bottom: 2px;
}

.jp-DocumentSearch-button-content {
  display: inline-block;
  cursor: pointer;
  box-sizing: border-box;
  width: 100%;
  height: 100%;
}

.jp-DocumentSearch-button-content svg {
  width: 100%;
  height: 100%;
}

.jp-DocumentSearch-input-wrapper {
  border: var(--jp-border-width) solid var(--jp-border-color0);
  display: flex;
  background-color: var(--jp-layout-color0);
  margin: 2px;
}

.jp-DocumentSearch-input-wrapper:focus-within {
  border-color: var(--jp-cell-editor-active-border-color);
}

.jp-DocumentSearch-toggle-wrapper,
.jp-DocumentSearch-button-wrapper {
  all: initial;
  overflow: hidden;
  display: inline-block;
  border: none;
  box-sizing: border-box;
}

.jp-DocumentSearch-toggle-wrapper {
  width: 14px;
  height: 14px;
}

.jp-DocumentSearch-button-wrapper {
  width: var(--jp-private-document-search-button-height);
  height: var(--jp-private-document-search-button-height);
}

.jp-DocumentSearch-toggle-wrapper:focus,
.jp-DocumentSearch-button-wrapper:focus {
  outline: var(--jp-border-width) solid
    var(--jp-cell-editor-active-border-color);
  outline-offset: -1px;
}

.jp-DocumentSearch-toggle-wrapper,
.jp-DocumentSearch-button-wrapper,
.jp-DocumentSearch-button-content:focus {
  outline: none;
}

.jp-DocumentSearch-toggle-placeholder {
  width: 5px;
}

.jp-DocumentSearch-input-button::before {
  display: block;
  padding-top: 100%;
}

.jp-DocumentSearch-input-button-off {
  opacity: var(--jp-search-toggle-off-opacity);
}

.jp-DocumentSearch-input-button-off:hover {
  opacity: var(--jp-search-toggle-hover-opacity);
}

.jp-DocumentSearch-input-button-on {
  opacity: var(--jp-search-toggle-on-opacity);
}

.jp-DocumentSearch-index-counter {
  padding-left: 10px;
  padding-right: 10px;
  user-select: none;
  min-width: 35px;
  display: inline-block;
}

.jp-DocumentSearch-up-down-wrapper {
  display: inline-block;
  padding-right: 2px;
  margin-left: auto;
  white-space: nowrap;
}

.jp-DocumentSearch-spacer {
  margin-left: auto;
}

.jp-DocumentSearch-up-down-wrapper button {
  outline: 0;
  border: none;
  width: var(--jp-private-document-search-button-height);
  height: var(--jp-private-document-search-button-height);
  vertical-align: middle;
  margin: 1px 5px 2px;
}

.jp-DocumentSearch-up-down-button:hover {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-up-down-button:active {
  background-color: var(--jp-layout-color3);
}

.jp-DocumentSearch-filter-button {
  border-radius: var(--jp-border-radius);
}

.jp-DocumentSearch-filter-button:hover {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-filter-button-enabled {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-filter-button-enabled:hover {
  background-color: var(--jp-layout-color3);
}

.jp-DocumentSearch-search-options {
  padding: 0 8px;
  margin-left: 3px;
  width: 100%;
  display: grid;
  justify-content: start;
  grid-template-columns: 1fr 1fr;
  align-items: center;
  justify-items: stretch;
}

.jp-DocumentSearch-search-filter-disabled {
  color: var(--jp-ui-font-color2);
}

.jp-DocumentSearch-search-filter {
  display: flex;
  align-items: center;
  user-select: none;
}

.jp-DocumentSearch-regex-error {
  color: var(--jp-error-color0);
}

.jp-DocumentSearch-replace-button-wrapper {
  overflow: hidden;
  display: inline-block;
  box-sizing: border-box;
  border: var(--jp-border-width) solid var(--jp-border-color0);
  margin: auto 2px;
  padding: 1px 4px;
  height: calc(var(--jp-private-document-search-button-height) + 2px);
}

.jp-DocumentSearch-replace-button-wrapper:focus {
  border: var(--jp-border-width) solid var(--jp-cell-editor-active-border-color);
}

.jp-DocumentSearch-replace-button {
  display: inline-block;
  text-align: center;
  cursor: pointer;
  box-sizing: border-box;
  color: var(--jp-ui-font-color1);

  /* height - 2 * (padding of wrapper) */
  line-height: calc(var(--jp-private-document-search-button-height) - 2px);
  width: 100%;
  height: 100%;
}

.jp-DocumentSearch-replace-button:focus {
  outline: none;
}

.jp-DocumentSearch-replace-wrapper-class {
  margin-left: 14px;
  display: flex;
}

.jp-DocumentSearch-replace-toggle {
  border: none;
  background-color: var(--jp-toolbar-background);
  border-radius: var(--jp-border-radius);
}

.jp-DocumentSearch-replace-toggle:hover {
  background-color: var(--jp-layout-color2);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.cm-editor {
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  font-family: var(--jp-code-font-family);
  border: 0;
  border-radius: 0;
  height: auto;

  /* Changed to auto to autogrow */
}

.cm-editor pre {
  padding: 0 var(--jp-code-padding);
}

.jp-CodeMirrorEditor[data-type='inline'] .cm-dialog {
  background-color: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
}

.jp-CodeMirrorEditor {
  cursor: text;
}

/* When zoomed out 67% and 33% on a screen of 1440 width x 900 height */
@media screen and (min-width: 2138px) and (max-width: 4319px) {
  .jp-CodeMirrorEditor[data-type='inline'] .cm-cursor {
    border-left: var(--jp-code-cursor-width1) solid
      var(--jp-editor-cursor-color);
  }
}

/* When zoomed out less than 33% */
@media screen and (min-width: 4320px) {
  .jp-CodeMirrorEditor[data-type='inline'] .cm-cursor {
    border-left: var(--jp-code-cursor-width2) solid
      var(--jp-editor-cursor-color);
  }
}

.cm-editor.jp-mod-readOnly .cm-cursor {
  display: none;
}

.jp-CollaboratorCursor {
  border-left: 5px solid transparent;
  border-right: 5px solid transparent;
  border-top: none;
  border-bottom: 3px solid;
  background-clip: content-box;
  margin-left: -5px;
  margin-right: -5px;
}

.cm-searching,
.cm-searching span {
  /* `.cm-searching span`: we need to override syntax highlighting */
  background-color: var(--jp-search-unselected-match-background-color);
  color: var(--jp-search-unselected-match-color);
}

.cm-searching::selection,
.cm-searching span::selection {
  background-color: var(--jp-search-unselected-match-background-color);
  color: var(--jp-search-unselected-match-color);
}

.jp-current-match > .cm-searching,
.jp-current-match > .cm-searching span,
.cm-searching > .jp-current-match,
.cm-searching > .jp-current-match span {
  background-color: var(--jp-search-selected-match-background-color);
  color: var(--jp-search-selected-match-color);
}

.jp-current-match > .cm-searching::selection,
.cm-searching > .jp-current-match::selection,
.jp-current-match > .cm-searching span::selection {
  background-color: var(--jp-search-selected-match-background-color);
  color: var(--jp-search-selected-match-color);
}

.cm-trailingspace {
  background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAgAAAAFCAYAAAB4ka1VAAAAsElEQVQIHQGlAFr/AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA7+r3zKmT0/+pk9P/7+r3zAAAAAAAAAAABAAAAAAAAAAA6OPzM+/q9wAAAAAA6OPzMwAAAAAAAAAAAgAAAAAAAAAAGR8NiRQaCgAZIA0AGR8NiQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAQyoYJ/SY80UAAAAASUVORK5CYII=);
  background-position: center left;
  background-repeat: repeat-x;
}

.jp-CollaboratorCursor-hover {
  position: absolute;
  z-index: 1;
  transform: translateX(-50%);
  color: white;
  border-radius: 3px;
  padding-left: 4px;
  padding-right: 4px;
  padding-top: 1px;
  padding-bottom: 1px;
  text-align: center;
  font-size: var(--jp-ui-font-size1);
  white-space: nowrap;
}

.jp-CodeMirror-ruler {
  border-left: 1px dashed var(--jp-border-color2);
}

/* Styles for shared cursors (remote cursor locations and selected ranges) */
.jp-CodeMirrorEditor .cm-ySelectionCaret {
  position: relative;
  border-left: 1px solid black;
  margin-left: -1px;
  margin-right: -1px;
  box-sizing: border-box;
}

.jp-CodeMirrorEditor .cm-ySelectionCaret > .cm-ySelectionInfo {
  white-space: nowrap;
  position: absolute;
  top: -1.15em;
  padding-bottom: 0.05em;
  left: -1px;
  font-size: 0.95em;
  font-family: var(--jp-ui-font-family);
  font-weight: bold;
  line-height: normal;
  user-select: none;
  color: white;
  padding-left: 2px;
  padding-right: 2px;
  z-index: 101;
  transition: opacity 0.3s ease-in-out;
}

.jp-CodeMirrorEditor .cm-ySelectionInfo {
  transition-delay: 0.7s;
  opacity: 0;
}

.jp-CodeMirrorEditor .cm-ySelectionCaret:hover > .cm-ySelectionInfo {
  opacity: 1;
  transition-delay: 0s;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-MimeDocument {
  outline: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-filebrowser-button-height: 28px;
  --jp-private-filebrowser-button-width: 48px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-FileBrowser .jp-SidePanel-content {
  display: flex;
  flex-direction: column;
}

.jp-FileBrowser-toolbar.jp-Toolbar {
  flex-wrap: wrap;
  row-gap: 12px;
  border-bottom: none;
  height: auto;
  margin: 8px 12px 0;
  box-shadow: none;
  padding: 0;
  justify-content: flex-start;
}

.jp-FileBrowser-Panel {
  flex: 1 1 auto;
  display: flex;
  flex-direction: column;
}

.jp-BreadCrumbs {
  flex: 0 0 auto;
  margin: 8px 12px;
}

.jp-BreadCrumbs-item {
  margin: 0 2px;
  padding: 0 2px;
  border-radius: var(--jp-border-radius);
  cursor: pointer;
}

.jp-BreadCrumbs-item:hover {
  background-color: var(--jp-layout-color2);
}

.jp-BreadCrumbs-item:first-child {
  margin-left: 0;
}

.jp-BreadCrumbs-item.jp-mod-dropTarget {
  background-color: var(--jp-brand-color2);
  opacity: 0.7;
}

/*-----------------------------------------------------------------------------
| Buttons
|----------------------------------------------------------------------------*/

.jp-FileBrowser-toolbar > .jp-Toolbar-item {
  flex: 0 0 auto;
  padding-left: 0;
  padding-right: 2px;
  align-items: center;
  height: unset;
}

.jp-FileBrowser-toolbar > .jp-Toolbar-item .jp-ToolbarButtonComponent {
  width: 40px;
}

/*-----------------------------------------------------------------------------
| Other styles
|----------------------------------------------------------------------------*/

.jp-FileDialog.jp-mod-conflict input {
  color: var(--jp-error-color1);
}

.jp-FileDialog .jp-new-name-title {
  margin-top: 12px;
}

.jp-LastModified-hidden {
  display: none;
}

.jp-FileSize-hidden {
  display: none;
}

.jp-FileBrowser .lm-AccordionPanel > h3:first-child {
  display: none;
}

/*-----------------------------------------------------------------------------
| DirListing
|----------------------------------------------------------------------------*/

.jp-DirListing {
  flex: 1 1 auto;
  display: flex;
  flex-direction: column;
  outline: 0;
}

.jp-DirListing-header {
  flex: 0 0 auto;
  display: flex;
  flex-direction: row;
  align-items: center;
  overflow: hidden;
  border-top: var(--jp-border-width) solid var(--jp-border-color2);
  border-bottom: var(--jp-border-width) solid var(--jp-border-color1);
  box-shadow: var(--jp-toolbar-box-shadow);
  z-index: 2;
}

.jp-DirListing-headerItem {
  padding: 4px 12px 2px;
  font-weight: 500;
}

.jp-DirListing-headerItem:hover {
  background: var(--jp-layout-color2);
}

.jp-DirListing-headerItem.jp-id-name {
  flex: 1 0 84px;
}

.jp-DirListing-headerItem.jp-id-modified {
  flex: 0 0 112px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
}

.jp-DirListing-headerItem.jp-id-filesize {
  flex: 0 0 75px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
}

.jp-id-narrow {
  display: none;
  flex: 0 0 5px;
  padding: 4px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
  color: var(--jp-border-color2);
}

.jp-DirListing-narrow .jp-id-narrow {
  display: block;
}

.jp-DirListing-narrow .jp-id-modified,
.jp-DirListing-narrow .jp-DirListing-itemModified {
  display: none;
}

.jp-DirListing-headerItem.jp-mod-selected {
  font-weight: 600;
}

/* increase specificity to override bundled default */
.jp-DirListing-content {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  list-style-type: none;
  overflow: auto;
  background-color: var(--jp-layout-color1);
}

.jp-DirListing-content mark {
  color: var(--jp-ui-font-color0);
  background-color: transparent;
  font-weight: bold;
}

.jp-DirListing-content .jp-DirListing-item.jp-mod-selected mark {
  color: var(--jp-ui-inverse-font-color0);
}

/* Style the directory listing content when a user drops a file to upload */
.jp-DirListing.jp-mod-native-drop .jp-DirListing-content {
  outline: 5px dashed rgba(128, 128, 128, 0.5);
  outline-offset: -10px;
  cursor: copy;
}

.jp-DirListing-item {
  display: flex;
  flex-direction: row;
  align-items: center;
  padding: 4px 12px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-DirListing-checkboxWrapper {
  /* Increases hit area of checkbox. */
  padding: 4px;
}

.jp-DirListing-header
  .jp-DirListing-checkboxWrapper
  + .jp-DirListing-headerItem {
  padding-left: 4px;
}

.jp-DirListing-content .jp-DirListing-checkboxWrapper {
  position: relative;
  left: -4px;
  margin: -4px 0 -4px -8px;
}

.jp-DirListing-checkboxWrapper.jp-mod-visible {
  visibility: visible;
}

/* For devices that support hovering, hide checkboxes until hovered, selected...
*/
@media (hover: hover) {
  .jp-DirListing-checkboxWrapper {
    visibility: hidden;
  }

  .jp-DirListing-item:hover .jp-DirListing-checkboxWrapper,
  .jp-DirListing-item.jp-mod-selected .jp-DirListing-checkboxWrapper {
    visibility: visible;
  }
}

.jp-DirListing-item[data-is-dot] {
  opacity: 75%;
}

.jp-DirListing-item.jp-mod-selected {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
}

.jp-DirListing-item.jp-mod-dropTarget {
  background: var(--jp-brand-color3);
}

.jp-DirListing-item:hover:not(.jp-mod-selected) {
  background: var(--jp-layout-color2);
}

.jp-DirListing-itemIcon {
  flex: 0 0 20px;
  margin-right: 4px;
}

.jp-DirListing-itemText {
  flex: 1 0 64px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  user-select: none;
}

.jp-DirListing-itemText:focus {
  outline-width: 2px;
  outline-color: var(--jp-inverse-layout-color1);
  outline-style: solid;
  outline-offset: 1px;
}

.jp-DirListing-item.jp-mod-selected .jp-DirListing-itemText:focus {
  outline-color: var(--jp-layout-color1);
}

.jp-DirListing-itemModified {
  flex: 0 0 125px;
  text-align: right;
}

.jp-DirListing-itemFileSize {
  flex: 0 0 90px;
  text-align: right;
}

.jp-DirListing-editor {
  flex: 1 0 64px;
  outline: none;
  border: none;
  color: var(--jp-ui-font-color1);
  background-color: var(--jp-layout-color1);
}

.jp-DirListing-item.jp-mod-running .jp-DirListing-itemIcon::before {
  color: var(--jp-success-color1);
  content: '\25CF';
  font-size: 8px;
  position: absolute;
  left: -8px;
}

.jp-DirListing-item.jp-mod-running.jp-mod-selected
  .jp-DirListing-itemIcon::before {
  color: var(--jp-ui-inverse-font-color1);
}

.jp-DirListing-item.lm-mod-drag-image,
.jp-DirListing-item.jp-mod-selected.lm-mod-drag-image {
  font-size: var(--jp-ui-font-size1);
  padding-left: 4px;
  margin-left: 4px;
  width: 160px;
  background-color: var(--jp-ui-inverse-font-color2);
  box-shadow: var(--jp-elevation-z2);
  border-radius: 0;
  color: var(--jp-ui-font-color1);
  transform: translateX(-40%) translateY(-58%);
}

.jp-Document {
  min-width: 120px;
  min-height: 120px;
  outline: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Main OutputArea
| OutputArea has a list of Outputs
|----------------------------------------------------------------------------*/

.jp-OutputArea {
  overflow-y: auto;
}

.jp-OutputArea-child {
  display: table;
  table-layout: fixed;
  width: 100%;
  overflow: hidden;
}

.jp-OutputPrompt {
  width: var(--jp-cell-prompt-width);
  color: var(--jp-cell-outprompt-font-color);
  font-family: var(--jp-cell-prompt-font-family);
  padding: var(--jp-code-padding);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;
  opacity: var(--jp-cell-prompt-opacity);

  /* Right align prompt text, don't wrap to handle large prompt numbers */
  text-align: right;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;

  /* Disable text selection */
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-OutputArea-prompt {
  display: table-cell;
  vertical-align: top;
}

.jp-OutputArea-output {
  display: table-cell;
  width: 100%;
  height: auto;
  overflow: auto;
  user-select: text;
  -moz-user-select: text;
  -webkit-user-select: text;
  -ms-user-select: text;
}

.jp-OutputArea .jp-RenderedText {
  padding-left: 1ch;
}

/**
 * Prompt overlay.
 */

.jp-OutputArea-promptOverlay {
  position: absolute;
  top: 0;
  width: var(--jp-cell-prompt-width);
  height: 100%;
  opacity: 0.5;
}

.jp-OutputArea-promptOverlay:hover {
  background: var(--jp-layout-color2);
  box-shadow: inset 0 0 1px var(--jp-inverse-layout-color0);
  cursor: zoom-out;
}

.jp-mod-outputsScrolled .jp-OutputArea-promptOverlay:hover {
  cursor: zoom-in;
}

/**
 * Isolated output.
 */
.jp-OutputArea-output.jp-mod-isolated {
  width: 100%;
  display: block;
}

/*
When drag events occur, `lm-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated {
  position: relative;
}

body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: transparent;
}

/* pre */

.jp-OutputArea-output pre {
  border: none;
  margin: 0;
  padding: 0;
  overflow-x: auto;
  overflow-y: auto;
  word-break: break-all;
  word-wrap: break-word;
  white-space: pre-wrap;
}

/* tables */

.jp-OutputArea-output.jp-RenderedHTMLCommon table {
  margin-left: 0;
  margin-right: 0;
}

/* description lists */

.jp-OutputArea-output dl,
.jp-OutputArea-output dt,
.jp-OutputArea-output dd {
  display: block;
}

.jp-OutputArea-output dl {
  width: 100%;
  overflow: hidden;
  padding: 0;
  margin: 0;
}

.jp-OutputArea-output dt {
  font-weight: bold;
  float: left;
  width: 20%;
  padding: 0;
  margin: 0;
}

.jp-OutputArea-output dd {
  float: left;
  width: 80%;
  padding: 0;
  margin: 0;
}

.jp-TrimmedOutputs pre {
  background: var(--jp-layout-color3);
  font-size: calc(var(--jp-code-font-size) * 1.4);
  text-align: center;
  text-transform: uppercase;
}

/* Hide the gutter in case of
 *  - nested output areas (e.g. in the case of output widgets)
 *  - mirrored output areas
 */
.jp-OutputArea .jp-OutputArea .jp-OutputArea-prompt {
  display: none;
}

/* Hide empty lines in the output area, for instance due to cleared widgets */
.jp-OutputArea-prompt:empty {
  padding: 0;
  border: 0;
}

/*-----------------------------------------------------------------------------
| executeResult is added to any Output-result for the display of the object
| returned by a cell
|----------------------------------------------------------------------------*/

.jp-OutputArea-output.jp-OutputArea-executeResult {
  margin-left: 0;
  width: 100%;
}

/* Text output with the Out[] prompt needs a top padding to match the
 * alignment of the Out[] prompt itself.
 */
.jp-OutputArea-executeResult .jp-RenderedText.jp-OutputArea-output {
  padding-top: var(--jp-code-padding);
  border-top: var(--jp-border-width) solid transparent;
}

/*-----------------------------------------------------------------------------
| The Stdin output
|----------------------------------------------------------------------------*/

.jp-Stdin-prompt {
  color: var(--jp-content-font-color0);
  padding-right: var(--jp-code-padding);
  vertical-align: baseline;
  flex: 0 0 auto;
}

.jp-Stdin-input {
  font-family: var(--jp-code-font-family);
  font-size: inherit;
  color: inherit;
  background-color: inherit;
  width: 42%;
  min-width: 200px;

  /* make sure input baseline aligns with prompt */
  vertical-align: baseline;

  /* padding + margin = 0.5em between prompt and cursor */
  padding: 0 0.25em;
  margin: 0 0.25em;
  flex: 0 0 70%;
}

.jp-Stdin-input::placeholder {
  opacity: 0;
}

.jp-Stdin-input:focus {
  box-shadow: none;
}

.jp-Stdin-input:focus::placeholder {
  opacity: 1;
}

/*-----------------------------------------------------------------------------
| Output Area View
|----------------------------------------------------------------------------*/

.jp-LinkedOutputView .jp-OutputArea {
  height: 100%;
  display: block;
}

.jp-LinkedOutputView .jp-OutputArea-output:only-child {
  height: 100%;
}

/*-----------------------------------------------------------------------------
| Printing
|----------------------------------------------------------------------------*/

@media print {
  .jp-OutputArea-child {
    break-inside: avoid-page;
  }
}

/*-----------------------------------------------------------------------------
| Mobile
|----------------------------------------------------------------------------*/
@media only screen and (max-width: 760px) {
  .jp-OutputPrompt {
    display: table-row;
    text-align: left;
  }

  .jp-OutputArea-child .jp-OutputArea-output {
    display: table-row;
    margin-left: var(--jp-notebook-padding);
  }
}

/* Trimmed outputs warning */
.jp-TrimmedOutputs > a {
  margin: 10px;
  text-decoration: none;
  cursor: pointer;
}

.jp-TrimmedOutputs > a:hover {
  text-decoration: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Table of Contents
|----------------------------------------------------------------------------*/

:root {
  --jp-private-toc-active-width: 4px;
}

.jp-TableOfContents {
  display: flex;
  flex-direction: column;
  background: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  height: 100%;
}

.jp-TableOfContents-placeholder {
  text-align: center;
}

.jp-TableOfContents-placeholderContent {
  color: var(--jp-content-font-color2);
  padding: 8px;
}

.jp-TableOfContents-placeholderContent > h3 {
  margin-bottom: var(--jp-content-heading-margin-bottom);
}

.jp-TableOfContents .jp-SidePanel-content {
  overflow-y: auto;
}

.jp-TableOfContents-tree {
  margin: 4px;
}

.jp-TableOfContents ol {
  list-style-type: none;
}

/* stylelint-disable-next-line selector-max-type */
.jp-TableOfContents li > ol {
  /* Align left border with triangle icon center */
  padding-left: 11px;
}

.jp-TableOfContents-content {
  /* left margin for the active heading indicator */
  margin: 0 0 0 var(--jp-private-toc-active-width);
  padding: 0;
  background-color: var(--jp-layout-color1);
}

.jp-tocItem {
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-tocItem-heading {
  display: flex;
  cursor: pointer;
}

.jp-tocItem-heading:hover {
  background-color: var(--jp-layout-color2);
}

.jp-tocItem-content {
  display: block;
  padding: 4px 0;
  white-space: nowrap;
  text-overflow: ellipsis;
  overflow-x: hidden;
}

.jp-tocItem-collapser {
  height: 20px;
  margin: 2px 2px 0;
  padding: 0;
  background: none;
  border: none;
  cursor: pointer;
}

.jp-tocItem-collapser:hover {
  background-color: var(--jp-layout-color3);
}

/* Active heading indicator */

.jp-tocItem-heading::before {
  content: ' ';
  background: transparent;
  width: var(--jp-private-toc-active-width);
  height: 24px;
  position: absolute;
  left: 0;
  border-radius: var(--jp-border-radius);
}

.jp-tocItem-heading.jp-tocItem-active::before {
  background-color: var(--jp-brand-color1);
}

.jp-tocItem-heading:hover.jp-tocItem-active::before {
  background: var(--jp-brand-color0);
  opacity: 1;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Collapser {
  flex: 0 0 var(--jp-cell-collapser-width);
  padding: 0;
  margin: 0;
  border: none;
  outline: none;
  background: transparent;
  border-radius: var(--jp-border-radius);
  opacity: 1;
}

.jp-Collapser-child {
  display: block;
  width: 100%;
  box-sizing: border-box;

  /* height: 100% doesn't work because the height of its parent is computed from content */
  position: absolute;
  top: 0;
  bottom: 0;
}

/*-----------------------------------------------------------------------------
| Printing
|----------------------------------------------------------------------------*/

/*
Hiding collapsers in print mode.

Note: input and output wrappers have "display: block" propery in print mode.
*/

@media print {
  .jp-Collapser {
    display: none;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Header/Footer
|----------------------------------------------------------------------------*/

/* Hidden by zero height by default */
.jp-CellHeader,
.jp-CellFooter {
  height: 0;
  width: 100%;
  padding: 0;
  margin: 0;
  border: none;
  outline: none;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Input
|----------------------------------------------------------------------------*/

/* All input areas */
.jp-InputArea {
  display: table;
  table-layout: fixed;
  width: 100%;
  overflow: hidden;
}

.jp-InputArea-editor {
  display: table-cell;
  overflow: hidden;
  vertical-align: top;

  /* This is the non-active, default styling */
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  border-radius: 0;
  background: var(--jp-cell-editor-background);
}

.jp-InputPrompt {
  display: table-cell;
  vertical-align: top;
  width: var(--jp-cell-prompt-width);
  color: var(--jp-cell-inprompt-font-color);
  font-family: var(--jp-cell-prompt-font-family);
  padding: var(--jp-code-padding);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  opacity: var(--jp-cell-prompt-opacity);
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;

  /* Right align prompt text, don't wrap to handle large prompt numbers */
  text-align: right;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;

  /* Disable text selection */
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

/*-----------------------------------------------------------------------------
| Mobile
|----------------------------------------------------------------------------*/
@media only screen and (max-width: 760px) {
  .jp-InputArea-editor {
    display: table-row;
    margin-left: var(--jp-notebook-padding);
  }

  .jp-InputPrompt {
    display: table-row;
    text-align: left;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Placeholder
|----------------------------------------------------------------------------*/

.jp-Placeholder {
  display: table;
  table-layout: fixed;
  width: 100%;
}

.jp-Placeholder-prompt {
  display: table-cell;
  box-sizing: border-box;
}

.jp-Placeholder-content {
  display: table-cell;
  padding: 4px 6px;
  border: 1px solid transparent;
  border-radius: 0;
  background: none;
  box-sizing: border-box;
  cursor: pointer;
}

.jp-Placeholder-contentContainer {
  display: flex;
}

.jp-Placeholder-content:hover,
.jp-InputPlaceholder > .jp-Placeholder-content:hover {
  border-color: var(--jp-layout-color3);
}

.jp-Placeholder-content .jp-MoreHorizIcon {
  width: 32px;
  height: 16px;
  border: 1px solid transparent;
  border-radius: var(--jp-border-radius);
}

.jp-Placeholder-content .jp-MoreHorizIcon:hover {
  border: 1px solid var(--jp-border-color1);
  box-shadow: 0 0 2px 0 rgba(0, 0, 0, 0.25);
  background-color: var(--jp-layout-color0);
}

.jp-PlaceholderText {
  white-space: nowrap;
  overflow-x: hidden;
  color: var(--jp-inverse-layout-color3);
  font-family: var(--jp-code-font-family);
}

.jp-InputPlaceholder > .jp-Placeholder-content {
  border-color: var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Private CSS variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-cell-scrolling-output-offset: 5px;
}

/*-----------------------------------------------------------------------------
| Cell
|----------------------------------------------------------------------------*/

.jp-Cell {
  padding: var(--jp-cell-padding);
  margin: 0;
  border: none;
  outline: none;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Common input/output
|----------------------------------------------------------------------------*/

.jp-Cell-inputWrapper,
.jp-Cell-outputWrapper {
  display: flex;
  flex-direction: row;
  padding: 0;
  margin: 0;

  /* Added to reveal the box-shadow on the input and output collapsers. */
  overflow: visible;
}

/* Only input/output areas inside cells */
.jp-Cell-inputArea,
.jp-Cell-outputArea {
  flex: 1 1 auto;
}

/*-----------------------------------------------------------------------------
| Collapser
|----------------------------------------------------------------------------*/

/* Make the output collapser disappear when there is not output, but do so
 * in a manner that leaves it in the layout and preserves its width.
 */
.jp-Cell.jp-mod-noOutputs .jp-Cell-outputCollapser {
  border: none !important;
  background: transparent !important;
}

.jp-Cell:not(.jp-mod-noOutputs) .jp-Cell-outputCollapser {
  min-height: var(--jp-cell-collapser-min-height);
}

/*-----------------------------------------------------------------------------
| Output
|----------------------------------------------------------------------------*/

/* Put a space between input and output when there IS output */
.jp-Cell:not(.jp-mod-noOutputs) .jp-Cell-outputWrapper {
  margin-top: 5px;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea {
  overflow-y: auto;
  max-height: 24em;
  margin-left: var(--jp-private-cell-scrolling-output-offset);
  resize: vertical;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea[style*='height'] {
  max-height: unset;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea::after {
  content: ' ';
  box-shadow: inset 0 0 6px 2px rgb(0 0 0 / 30%);
  width: 100%;
  height: 100%;
  position: sticky;
  bottom: 0;
  top: 0;
  margin-top: -50%;
  float: left;
  display: block;
  pointer-events: none;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-child {
  padding-top: 6px;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-prompt {
  width: calc(
    var(--jp-cell-prompt-width) - var(--jp-private-cell-scrolling-output-offset)
  );
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-promptOverlay {
  left: calc(-1 * var(--jp-private-cell-scrolling-output-offset));
}

/*-----------------------------------------------------------------------------
| CodeCell
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| MarkdownCell
|----------------------------------------------------------------------------*/

.jp-MarkdownOutput {
  display: table-cell;
  width: 100%;
  margin-top: 0;
  margin-bottom: 0;
  padding-left: var(--jp-code-padding);
}

.jp-MarkdownOutput.jp-RenderedHTMLCommon {
  overflow: auto;
}

/* collapseHeadingButton (show always if hiddenCellsButton is _not_ shown) */
.jp-collapseHeadingButton {
  display: flex;
  min-height: var(--jp-cell-collapser-min-height);
  font-size: var(--jp-code-font-size);
  position: absolute;
  background-color: transparent;
  background-size: 25px;
  background-repeat: no-repeat;
  background-position-x: center;
  background-position-y: top;
  background-image: var(--jp-icon-caret-down);
  right: 0;
  top: 0;
  bottom: 0;
}

.jp-collapseHeadingButton.jp-mod-collapsed {
  background-image: var(--jp-icon-caret-right);
}

/*
 set the container font size to match that of content
 so that the nested collapse buttons have the right size
*/
.jp-MarkdownCell .jp-InputPrompt {
  font-size: var(--jp-content-font-size1);
}

/*
  Align collapseHeadingButton with cell top header
  The font sizes are identical to the ones in packages/rendermime/style/base.css
*/
.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='1'] {
  font-size: var(--jp-content-font-size5);
  background-position-y: calc(0.3 * var(--jp-content-font-size5));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='2'] {
  font-size: var(--jp-content-font-size4);
  background-position-y: calc(0.3 * var(--jp-content-font-size4));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='3'] {
  font-size: var(--jp-content-font-size3);
  background-position-y: calc(0.3 * var(--jp-content-font-size3));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='4'] {
  font-size: var(--jp-content-font-size2);
  background-position-y: calc(0.3 * var(--jp-content-font-size2));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='5'] {
  font-size: var(--jp-content-font-size1);
  background-position-y: top;
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='6'] {
  font-size: var(--jp-content-font-size0);
  background-position-y: top;
}

/* collapseHeadingButton (show only on (hover,active) if hiddenCellsButton is shown) */
.jp-Notebook.jp-mod-showHiddenCellsButton .jp-collapseHeadingButton {
  display: none;
}

.jp-Notebook.jp-mod-showHiddenCellsButton
  :is(.jp-MarkdownCell:hover, .jp-mod-active)
  .jp-collapseHeadingButton {
  display: flex;
}

/* showHiddenCellsButton (only show if jp-mod-showHiddenCellsButton is set, which
is a consequence of the showHiddenCellsButton option in Notebook Settings)*/
.jp-Notebook.jp-mod-showHiddenCellsButton .jp-showHiddenCellsButton {
  margin-left: calc(var(--jp-cell-prompt-width) + 2 * var(--jp-code-padding));
  margin-top: var(--jp-code-padding);
  border: 1px solid var(--jp-border-color2);
  background-color: var(--jp-border-color3) !important;
  color: var(--jp-content-font-color0) !important;
  display: flex;
}

.jp-Notebook.jp-mod-showHiddenCellsButton .jp-showHiddenCellsButton:hover {
  background-color: var(--jp-border-color2) !important;
}

.jp-showHiddenCellsButton {
  display: none;
}

/*-----------------------------------------------------------------------------
| Printing
|----------------------------------------------------------------------------*/

/*
Using block instead of flex to allow the use of the break-inside CSS property for
cell outputs.
*/

@media print {
  .jp-Cell-inputWrapper,
  .jp-Cell-outputWrapper {
    display: block;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

:root {
  --jp-notebook-toolbar-padding: 2px 5px 2px 2px;
}

/*-----------------------------------------------------------------------------

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-NotebookPanel-toolbar {
  padding: var(--jp-notebook-toolbar-padding);

  /* disable paint containment from lumino 2.0 default strict CSS containment */
  contain: style size !important;
}

.jp-Toolbar-item.jp-Notebook-toolbarCellType .jp-select-wrapper.jp-mod-focused {
  border: none;
  box-shadow: none;
}

.jp-Notebook-toolbarCellTypeDropdown select {
  height: 24px;
  font-size: var(--jp-ui-font-size1);
  line-height: 14px;
  border-radius: 0;
  display: block;
}

.jp-Notebook-toolbarCellTypeDropdown span {
  top: 5px !important;
}

.jp-Toolbar-responsive-popup {
  position: absolute;
  height: fit-content;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: flex-end;
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  box-shadow: var(--jp-toolbar-box-shadow);
  background: var(--jp-toolbar-background);
  min-height: var(--jp-toolbar-micro-height);
  padding: var(--jp-notebook-toolbar-padding);
  z-index: 1;
  right: 0;
  top: 0;
}

.jp-Toolbar > .jp-Toolbar-responsive-opener {
  margin-left: auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-Notebook-ExecutionIndicator {
  position: relative;
  display: inline-block;
  height: 100%;
  z-index: 9997;
}

.jp-Notebook-ExecutionIndicator-tooltip {
  visibility: hidden;
  height: auto;
  width: max-content;
  width: -moz-max-content;
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color1);
  text-align: justify;
  border-radius: 6px;
  padding: 0 5px;
  position: fixed;
  display: table;
}

.jp-Notebook-ExecutionIndicator-tooltip.up {
  transform: translateX(-50%) translateY(-100%) translateY(-32px);
}

.jp-Notebook-ExecutionIndicator-tooltip.down {
  transform: translateX(calc(-100% + 16px)) translateY(5px);
}

.jp-Notebook-ExecutionIndicator-tooltip.hidden {
  display: none;
}

.jp-Notebook-ExecutionIndicator:hover .jp-Notebook-ExecutionIndicator-tooltip {
  visibility: visible;
}

.jp-Notebook-ExecutionIndicator span {
  font-size: var(--jp-ui-font-size1);
  font-family: var(--jp-ui-font-family);
  color: var(--jp-ui-font-color1);
  line-height: 24px;
  display: block;
}

.jp-Notebook-ExecutionIndicator-progress-bar {
  display: flex;
  justify-content: center;
  height: 100%;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*
 * Execution indicator
 */
.jp-tocItem-content::after {
  content: '';

  /* Must be identical to form a circle */
  width: 12px;
  height: 12px;
  background: none;
  border: none;
  position: absolute;
  right: 0;
}

.jp-tocItem-content[data-running='0']::after {
  border-radius: 50%;
  border: var(--jp-border-width) solid var(--jp-inverse-layout-color3);
  background: none;
}

.jp-tocItem-content[data-running='1']::after {
  border-radius: 50%;
  border: var(--jp-border-width) solid var(--jp-inverse-layout-color3);
  background-color: var(--jp-inverse-layout-color3);
}

.jp-tocItem-content[data-running='0'],
.jp-tocItem-content[data-running='1'] {
  margin-right: 12px;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-Notebook-footer {
  height: 27px;
  margin-left: calc(
    var(--jp-cell-prompt-width) + var(--jp-cell-collapser-width) +
      var(--jp-cell-padding)
  );
  width: calc(
    100% -
      (
        var(--jp-cell-prompt-width) + var(--jp-cell-collapser-width) +
          var(--jp-cell-padding) + var(--jp-cell-padding)
      )
  );
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  color: var(--jp-ui-font-color3);
  margin-top: 6px;
  background: none;
  cursor: pointer;
}

.jp-Notebook-footer:focus {
  border-color: var(--jp-cell-editor-active-border-color);
}

/* For devices that support hovering, hide footer until hover */
@media (hover: hover) {
  .jp-Notebook-footer {
    opacity: 0;
  }

  .jp-Notebook-footer:focus,
  .jp-Notebook-footer:hover {
    opacity: 1;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Imports
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| CSS variables
|----------------------------------------------------------------------------*/

:root {
  --jp-side-by-side-output-size: 1fr;
  --jp-side-by-side-resized-cell: var(--jp-side-by-side-output-size);
  --jp-private-notebook-dragImage-width: 304px;
  --jp-private-notebook-dragImage-height: 36px;
  --jp-private-notebook-selected-color: var(--md-blue-400);
  --jp-private-notebook-active-color: var(--md-green-400);
}

/*-----------------------------------------------------------------------------
| Notebook
|----------------------------------------------------------------------------*/

/* stylelint-disable selector-max-class */

.jp-NotebookPanel {
  display: block;
  height: 100%;
}

.jp-NotebookPanel.jp-Document {
  min-width: 240px;
  min-height: 120px;
}

.jp-Notebook {
  padding: var(--jp-notebook-padding);
  outline: none;
  overflow: auto;
  background: var(--jp-layout-color0);
}

.jp-Notebook.jp-mod-scrollPastEnd::after {
  display: block;
  content: '';
  min-height: var(--jp-notebook-scroll-padding);
}

.jp-MainAreaWidget-ContainStrict .jp-Notebook * {
  contain: strict;
}

.jp-Notebook .jp-Cell {
  overflow: visible;
}

.jp-Notebook .jp-Cell .jp-InputPrompt {
  cursor: move;
}

/*-----------------------------------------------------------------------------
| Notebook state related styling
|
| The notebook and cells each have states, here are the possibilities:
|
| - Notebook
|   - Command
|   - Edit
| - Cell
|   - None
|   - Active (only one can be active)
|   - Selected (the cells actions are applied to)
|   - Multiselected (when multiple selected, the cursor)
|   - No outputs
|----------------------------------------------------------------------------*/

/* Command or edit modes */

.jp-Notebook .jp-Cell:not(.jp-mod-active) .jp-InputPrompt {
  opacity: var(--jp-cell-prompt-not-active-opacity);
  color: var(--jp-cell-prompt-not-active-font-color);
}

.jp-Notebook .jp-Cell:not(.jp-mod-active) .jp-OutputPrompt {
  opacity: var(--jp-cell-prompt-not-active-opacity);
  color: var(--jp-cell-prompt-not-active-font-color);
}

/* cell is active */
.jp-Notebook .jp-Cell.jp-mod-active .jp-Collapser {
  background: var(--jp-brand-color1);
}

/* cell is dirty */
.jp-Notebook .jp-Cell.jp-mod-dirty .jp-InputPrompt {
  color: var(--jp-warn-color1);
}

.jp-Notebook .jp-Cell.jp-mod-dirty .jp-InputPrompt::before {
  color: var(--jp-warn-color1);
  content: '•';
}

.jp-Notebook .jp-Cell.jp-mod-active.jp-mod-dirty .jp-Collapser {
  background: var(--jp-warn-color1);
}

/* collapser is hovered */
.jp-Notebook .jp-Cell .jp-Collapser:hover {
  box-shadow: var(--jp-elevation-z2);
  background: var(--jp-brand-color1);
  opacity: var(--jp-cell-collapser-not-active-hover-opacity);
}

/* cell is active and collapser is hovered */
.jp-Notebook .jp-Cell.jp-mod-active .jp-Collapser:hover {
  background: var(--jp-brand-color0);
  opacity: 1;
}

/* Command mode */

.jp-Notebook.jp-mod-commandMode .jp-Cell.jp-mod-selected {
  background: var(--jp-notebook-multiselected-color);
}

.jp-Notebook.jp-mod-commandMode
  .jp-Cell.jp-mod-active.jp-mod-selected:not(.jp-mod-multiSelected) {
  background: transparent;
}

/* Edit mode */

.jp-Notebook.jp-mod-editMode .jp-Cell.jp-mod-active .jp-InputArea-editor {
  border: var(--jp-border-width) solid var(--jp-cell-editor-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
  background-color: var(--jp-cell-editor-active-background);
}

/*-----------------------------------------------------------------------------
| Notebook drag and drop
|----------------------------------------------------------------------------*/

.jp-Notebook-cell.jp-mod-dropSource {
  opacity: 0.5;
}

.jp-Notebook-cell.jp-mod-dropTarget,
.jp-Notebook.jp-mod-commandMode
  .jp-Notebook-cell.jp-mod-active.jp-mod-selected.jp-mod-dropTarget {
  border-top-color: var(--jp-private-notebook-selected-color);
  border-top-style: solid;
  border-top-width: 2px;
}

.jp-dragImage {
  display: block;
  flex-direction: row;
  width: var(--jp-private-notebook-dragImage-width);
  height: var(--jp-private-notebook-dragImage-height);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background);
  overflow: visible;
}

.jp-dragImage-singlePrompt {
  box-shadow: 2px 2px 4px 0 rgba(0, 0, 0, 0.12);
}

.jp-dragImage .jp-dragImage-content {
  flex: 1 1 auto;
  z-index: 2;
  font-size: var(--jp-code-font-size);
  font-family: var(--jp-code-font-family);
  line-height: var(--jp-code-line-height);
  padding: var(--jp-code-padding);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background-color);
  color: var(--jp-content-font-color3);
  text-align: left;
  margin: 4px 4px 4px 0;
}

.jp-dragImage .jp-dragImage-prompt {
  flex: 0 0 auto;
  min-width: 36px;
  color: var(--jp-cell-inprompt-font-color);
  padding: var(--jp-code-padding);
  padding-left: 12px;
  font-family: var(--jp-cell-prompt-font-family);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  line-height: 1.9;
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;
}

.jp-dragImage-multipleBack {
  z-index: -1;
  position: absolute;
  height: 32px;
  width: 300px;
  top: 8px;
  left: 8px;
  background: var(--jp-layout-color2);
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  box-shadow: 2px 2px 4px 0 rgba(0, 0, 0, 0.12);
}

/*-----------------------------------------------------------------------------
| Cell toolbar
|----------------------------------------------------------------------------*/

.jp-NotebookTools {
  display: block;
  min-width: var(--jp-sidebar-min-width);
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);

  /* This is needed so that all font sizing of children done in ems is
    * relative to this base size */
  font-size: var(--jp-ui-font-size1);
  overflow: auto;
}

.jp-ActiveCellTool {
  padding: 12px 0;
  display: flex;
}

.jp-ActiveCellTool-Content {
  flex: 1 1 auto;
}

.jp-ActiveCellTool .jp-ActiveCellTool-CellContent {
  background: var(--jp-cell-editor-background);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  border-radius: 0;
  min-height: 29px;
}

.jp-ActiveCellTool .jp-InputPrompt {
  min-width: calc(var(--jp-cell-prompt-width) * 0.75);
}

.jp-ActiveCellTool-CellContent > pre {
  padding: 5px 4px;
  margin: 0;
  white-space: normal;
}

.jp-MetadataEditorTool {
  flex-direction: column;
  padding: 12px 0;
}

.jp-RankedPanel > :not(:first-child) {
  margin-top: 12px;
}

.jp-KeySelector select.jp-mod-styled {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  border: var(--jp-border-width) solid var(--jp-border-color1);
}

.jp-KeySelector label,
.jp-MetadataEditorTool label,
.jp-NumberSetter label {
  line-height: 1.4;
}

.jp-NotebookTools .jp-select-wrapper {
  margin-top: 4px;
  margin-bottom: 0;
}

.jp-NumberSetter input {
  width: 100%;
  margin-top: 4px;
}

.jp-NotebookTools .jp-Collapse {
  margin-top: 16px;
}

/*-----------------------------------------------------------------------------
| Presentation Mode (.jp-mod-presentationMode)
|----------------------------------------------------------------------------*/

.jp-mod-presentationMode .jp-Notebook {
  --jp-content-font-size1: var(--jp-content-presentation-font-size1);
  --jp-code-font-size: var(--jp-code-presentation-font-size);
}

.jp-mod-presentationMode .jp-Notebook .jp-Cell .jp-InputPrompt,
.jp-mod-presentationMode .jp-Notebook .jp-Cell .jp-OutputPrompt {
  flex: 0 0 110px;
}

/*-----------------------------------------------------------------------------
| Side-by-side Mode (.jp-mod-sideBySide)
|----------------------------------------------------------------------------*/
.jp-mod-sideBySide.jp-Notebook .jp-Notebook-cell {
  margin-top: 3em;
  margin-bottom: 3em;
  margin-left: 5%;
  margin-right: 5%;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell {
  display: grid;
  grid-template-columns: minmax(0, 1fr) min-content minmax(
      0,
      var(--jp-side-by-side-output-size)
    );
  grid-template-rows: auto minmax(0, 1fr) auto;
  grid-template-areas:
    'header header header'
    'input handle output'
    'footer footer footer';
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell.jp-mod-resizedCell {
  grid-template-columns: minmax(0, 1fr) min-content minmax(
      0,
      var(--jp-side-by-side-resized-cell)
    );
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellHeader {
  grid-area: header;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-Cell-inputWrapper {
  grid-area: input;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-Cell-outputWrapper {
  /* overwrite the default margin (no vertical separation needed in side by side move */
  margin-top: 0;
  grid-area: output;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellFooter {
  grid-area: footer;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellResizeHandle {
  grid-area: handle;
  user-select: none;
  display: block;
  height: 100%;
  cursor: ew-resize;
  padding: 0 var(--jp-cell-padding);
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellResizeHandle::after {
  content: '';
  display: block;
  background: var(--jp-border-color2);
  height: 100%;
  width: 5px;
}

.jp-mod-sideBySide.jp-Notebook
  .jp-CodeCell.jp-mod-resizedCell
  .jp-CellResizeHandle::after {
  background: var(--jp-border-color0);
}

.jp-CellResizeHandle {
  display: none;
}

/*-----------------------------------------------------------------------------
| Placeholder
|----------------------------------------------------------------------------*/

.jp-Cell-Placeholder {
  padding-left: 55px;
}

.jp-Cell-Placeholder-wrapper {
  background: #fff;
  border: 1px solid;
  border-color: #e5e6e9 #dfe0e4 #d0d1d5;
  border-radius: 4px;
  -webkit-border-radius: 4px;
  margin: 10px 15px;
}

.jp-Cell-Placeholder-wrapper-inner {
  padding: 15px;
  position: relative;
}

.jp-Cell-Placeholder-wrapper-body {
  background-repeat: repeat;
  background-size: 50% auto;
}

.jp-Cell-Placeholder-wrapper-body div {
  background: #f6f7f8;
  background-image: -webkit-linear-gradient(
    left,
    #f6f7f8 0%,
    #edeef1 20%,
    #f6f7f8 40%,
    #f6f7f8 100%
  );
  background-repeat: no-repeat;
  background-size: 800px 104px;
  height: 104px;
  position: absolute;
  right: 15px;
  left: 15px;
  top: 15px;
}

div.jp-Cell-Placeholder-h1 {
  top: 20px;
  height: 20px;
  left: 15px;
  width: 150px;
}

div.jp-Cell-Placeholder-h2 {
  left: 15px;
  top: 50px;
  height: 10px;
  width: 100px;
}

div.jp-Cell-Placeholder-content-1,
div.jp-Cell-Placeholder-content-2,
div.jp-Cell-Placeholder-content-3 {
  left: 15px;
  right: 15px;
  height: 10px;
}

div.jp-Cell-Placeholder-content-1 {
  top: 100px;
}

div.jp-Cell-Placeholder-content-2 {
  top: 120px;
}

div.jp-Cell-Placeholder-content-3 {
  top: 140px;
}

</style>
<style type="text/css">
/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*
The following CSS variables define the main, public API for styling JupyterLab.
These variables should be used by all plugins wherever possible. In other
words, plugins should not define custom colors, sizes, etc unless absolutely
necessary. This enables users to change the visual theme of JupyterLab
by changing these variables.

Many variables appear in an ordered sequence (0,1,2,3). These sequences
are designed to work well together, so for example, `--jp-border-color1` should
be used with `--jp-layout-color1`. The numbers have the following meanings:

* 0: super-primary, reserved for special emphasis
* 1: primary, most important under normal situations
* 2: secondary, next most important under normal situations
* 3: tertiary, next most important under normal situations

Throughout JupyterLab, we are mostly following principles from Google's
Material Design when selecting colors. We are not, however, following
all of MD as it is not optimized for dense, information rich UIs.
*/

:root {
  /* Elevation
   *
   * We style box-shadows using Material Design's idea of elevation. These particular numbers are taken from here:
   *
   * https://github.com/material-components/material-components-web
   * https://material-components-web.appspot.com/elevation.html
   */

  --jp-shadow-base-lightness: 0;
  --jp-shadow-umbra-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.2
  );
  --jp-shadow-penumbra-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.14
  );
  --jp-shadow-ambient-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.12
  );
  --jp-elevation-z0: none;
  --jp-elevation-z1: 0 2px 1px -1px var(--jp-shadow-umbra-color),
    0 1px 1px 0 var(--jp-shadow-penumbra-color),
    0 1px 3px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z2: 0 3px 1px -2px var(--jp-shadow-umbra-color),
    0 2px 2px 0 var(--jp-shadow-penumbra-color),
    0 1px 5px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z4: 0 2px 4px -1px var(--jp-shadow-umbra-color),
    0 4px 5px 0 var(--jp-shadow-penumbra-color),
    0 1px 10px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z6: 0 3px 5px -1px var(--jp-shadow-umbra-color),
    0 6px 10px 0 var(--jp-shadow-penumbra-color),
    0 1px 18px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z8: 0 5px 5px -3px var(--jp-shadow-umbra-color),
    0 8px 10px 1px var(--jp-shadow-penumbra-color),
    0 3px 14px 2px var(--jp-shadow-ambient-color);
  --jp-elevation-z12: 0 7px 8px -4px var(--jp-shadow-umbra-color),
    0 12px 17px 2px var(--jp-shadow-penumbra-color),
    0 5px 22px 4px var(--jp-shadow-ambient-color);
  --jp-elevation-z16: 0 8px 10px -5px var(--jp-shadow-umbra-color),
    0 16px 24px 2px var(--jp-shadow-penumbra-color),
    0 6px 30px 5px var(--jp-shadow-ambient-color);
  --jp-elevation-z20: 0 10px 13px -6px var(--jp-shadow-umbra-color),
    0 20px 31px 3px var(--jp-shadow-penumbra-color),
    0 8px 38px 7px var(--jp-shadow-ambient-color);
  --jp-elevation-z24: 0 11px 15px -7px var(--jp-shadow-umbra-color),
    0 24px 38px 3px var(--jp-shadow-penumbra-color),
    0 9px 46px 8px var(--jp-shadow-ambient-color);

  /* Borders
   *
   * The following variables, specify the visual styling of borders in JupyterLab.
   */

  --jp-border-width: 1px;
  --jp-border-color0: var(--md-grey-400);
  --jp-border-color1: var(--md-grey-400);
  --jp-border-color2: var(--md-grey-300);
  --jp-border-color3: var(--md-grey-200);
  --jp-inverse-border-color: var(--md-grey-600);
  --jp-border-radius: 2px;

  /* UI Fonts
   *
   * The UI font CSS variables are used for the typography all of the JupyterLab
   * user interface elements that are not directly user generated content.
   *
   * The font sizing here is done assuming that the body font size of --jp-ui-font-size1
   * is applied to a parent element. When children elements, such as headings, are sized
   * in em all things will be computed relative to that body size.
   */

  --jp-ui-font-scale-factor: 1.2;
  --jp-ui-font-size0: 0.83333em;
  --jp-ui-font-size1: 13px; /* Base font size */
  --jp-ui-font-size2: 1.2em;
  --jp-ui-font-size3: 1.44em;
  --jp-ui-font-family: system-ui, -apple-system, blinkmacsystemfont, 'Segoe UI',
    helvetica, arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
    'Segoe UI Symbol';

  /*
   * Use these font colors against the corresponding main layout colors.
   * In a light theme, these go from dark to light.
   */

  /* Defaults use Material Design specification */
  --jp-ui-font-color0: rgba(0, 0, 0, 1);
  --jp-ui-font-color1: rgba(0, 0, 0, 0.87);
  --jp-ui-font-color2: rgba(0, 0, 0, 0.54);
  --jp-ui-font-color3: rgba(0, 0, 0, 0.38);

  /*
   * Use these against the brand/accent/warn/error colors.
   * These will typically go from light to darker, in both a dark and light theme.
   */

  --jp-ui-inverse-font-color0: rgba(255, 255, 255, 1);
  --jp-ui-inverse-font-color1: rgba(255, 255, 255, 1);
  --jp-ui-inverse-font-color2: rgba(255, 255, 255, 0.7);
  --jp-ui-inverse-font-color3: rgba(255, 255, 255, 0.5);

  /* Content Fonts
   *
   * Content font variables are used for typography of user generated content.
   *
   * The font sizing here is done assuming that the body font size of --jp-content-font-size1
   * is applied to a parent element. When children elements, such as headings, are sized
   * in em all things will be computed relative to that body size.
   */

  --jp-content-line-height: 1.6;
  --jp-content-font-scale-factor: 1.2;
  --jp-content-font-size0: 0.83333em;
  --jp-content-font-size1: 14px; /* Base font size */
  --jp-content-font-size2: 1.2em;
  --jp-content-font-size3: 1.44em;
  --jp-content-font-size4: 1.728em;
  --jp-content-font-size5: 2.0736em;

  /* This gives a magnification of about 125% in presentation mode over normal. */
  --jp-content-presentation-font-size1: 17px;
  --jp-content-heading-line-height: 1;
  --jp-content-heading-margin-top: 1.2em;
  --jp-content-heading-margin-bottom: 0.8em;
  --jp-content-heading-font-weight: 500;

  /* Defaults use Material Design specification */
  --jp-content-font-color0: rgba(0, 0, 0, 1);
  --jp-content-font-color1: rgba(0, 0, 0, 0.87);
  --jp-content-font-color2: rgba(0, 0, 0, 0.54);
  --jp-content-font-color3: rgba(0, 0, 0, 0.38);
  --jp-content-link-color: var(--md-blue-900);
  --jp-content-font-family: system-ui, -apple-system, blinkmacsystemfont,
    'Segoe UI', helvetica, arial, sans-serif, 'Apple Color Emoji',
    'Segoe UI Emoji', 'Segoe UI Symbol';

  /*
   * Code Fonts
   *
   * Code font variables are used for typography of code and other monospaces content.
   */

  --jp-code-font-size: 13px;
  --jp-code-line-height: 1.3077; /* 17px for 13px base */
  --jp-code-padding: 5px; /* 5px for 13px base, codemirror highlighting needs integer px value */
  --jp-code-font-family-default: menlo, consolas, 'DejaVu Sans Mono', monospace;
  --jp-code-font-family: var(--jp-code-font-family-default);

  /* This gives a magnification of about 125% in presentation mode over normal. */
  --jp-code-presentation-font-size: 16px;

  /* may need to tweak cursor width if you change font size */
  --jp-code-cursor-width0: 1.4px;
  --jp-code-cursor-width1: 2px;
  --jp-code-cursor-width2: 4px;

  /* Layout
   *
   * The following are the main layout colors use in JupyterLab. In a light
   * theme these would go from light to dark.
   */

  --jp-layout-color0: white;
  --jp-layout-color1: white;
  --jp-layout-color2: var(--md-grey-200);
  --jp-layout-color3: var(--md-grey-400);
  --jp-layout-color4: var(--md-grey-600);

  /* Inverse Layout
   *
   * The following are the inverse layout colors use in JupyterLab. In a light
   * theme these would go from dark to light.
   */

  --jp-inverse-layout-color0: #111;
  --jp-inverse-layout-color1: var(--md-grey-900);
  --jp-inverse-layout-color2: var(--md-grey-800);
  --jp-inverse-layout-color3: var(--md-grey-700);
  --jp-inverse-layout-color4: var(--md-grey-600);

  /* Brand/accent */

  --jp-brand-color0: var(--md-blue-900);
  --jp-brand-color1: var(--md-blue-700);
  --jp-brand-color2: var(--md-blue-300);
  --jp-brand-color3: var(--md-blue-100);
  --jp-brand-color4: var(--md-blue-50);
  --jp-accent-color0: var(--md-green-900);
  --jp-accent-color1: var(--md-green-700);
  --jp-accent-color2: var(--md-green-300);
  --jp-accent-color3: var(--md-green-100);

  /* State colors (warn, error, success, info) */

  --jp-warn-color0: var(--md-orange-900);
  --jp-warn-color1: var(--md-orange-700);
  --jp-warn-color2: var(--md-orange-300);
  --jp-warn-color3: var(--md-orange-100);
  --jp-error-color0: var(--md-red-900);
  --jp-error-color1: var(--md-red-700);
  --jp-error-color2: var(--md-red-300);
  --jp-error-color3: var(--md-red-100);
  --jp-success-color0: var(--md-green-900);
  --jp-success-color1: var(--md-green-700);
  --jp-success-color2: var(--md-green-300);
  --jp-success-color3: var(--md-green-100);
  --jp-info-color0: var(--md-cyan-900);
  --jp-info-color1: var(--md-cyan-700);
  --jp-info-color2: var(--md-cyan-300);
  --jp-info-color3: var(--md-cyan-100);

  /* Cell specific styles */

  --jp-cell-padding: 5px;
  --jp-cell-collapser-width: 8px;
  --jp-cell-collapser-min-height: 20px;
  --jp-cell-collapser-not-active-hover-opacity: 0.6;
  --jp-cell-editor-background: var(--md-grey-100);
  --jp-cell-editor-border-color: var(--md-grey-300);
  --jp-cell-editor-box-shadow: inset 0 0 2px var(--md-blue-300);
  --jp-cell-editor-active-background: var(--jp-layout-color0);
  --jp-cell-editor-active-border-color: var(--jp-brand-color1);
  --jp-cell-prompt-width: 64px;
  --jp-cell-prompt-font-family: var(--jp-code-font-family-default);
  --jp-cell-prompt-letter-spacing: 0;
  --jp-cell-prompt-opacity: 1;
  --jp-cell-prompt-not-active-opacity: 0.5;
  --jp-cell-prompt-not-active-font-color: var(--md-grey-700);

  /* A custom blend of MD grey and blue 600
   * See https://meyerweb.com/eric/tools/color-blend/#546E7A:1E88E5:5:hex */
  --jp-cell-inprompt-font-color: #307fc1;

  /* A custom blend of MD grey and orange 600
   * https://meyerweb.com/eric/tools/color-blend/#546E7A:F4511E:5:hex */
  --jp-cell-outprompt-font-color: #bf5b3d;

  /* Notebook specific styles */

  --jp-notebook-padding: 10px;
  --jp-notebook-select-background: var(--jp-layout-color1);
  --jp-notebook-multiselected-color: var(--md-blue-50);

  /* The scroll padding is calculated to fill enough space at the bottom of the
  notebook to show one single-line cell (with appropriate padding) at the top
  when the notebook is scrolled all the way to the bottom. We also subtract one
  pixel so that no scrollbar appears if we have just one single-line cell in the
  notebook. This padding is to enable a 'scroll past end' feature in a notebook.
  */
  --jp-notebook-scroll-padding: calc(
    100% - var(--jp-code-font-size) * var(--jp-code-line-height) -
      var(--jp-code-padding) - var(--jp-cell-padding) - 1px
  );

  /* Rendermime styles */

  --jp-rendermime-error-background: #fdd;
  --jp-rendermime-table-row-background: var(--md-grey-100);
  --jp-rendermime-table-row-hover-background: var(--md-light-blue-50);

  /* Dialog specific styles */

  --jp-dialog-background: rgba(0, 0, 0, 0.25);

  /* Console specific styles */

  --jp-console-padding: 10px;

  /* Toolbar specific styles */

  --jp-toolbar-border-color: var(--jp-border-color1);
  --jp-toolbar-micro-height: 8px;
  --jp-toolbar-background: var(--jp-layout-color1);
  --jp-toolbar-box-shadow: 0 0 2px 0 rgba(0, 0, 0, 0.24);
  --jp-toolbar-header-margin: 4px 4px 0 4px;
  --jp-toolbar-active-background: var(--md-grey-300);

  /* Statusbar specific styles */

  --jp-statusbar-height: 24px;

  /* Input field styles */

  --jp-input-box-shadow: inset 0 0 2px var(--md-blue-300);
  --jp-input-active-background: var(--jp-layout-color1);
  --jp-input-hover-background: var(--jp-layout-color1);
  --jp-input-background: var(--md-grey-100);
  --jp-input-border-color: var(--jp-inverse-border-color);
  --jp-input-active-border-color: var(--jp-brand-color1);
  --jp-input-active-box-shadow-color: rgba(19, 124, 189, 0.3);

  /* General editor styles */

  --jp-editor-selected-background: #d9d9d9;
  --jp-editor-selected-focused-background: #d7d4f0;
  --jp-editor-cursor-color: var(--jp-ui-font-color0);

  /* Code mirror specific styles */

  --jp-mirror-editor-keyword-color: #008000;
  --jp-mirror-editor-atom-color: #88f;
  --jp-mirror-editor-number-color: #080;
  --jp-mirror-editor-def-color: #00f;
  --jp-mirror-editor-variable-color: var(--md-grey-900);
  --jp-mirror-editor-variable-2-color: rgb(0, 54, 109);
  --jp-mirror-editor-variable-3-color: #085;
  --jp-mirror-editor-punctuation-color: #05a;
  --jp-mirror-editor-property-color: #05a;
  --jp-mirror-editor-operator-color: #a2f;
  --jp-mirror-editor-comment-color: #408080;
  --jp-mirror-editor-string-color: #ba2121;
  --jp-mirror-editor-string-2-color: #708;
  --jp-mirror-editor-meta-color: #a2f;
  --jp-mirror-editor-qualifier-color: #555;
  --jp-mirror-editor-builtin-color: #008000;
  --jp-mirror-editor-bracket-color: #997;
  --jp-mirror-editor-tag-color: #170;
  --jp-mirror-editor-attribute-color: #00c;
  --jp-mirror-editor-header-color: blue;
  --jp-mirror-editor-quote-color: #090;
  --jp-mirror-editor-link-color: #00c;
  --jp-mirror-editor-error-color: #f00;
  --jp-mirror-editor-hr-color: #999;

  /*
    RTC user specific colors.
    These colors are used for the cursor, username in the editor,
    and the icon of the user.
  */

  --jp-collaborator-color1: #ffad8e;
  --jp-collaborator-color2: #dac83d;
  --jp-collaborator-color3: #72dd76;
  --jp-collaborator-color4: #00e4d0;
  --jp-collaborator-color5: #45d4ff;
  --jp-collaborator-color6: #e2b1ff;
  --jp-collaborator-color7: #ff9de6;

  /* Vega extension styles */

  --jp-vega-background: white;

  /* Sidebar-related styles */

  --jp-sidebar-min-width: 250px;

  /* Search-related styles */

  --jp-search-toggle-off-opacity: 0.5;
  --jp-search-toggle-hover-opacity: 0.8;
  --jp-search-toggle-on-opacity: 1;
  --jp-search-selected-match-background-color: rgb(245, 200, 0);
  --jp-search-selected-match-color: black;
  --jp-search-unselected-match-background-color: var(
    --jp-inverse-layout-color0
  );
  --jp-search-unselected-match-color: var(--jp-ui-inverse-font-color0);

  /* Icon colors that work well with light or dark backgrounds */
  --jp-icon-contrast-color0: var(--md-purple-600);
  --jp-icon-contrast-color1: var(--md-green-600);
  --jp-icon-contrast-color2: var(--md-pink-600);
  --jp-icon-contrast-color3: var(--md-blue-600);

  /* Button colors */
  --jp-accept-color-normal: var(--md-blue-700);
  --jp-accept-color-hover: var(--md-blue-800);
  --jp-accept-color-active: var(--md-blue-900);
  --jp-warn-color-normal: var(--md-red-700);
  --jp-warn-color-hover: var(--md-red-800);
  --jp-warn-color-active: var(--md-red-900);
  --jp-reject-color-normal: var(--md-grey-600);
  --jp-reject-color-hover: var(--md-grey-700);
  --jp-reject-color-active: var(--md-grey-800);

  /* File or activity icons and switch semantic variables */
  --jp-jupyter-icon-color: #f37626;
  --jp-notebook-icon-color: #f37626;
  --jp-json-icon-color: var(--md-orange-700);
  --jp-console-icon-background-color: var(--md-blue-700);
  --jp-console-icon-color: white;
  --jp-terminal-icon-background-color: var(--md-grey-800);
  --jp-terminal-icon-color: var(--md-grey-200);
  --jp-text-editor-icon-color: var(--md-grey-700);
  --jp-inspector-icon-color: var(--md-grey-700);
  --jp-switch-color: var(--md-grey-400);
  --jp-switch-true-position-color: var(--md-orange-900);
}
</style>
<style type="text/css">
/* Force rendering true colors when outputing to pdf */
* {
  -webkit-print-color-adjust: exact;
}

/* Misc */
a.anchor-link {
  display: none;
}

/* Input area styling */
.jp-InputArea {
  overflow: hidden;
}

.jp-InputArea-editor {
  overflow: hidden;
}

.cm-editor.cm-s-jupyter .highlight pre {
/* weird, but --jp-code-padding defined to be 5px but 4px horizontal padding is hardcoded for pre.cm-line */
  padding: var(--jp-code-padding) 4px;
  margin: 0;

  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
  color: inherit;

}

.jp-OutputArea-output pre {
  line-height: inherit;
  font-family: inherit;
}

.jp-RenderedText pre {
  color: var(--jp-content-font-color1);
  font-size: var(--jp-code-font-size);
}

/* Hiding the collapser by default */
.jp-Collapser {
  display: none;
}

@page {
    margin: 0.5in; /* Margin for each printed piece of paper */
}

@media print {
  .jp-Cell-inputWrapper,
  .jp-Cell-outputWrapper {
    display: block;
  }
}
</style>
<!-- Load mathjax -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/latest.js?config=TeX-AMS_CHTML-full,Safe"> </script>
<!-- MathJax configuration -->
<script type="text/x-mathjax-config">
    init_mathjax = function() {
        if (window.MathJax) {
        // MathJax loaded
            MathJax.Hub.Config({
                TeX: {
                    equationNumbers: {
                    autoNumber: "AMS",
                    useLabelIds: true
                    }
                },
                tex2jax: {
                    inlineMath: [ ['$','$'], ["\\(","\\)"] ],
                    displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
                    processEscapes: true,
                    processEnvironments: true
                },
                displayAlign: 'center',
                CommonHTML: {
                    linebreaks: {
                    automatic: true
                    }
                }
            });

            MathJax.Hub.Queue(["Typeset", MathJax.Hub]);
        }
    }
    init_mathjax();
    </script>
<!-- End of mathjax configuration --><script type="module">
  document.addEventListener("DOMContentLoaded", async () => {
    const diagrams = document.querySelectorAll(".jp-Mermaid > pre.mermaid");
    // do not load mermaidjs if not needed
    if (!diagrams.length) {
      return;
    }
    const mermaid = (await import("https://cdnjs.cloudflare.com/ajax/libs/mermaid/10.7.0/mermaid.esm.min.mjs")).default;
    const parser = new DOMParser();

    mermaid.initialize({
      maxTextSize: 100000,
      maxEdges: 100000,
      startOnLoad: false,
      fontFamily: window
        .getComputedStyle(document.body)
        .getPropertyValue("--jp-ui-font-family"),
      theme: document.querySelector("body[data-jp-theme-light='true']")
        ? "default"
        : "dark",
    });

    let _nextMermaidId = 0;

    function makeMermaidImage(svg) {
      const img = document.createElement("img");
      const doc = parser.parseFromString(svg, "image/svg+xml");
      const svgEl = doc.querySelector("svg");
      const { maxWidth } = svgEl?.style || {};
      const firstTitle = doc.querySelector("title");
      const firstDesc = doc.querySelector("desc");

      img.setAttribute("src", `data:image/svg+xml,${encodeURIComponent(svg)}`);
      if (maxWidth) {
        img.width = parseInt(maxWidth);
      }
      if (firstTitle) {
        img.setAttribute("alt", firstTitle.textContent);
      }
      if (firstDesc) {
        const caption = document.createElement("figcaption");
        caption.className = "sr-only";
        caption.textContent = firstDesc.textContent;
        return [img, caption];
      }
      return [img];
    }

    async function makeMermaidError(text) {
      let errorMessage = "";
      try {
        await mermaid.parse(text);
      } catch (err) {
        errorMessage = `${err}`;
      }

      const result = document.createElement("details");
      result.className = 'jp-RenderedMermaid-Details';
      const summary = document.createElement("summary");
      summary.className = 'jp-RenderedMermaid-Summary';
      const pre = document.createElement("pre");
      const code = document.createElement("code");
      code.innerText = text;
      pre.appendChild(code);
      summary.appendChild(pre);
      result.appendChild(summary);

      const warning = document.createElement("pre");
      warning.innerText = errorMessage;
      result.appendChild(warning);
      return [result];
    }

    async function renderOneMarmaid(src) {
      const id = `jp-mermaid-${_nextMermaidId++}`;
      const parent = src.parentNode;
      let raw = src.textContent.trim();
      const el = document.createElement("div");
      el.style.visibility = "hidden";
      document.body.appendChild(el);
      let results = null;
      let output = null;
      try {
        let { svg } = await mermaid.render(id, raw, el);
        svg = cleanMermaidSvg(svg);
        results = makeMermaidImage(svg);
        output = document.createElement("figure");
        results.map(output.appendChild, output);
      } catch (err) {
        parent.classList.add("jp-mod-warning");
        results = await makeMermaidError(raw);
        output = results[0];
      } finally {
        el.remove();
      }
      parent.classList.add("jp-RenderedMermaid");
      parent.appendChild(output);
    }


    /**
     * Post-process to ensure mermaid diagrams contain only valid SVG and XHTML.
     */
    function cleanMermaidSvg(svg) {
      return svg.replace(RE_VOID_ELEMENT, replaceVoidElement);
    }


    /**
     * A regular expression for all void elements, which may include attributes and
     * a slash.
     *
     * @see https://developer.mozilla.org/en-US/docs/Glossary/Void_element
     *
     * Of these, only `<br>` is generated by Mermaid in place of `\n`,
     * but _any_ "malformed" tag will break the SVG rendering entirely.
     */
    const RE_VOID_ELEMENT =
      /<\s*(area|base|br|col|embed|hr|img|input|link|meta|param|source|track|wbr)\s*([^>]*?)\s*>/gi;

    /**
     * Ensure a void element is closed with a slash, preserving any attributes.
     */
    function replaceVoidElement(match, tag, rest) {
      rest = rest.trim();
      if (!rest.endsWith('/')) {
        rest = `${rest} /`;
      }
      return `<${tag} ${rest}>`;
    }

    void Promise.all([...diagrams].map(renderOneMarmaid));
  });
</script>
<style>
  .jp-Mermaid:not(.jp-RenderedMermaid) {
    display: none;
  }

  .jp-RenderedMermaid {
    overflow: auto;
    display: flex;
  }

  .jp-RenderedMermaid.jp-mod-warning {
    width: auto;
    padding: 0.5em;
    margin-top: 0.5em;
    border: var(--jp-border-width) solid var(--jp-warn-color2);
    border-radius: var(--jp-border-radius);
    color: var(--jp-ui-font-color1);
    font-size: var(--jp-ui-font-size1);
    white-space: pre-wrap;
    word-wrap: break-word;
  }

  .jp-RenderedMermaid figure {
    margin: 0;
    overflow: auto;
    max-width: 100%;
  }

  .jp-RenderedMermaid img {
    max-width: 100%;
  }

  .jp-RenderedMermaid-Details > pre {
    margin-top: 1em;
  }

  .jp-RenderedMermaid-Summary {
    color: var(--jp-warn-color2);
  }

  .jp-RenderedMermaid:not(.jp-mod-warning) pre {
    display: none;
  }

  .jp-RenderedMermaid-Summary > pre {
    display: inline-block;
    white-space: normal;
  }
</style>
<!-- End of mermaid configuration --></head>
<body class="jp-Notebook" data-jp-theme-light="true" data-jp-theme-name="JupyterLab Light">
<main><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=760ba705-71c0-4e74-866e-25dce1c22245">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [2]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Import required libraries</span>
<span class="kn">import</span> <span class="nn">pandas</span> <span class="k">as</span> <span class="nn">pd</span>
<span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span>
<span class="kn">import</span> <span class="nn">matplotlib.pyplot</span> <span class="k">as</span> <span class="nn">plt</span>
<span class="kn">import</span> <span class="nn">seaborn</span> <span class="k">as</span> <span class="nn">sns</span>

<span class="c1"># Load the dataset</span>
<span class="n">file_path</span> <span class="o">=</span> <span class="s2">"sales.csv"</span>  <span class="c1"># Replace with your file's path</span>
<span class="n">df</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">read_csv</span><span class="p">(</span><span class="n">file_path</span><span class="p">)</span>

<span class="c1"># View the first 5 rows</span>
<span class="n">df</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[2]:</div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div>
<style scoped="">
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
<thead>
<tr style="text-align: right;">
<th></th>
<th>sale_id</th>
<th>branch</th>
<th>city</th>
<th>customer_type</th>
<th>gender</th>
<th>product_name</th>
<th>product_category</th>
<th>unit_price</th>
<th>quantity</th>
<th>tax</th>
<th>total_price</th>
<th>reward_points</th>
</tr>
</thead>
<tbody>
<tr>
<th>0</th>
<td>1</td>
<td>A</td>
<td>New York</td>
<td>Member</td>
<td>Male</td>
<td>Shampoo</td>
<td>Personal Care</td>
<td>5.50</td>
<td>3</td>
<td>1.16</td>
<td>17.66</td>
<td>1</td>
</tr>
<tr>
<th>1</th>
<td>2</td>
<td>B</td>
<td>Los Angeles</td>
<td>Normal</td>
<td>Female</td>
<td>Notebook</td>
<td>Stationery</td>
<td>2.75</td>
<td>10</td>
<td>1.93</td>
<td>29.43</td>
<td>0</td>
</tr>
<tr>
<th>2</th>
<td>3</td>
<td>A</td>
<td>New York</td>
<td>Member</td>
<td>Female</td>
<td>Apple</td>
<td>Fruits</td>
<td>1.20</td>
<td>15</td>
<td>1.26</td>
<td>19.26</td>
<td>1</td>
</tr>
<tr>
<th>3</th>
<td>4</td>
<td>A</td>
<td>Chicago</td>
<td>Normal</td>
<td>Male</td>
<td>Detergent</td>
<td>Household</td>
<td>7.80</td>
<td>5</td>
<td>2.73</td>
<td>41.73</td>
<td>0</td>
</tr>
<tr>
<th>4</th>
<td>5</td>
<td>B</td>
<td>Los Angeles</td>
<td>Member</td>
<td>Female</td>
<td>Orange Juice</td>
<td>Beverages</td>
<td>3.50</td>
<td>7</td>
<td>1.72</td>
<td>26.22</td>
<td>2</td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=c1748fda-b9d3-456c-97e0-5c76b61b3f37">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [3]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Check for missing values</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">"Missing Values:</span><span class="se">\n</span><span class="s2">"</span><span class="p">,</span> <span class="n">df</span><span class="o">.</span><span class="n">isnull</span><span class="p">()</span><span class="o">.</span><span class="n">sum</span><span class="p">())</span>

<span class="c1"># Get a summary of the dataset</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">"</span><span class="se">\n</span><span class="s2">Dataset Summary:"</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="n">df</span><span class="o">.</span><span class="n">describe</span><span class="p">())</span>

<span class="c1"># Check data types</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">"</span><span class="se">\n</span><span class="s2">Data Types:"</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="n">df</span><span class="o">.</span><span class="n">dtypes</span><span class="p">)</span>

<span class="c1"># Rename columns (optional for better readability)</span>
<span class="n">df</span><span class="o">.</span><span class="n">columns</span> <span class="o">=</span> <span class="n">df</span><span class="o">.</span><span class="n">columns</span><span class="o">.</span><span class="n">str</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="o">.</span><span class="n">str</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">" "</span><span class="p">,</span> <span class="s2">"_"</span><span class="p">)</span>

<span class="c1"># Unique values in columns</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">"</span><span class="se">\n</span><span class="s2">Unique Values:"</span><span class="p">)</span>
<span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">df</span><span class="o">.</span><span class="n">columns</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">"</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">df</span><span class="p">[</span><span class="n">column</span><span class="p">]</span><span class="o">.</span><span class="n">nunique</span><span class="p">()</span><span class="si">}</span><span class="s2"> unique values"</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>Missing Values:
 sale_id             0
branch              0
city                0
customer_type       0
gender              0
product_name        0
product_category    0
unit_price          0
quantity            0
tax                 0
total_price         0
reward_points       0
dtype: int64

Dataset Summary:
           sale_id   unit_price     quantity          tax  total_price  \
count  1000.000000  1000.000000  1000.000000  1000.000000  1000.000000   
mean    500.500000    10.836110    10.337000     7.758010   118.583900   
std     288.819436     5.775924     6.029908     6.538066    99.936441   
min       1.000000     1.020000     1.000000     0.080000     1.210000   
25%     250.750000     5.867500     5.000000     2.510000    38.380000   
50%     500.500000    10.615000    10.000000     5.870000    89.705000   
75%     750.250000    15.882500    16.000000    11.522500   176.072500   
max    1000.000000    20.980000    20.000000    28.390000   433.990000   

       reward_points  
count    1000.000000  
mean        6.057000  
std         9.350464  
min         0.000000  
25%         0.000000  
50%         0.000000  
75%        10.000000  
max        43.000000  

Data Types:
sale_id               int64
branch               object
city                 object
customer_type        object
gender               object
product_name         object
product_category     object
unit_price          float64
quantity              int64
tax                 float64
total_price         float64
reward_points         int64
dtype: object

Unique Values:
sale_id: 1000 unique values
branch: 2 unique values
city: 3 unique values
customer_type: 2 unique values
gender: 2 unique values
product_name: 5 unique values
product_category: 5 unique values
unit_price: 787 unique values
quantity: 20 unique values
tax: 755 unique values
total_price: 956 unique values
reward_points: 43 unique values
</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=156433e7-f6d1-44b8-b9e9-fe527436621d">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [19]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Revenue by City</span>
<span class="n">city_revenue</span> <span class="o">=</span> <span class="n">df</span><span class="o">.</span><span class="n">groupby</span><span class="p">(</span><span class="s1">'city'</span><span class="p">)[</span><span class="s1">'total_price'</span><span class="p">]</span><span class="o">.</span><span class="n">sum</span><span class="p">()</span><span class="o">.</span><span class="n">reset_index</span><span class="p">()</span>

<span class="c1"># Bar chart for revenue by city</span>
<span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">8</span><span class="p">,</span> <span class="mi">5</span><span class="p">))</span>
<span class="n">sns</span><span class="o">.</span><span class="n">barplot</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">'city'</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">'total_price'</span><span class="p">,</span> <span class="n">data</span><span class="o">=</span><span class="n">city_revenue</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">"Revenue by City"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">"City"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">"Total Revenue"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>

<span class="c1"># Revenue by Product Category</span>
<span class="n">category_revenue</span> <span class="o">=</span> <span class="n">df</span><span class="o">.</span><span class="n">groupby</span><span class="p">(</span><span class="s1">'product_category'</span><span class="p">)[</span><span class="s1">'total_price'</span><span class="p">]</span><span class="o">.</span><span class="n">sum</span><span class="p">()</span><span class="o">.</span><span class="n">reset_index</span><span class="p">()</span>

<span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">8</span><span class="p">,</span> <span class="mi">5</span><span class="p">))</span>
<span class="n">sns</span><span class="o">.</span><span class="n">barplot</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">'total_price'</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">'product_category'</span><span class="p">,</span> <span class="n">data</span><span class="o">=</span><span class="n">category_revenue</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">"Revenue by Product Category"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">"Total Revenue"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">"Product Category"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAskAAAHWCAYAAACFXRQ+AAAAOnRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjEwLjAsIGh0dHBzOi8vbWF0cGxvdGxpYi5vcmcvlHJYcgAAAAlwSFlzAAAPYQAAD2EBqD+naQAAVE5JREFUeJzt3XlclXX+///nAeTgBq6AJrmWSm6JG2kuSeKSaVlZOYlLNhpayqTmfBw0WyzLrbTMmkRLJ83SKU0MNS0VN5RcMTUcLAU1FdIUFN6/P+bL9etcoIKDHtLH/XY7t0/ner/O+3pd58OZnnPN+7yPwxhjBAAAAMDi4e4GAAAAgOKGkAwAAADYEJIBAAAAG0IyAAAAYENIBgAAAGwIyQAAAIANIRkAAACwISQDAAAANoRkAAAAwIaQDAAoEu3bt1eDBg3c3YaL8ePHy+FwuLsNAH9ChGQAsImJiZHD4bAeXl5euu2229SvXz/98ssv7m4Pki5cuKCpU6eqZcuW8vPzk4+Pj+68804NHTpUP/744xVf+9prr2np0qU3plEAf1oOY4xxdxMAUJzExMSof//+mjBhgmrWrKkLFy5o06ZNiomJUY0aNbR79275+Pi4u81ip3379jp58qR27959Xc9z8uRJde7cWQkJCXrggQcUFhamMmXKaP/+/fr000+VmpqqrKwsSdKlS5d06dIll/9/lSlTRo888ohiYmKua58A/ty83N0AABRXXbp0UbNmzSRJTz/9tCpVqqQ33nhDX375pR577DE3d3fr6tevn3bs2KHFixerV69eLmMvv/yy/u///s967uXlJS8v/lUHoPBYbgEABXTvvfdKkg4dOuRyPCkpSY888ogqVKggHx8fNWvWTF9++aU1vm3bNjkcDs2dOzfPnCtXrpTD4dCyZcusY7/88osGDBiggIAAOZ1O3XXXXfroo49cXrd27Vo5HA4tWrRIr776qqpVqyYfHx917NhRBw8edKmtUaOG+vXrl+fc7du3V/v27V2OZWZmaty4capTp46cTqeCgoI0atQoZWZmFug9kqSEhATdc889KlmypGrWrKlZs2ZZY2fPnlXp0qX1/PPP53ndzz//LE9PT02cOPGyc2/evFnLly/XwIED8wRkSXI6nXrrrbes5/Y1yQ6HQ+fOndPcuXOt5TT9+vXTt99+K4fDoSVLluSZc8GCBXI4HIqPjy/wewDgz4+QDAAFdPjwYUlS+fLlrWN79uxRq1attG/fPr344ouaPHmySpcurZ49e1qBq1mzZqpVq5YWLVqUZ86FCxeqfPnyCg8PlySlpaWpVatWWrVqlYYOHarp06erTp06GjhwoKZNm5bn9a+//rqWLFmiF154QWPGjNGmTZvUp0+fa7q+nJwcPfjgg3rrrbfUvXt3vfPOO+rZs6emTp2q3r17F2iO06dPq2vXrgoJCdGkSZNUrVo1DRkyxAr5ZcqU0UMPPaSFCxcqOzvb5bX/+te/ZIy5Yv+5/+XjqaeeuqZr/Pjjj+V0OnXvvffq448/1scff6y//vWvat++vYKCgjR//vw8r5k/f75q166t0NDQazongD8pAwBwMWfOHCPJrFq1ypw4ccIcOXLELF682FSuXNk4nU5z5MgRq7Zjx46mYcOG5sKFC9axnJwcc88995g77rjDOjZmzBhTokQJc+rUKetYZmamKVeunBkwYIB1bODAgaZKlSrm5MmTLj09/vjjxs/Pz/z+++/GGGO+/fZbI8nUr1/fZGZmWnXTp083ksyuXbusY9WrVzcRERF5rrNdu3amXbt21vOPP/7YeHh4mO+//96lbtasWUaS2bBhwxXft3bt2hlJZvLkyS7X2KRJE+Pv72+ysrKMMcasXLnSSDIrVqxweX2jRo1c+snPQw89ZCSZ06dPX7Eu17hx44z9X3WlS5fO9/0YM2aMcTqd5syZM9ax48ePGy8vLzNu3LgCnQ/AzYM7yQBwGWFhYapcubKCgoL0yCOPqHTp0vryyy9VrVo1SdKpU6e0Zs0aPfbYY/rtt9908uRJnTx5Ur/++qvCw8N14MABazeM3r176+LFi/riiy+s+b/55hudOXPGuktrjNHnn3+u7t27yxhjzXfy5EmFh4crPT1d27dvd+mxf//+8vb2tp7nLgn56aefCn29n332merXr6969eq5nPu+++6TJH377bdXncPLy0t//etfrefe3t7661//quPHjyshIcF6X6tWrepy13b37t3auXOn/vKXv1xx/oyMDElS2bJlC319V9O3b19lZmZq8eLF1rGFCxfq0qVLV+0LwM2HkAwAlzFz5kzFxcVp8eLF6tq1q06ePCmn02mNHzx4UMYY/eMf/1DlypVdHuPGjZMkHT9+XJLUuHFj1atXTwsXLrRev3Dh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2LDB5fiGDRsUHBx81dd7eHjo448/VkhIiDp06KCjR48WugdcHiEZbjVz5kxlZ2erRYsW+vzzz3XgwAHt27dPb7/9tkJDQ69pzjFjxmjr1q169tlntXPnTiUlJem9997TyZMnVb58eVWsWFGzZ8/WwYMHtWbNGkVFRbm8/sknn1ROTo6eeeYZ7du3TytXrtRbb70lSdb/lPXss8/qyJEjGjZsmJKSkvTvf/9b48aNU1RUlDw8+FihcNLT0/PccT1y5MhV/842b96s1157Tdu2bVNKSoq++OILnThxQvXr18/3PP/85z/1yCOPqEGDBi6PgQMH6uTJky7fqL+S+++/X7Vr11ZERIR27typDRs2WN/qz/2M9OnTR5UqVVKPHj30/fffKzk5WWvXrtVzzz2X75KksmXL6oUXXtCIESM0d+5cHTp0SNu3b9c777yjuXPnSpKio6P173//WwcPHtSePXu0bNmyy14rkJ+GDRuqT58+evvtt12Ojx492toWMTExUQcOHNC///1vDR061Kpp1KiRypcvrwULFriE5KVLlyozMzPPkomCGjlypN544w0tXLhQ+/fv14svvqjExEQ9//zzBXq9p6en5s+fr8aNG+u+++5TamrqNfWBfLh5TTRgjh49aiIjI0316tWNt7e3ue2228yDDz5ovv32W2OMcfkyUC4/Pz8zZ84cY0zeL+4ZY8zatWvNPffcY5xOpylXrpwJDw+3xuPi4kz9+vWN0+k0jRo1MmvXrs1zjg0bNphGjRoZb29vExISYhYsWGAkmaSkJJdzNG/e3Hh7e5vAwEAzevRo68tQQEFFREQYSXkeAwcONMZc+e9s7969Jjw83FSuXNk4nU5z5513mnfeeSff82zbts1IMlu2bMl3vEuXLuahhx4yxvz3i3vPP/+8y3iPHj1MRESE9Xzfvn2mdevWxtvb29SrV8989dVXRpKJjY21ao4dO2b69u1rKlWqZJxOp6lVq5YZNGiQ9YUl+5cWc3JyzLRp00zdunVNiRIlTOXKlU14eLhZt26dMcaYl19+2dSvX9+ULFnSVKhQwfTo0cP89NNPBX+zccvJ74uxycnJxtvb29gj0JYtW8z9999vypQpY0qXLm0aNWqU5wt1PXr0MF5eXtYOMtnZ2aZ8+fKmVatWBe6pevXqZurUqdbz7OxsM378eHPbbbeZEiVKmMaNG1tfTM/tV3/44niuP+5uYYwxFy9eNA8//LCpX7++SUtLK3A/uDyHMYX49hRwi5o/f7769++v9PT0q655Bm5FGzZsUJs2bXTw4EFrDScA/JkVfuU4cAuYN2+eatWqpdtuu00//PCDRo8erccee4yADPw/S5YsUZkyZXTHHXfo4MGDev7559W6dWsCMoCbBiEZyEdqaqqio6OVmpqqKlWq6NFHH9Wrr77q7raAYuO3337T6NGjlZKSokqVKiksLEyTJ092d1sAUGRYbgEAAADY8DV8AAAAwIaQDAAAANgQkgEAAAAbQjIAAABgQ0gGAAAAbAjJAAAXDodDS5cudXcbAOBWhGQAuMWkpqZq2LBhqlWrlpxOp4KCgtS9e3etXr1aknTs2DF16dJFknT48GE5HA4lJia6sWMAuPH4MREAuIUcPnxYrVu3Vrly5fTmm2+qYcOGunjxolauXKnIyEglJSUpMDDQ3W0CgNvxYyIAcAvp2rWrdu7cqf3796t06dIuY2fOnFG5cuXkcDi0ZMkS9ezZUw6Hw6WmXbt2mjBhgjp27KgjR464BOrhw4crISFB33///Q25FgC4nlhuAQC3iFOnTik2NlaRkZF5ArIklStXLs+xLVu2SJJWrVqlY8eO6YsvvlDbtm1Vq1Ytffzxx1bdxYsXNX/+fA0YMOC69Q8ANxIhGQBuEQcPHpQxRvXq1SvwaypXrixJqlixogIDA1WhQgVJ0sCBAzVnzhyr7quvvtKFCxf02GOPFW3TAOAmhGQAuEUU5eq6fv366eDBg9q0aZMkKSYmRo899li+d6gB4M+IL+4BwC3ijjvukMPhUFJS0v88l7+/v7p37645c+aoZs2aWrFihdauXfu/NwkAxQR3kgHgFlGhQgWFh4dr5syZOnfuXJ7xM2fO5Dnm7e0tScrOzs4z9vTTT2vhwoWaPXu2ateurdatWxd5zwDgLoRkALiFzJw5U9nZ2WrRooU+//xzHThwQPv27dPbb7+t0NDQPPX+/v4qWbKkYmNjlZaWpvT0dGssPDxcvr6+euWVV9S/f/8beRkAcN0RkgHgFlKrVi1t375dHTp00N/+9jc1aNBA999/v1avXq333nsvT72Xl5fefvttvf/++6patap69OhhjXl4eKhfv37Kzs5W3759b+RlAMB1xz7JAIBrNnDgQJ04cUJffvmlu1sBgCLFF/cAAIWWnp6uXbt2acGCBQRkADclQjIAoNB69OihLVu2aPDgwbr//vvd3Q4AFDmWWwAAAAA2fHEPAAAAsCEkAwAAADaEZAAAAMCGkAwAAADYEJIBAAAAG0IyAAAAYENIBgAAAGwIyQAAAIDN/wejhDVxszRkzAAAAABJRU5ErkJggg=="/>
</div>
</div>
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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1apVSxcuXJCHh4dCQ0NVtmxZzZs37471jhw5UjNnztTmzZslSY8//rgqVKigcePGOfpUr15diYmJ2rZtmySpYMGCev/999WqVStHnw8++EBLlizR+vXr1b17d/36669atWqVYx/vZODAgRo0aFCK9tKvTZCr3fOuywMAgIfblg/bZXYJSGcJCQny9fXVuXPn5OPjc8e+lj3T/8QTT2jbtm3atm2bfv75Z0VERKh+/fo6ePCgtm/frn379ilbtmzy9vaWt7e3cuTIocuXL2v//v2SpDZt2mjt2rX666+/JN04s96wYUP5+flJkrZv367o6GjH8t7e3oqIiFBycrLi4+MddVSoUCFFbbNmzVK1atUUGBgob29v9e3bV4cOHXLMj4uLU6VKlZyW+fv0hQsXtH//fnXq1Mlp+x988IGj/qioKG3btk2FCxdW9+7dtWLFijs+X3369NG5c+ccj8OHD6fh2QYAAMDDLEtmF5BRvLy8VLBgQcf0F198IV9fX33++edKTExU+fLlNX369BTL+fv7S5IqVqyoAgUKaObMmeratavmzZun6OhoR7/ExES99NJL6t69e4p15MuXz6mOv9uwYYPatGmjQYMGKSIiQr6+vpo5c6ZGjRqV6n1LTEyUJH3++eeqXLmy0zxXV1dJUrly5RQfH6+lS5dq1apVat68uerVq6c5c+bccp12u112uz3VNQAAAODRYdnQ/082m00uLi66dOmSypUrp1mzZikgIOCOH4W0adNG06dPV548eeTi4qKGDRs65pUrV067du1yemORGuvXr1dISIjee+89R9vBgwed+hQuXFibNm1Su3b//2O4TZs2OX7OlSuXgoOD9fvvvzuuMbgVHx8ftWjRQi1atNBzzz2nyMhInT59Wjly5EhTzQAAAHi0WTb0X7lyRUePHpUknTlzRuPGjVNiYqKefvppVapUSR9++KGaNGmiwYMHK0+ePDp48KDmzp2rt956S3ny5JF0I/QPHDhQQ4YM0XPPPed0Jvztt9/W448/rm7duqlz587y8vLSrl27tHLlSqex+P8UHh6uQ4cOaebMmapYsaIWL16cYsz/a6+9pi5duqhChQqqWrWqZs2apdjYWOXPn9/RZ9CgQerevbt8fX0VGRmpK1euaPPmzTpz5ozefPNNjR49WkFBQSpbtqxcXFz0zTffKDAw0DE8CQAA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"/>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=2fa7992b-15b1-40d8-8161-1828ec8e322e">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [20]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Sales count by customer type</span>
<span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">8</span><span class="p">,</span> <span class="mi">5</span><span class="p">))</span>
<span class="n">sns</span><span class="o">.</span><span class="n">countplot</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">'customer_type'</span><span class="p">,</span> <span class="n">data</span><span class="o">=</span><span class="n">df</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">"Customer Type Distribution"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">"Customer Type"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">"Count"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>

<span class="c1"># Revenue by Customer Type</span>
<span class="n">customer_revenue</span> <span class="o">=</span> <span class="n">df</span><span class="o">.</span><span class="n">groupby</span><span class="p">(</span><span class="s1">'customer_type'</span><span class="p">)[</span><span class="s1">'total_price'</span><span class="p">]</span><span class="o">.</span><span class="n">sum</span><span class="p">()</span><span class="o">.</span><span class="n">reset_index</span><span class="p">()</span>

<span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">8</span><span class="p">,</span> <span class="mi">5</span><span class="p">))</span>
<span class="n">sns</span><span class="o">.</span><span class="n">barplot</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">'customer_type'</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">'total_price'</span><span class="p">,</span> <span class="n">data</span><span class="o">=</span><span class="n">customer_revenue</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">"Revenue by Customer Type"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">"Customer Type"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">"Total Revenue"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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Y7ioqMjUqVPH3H333S7jpk6dahwOh/n555+tNklGklm/fr3V9ssvvxhfX19zxx13WG2DBg0ytWrVMr/99pvLMe+55x4TFBRkjh8/fs4a69WrZxISEs7aP23aNCPJfPbZZy61VdZ7/s033xhJpkGDBqVqLen75ptvrLabbrrJSDIvv/yy1VZQUGBatWplwsLCTGFhoTHGmNTUVCPJ7N69+0+Pebbayvq9LznPoUOHrLbvv//eVKtWzQwYMMBqGzdunJFkHnjgAZdj3nHHHaZGjRqlzgXg/DEtAUApeXl5kqTq1atX+rGDg4O1Zs0a7d+/v9z7Llq0SBEREerbt6/V5uXlpUcffVT5+flauXKly/i//vWvCgoKsrbbt28v6fe5r2c+7NS+fXsVFhbq119/lSQtXbpUOTk56tu3r3777Tfr5eHhofbt2+ubb74pVduZc04rqlq1aurXr58+//xzHT161Gr/4IMPdMMNN6h+/fou4+Pi4tSmTRtru27duurVq5e++uorFRUVyRijjz76SD179pQxxuVa4uPjlZuba00NqKiSu5hn1vtHF/Kel0hMTJSfn995jfX09NSQIUOsbW9vbw0ZMkTZ2dnKyMiocA1/5sCBA9q4caMGDhyokJAQq71Fixbq2rWrFi1aVGqfhx9+2GW7Y8eOOnTokPXfIIDyI9wCKMXpdEo6d2CpqClTpmjz5s2KjIzU9ddfr/Hjx+vnn38+r31/+eUXNWrUyHoyvkR0dLTVf6a6deu6bJcE3cjIyDLbjxw5Ikn66aefJEmdO3dWaGioy2vJkiXKzs522d/T01N16tQ5r2v4MwMGDNCJEyf0ySefSJJ27NihjIwM9e/fv9TYRo0alWpr3Lixjh8/roMHD+rgwYPKycnRrFmzSl3H/fffL0mlrqW88vPzJZ37H0IX8p6X+GOwP5fatWuXeqCvcePGknRRV+Ao+f07c250iejoaP322286duyYS/sff0evuuoqSf//dxFA+THnFkApTqdTtWvXPu/llBwOR5ntRUVFpdr69Omjjh076pNPPtGSJUv04osvavLkyfr444/Vo0ePC6r7j862PNPZ2s1/H4oqLi6W9Pu824iIiFLj/rjElY+PT6nAXVExMTFq06aNZs+erQEDBmj27Nny9vZWnz59yn2skuu47777lJiYWOaYFi1aXFC9Jb8j11xz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1+qZZ57RhAkTLsoKBqGhoUpLS9P8+fMVExOjSZMm6aWXXqr08+DK5DDmjIU0AQAAgMsYd24BAABgG4RbAAAA2AbhFgAAALZBuAUAAIBtEG4BAABgG4RbAAAA2AbhFgAAALZBuAUAAIBtEG4BAABgG4RbAPiDzMxMDR8+XA0aNJCPj48iIyPVs2dPLV++vFKOv2fPHjkcDm3cuLFSjncprFixQg6H45yvFStWuLtMAJCnuwsAgKpkz5496tChg4KDg/Xiiy+qefPmOnXqlL766islJSVp+/bt7i7xkjh16pS8vLys7RtuuEEHDhywth977DHl5eUpNTXVagsJCbmkNQJAWbhzCwBneOSRR+RwOLR27Vr17t1bjRs3VrNmzTRq1CitXr1aUtl3XnNyclzuXh45ckT9+vVTaGio/Pz81KhRIysI1q9fX5J03XXXyeFwqFOnTpKk4uJiTZgwQXXq1JGPj49atWqlxYsXW+coOe+HH36ojh07ys/PT+3atdOPP/6odevWqW3btgoMDFSPHj108OBBl+t66623FB0dLV9fXzVt2lQzZ84sddx58+bppptukq+vrz744AOX/b29vRUREWG9/Pz85OPjo4iICP3444+KjIzU4cOHXfYZMWKEOnbsKElKS0tTcHCwPv30UzVq1Ei+vr6Kj4/Xvn37XPb57LPP1Lp1a/n6+qpBgwZ69tlndfr06fK8hQCudAYAYIwx5tChQ8bhcJgXXnjhnON2795tJJl///vfVtuRI0eMJPPNN98YY4xJSkoyrVq1MuvWrTO7d+82S5cuNZ9//rkxxpi1a9caSWbZsmXmwIED5tChQ8YYY6ZOnWqcTqf5xz/+YbZv326efPJJ4+XlZX788UeX8zZt2tQsXrzYbN261cTGxpo2bdqYTp06mX/9619mw4YN5pprrjEPP/ywVdvs2bNNrVq1zEcffWR+/vln89FHH5mQkBCTlpbmctyoqChrzP79+8/5M0hMTDS9evWyths3bmymTJlibRcWFpqaNWuad955xxhjTGpqqvHy8jJt27Y1q1atMuvXrzfXX3+9ueGGG6x9vv32W+N0Ok1aWprZtWuXWbJkiYmKijLjx48/Zy0AcCbCLQD815o1a4wk8/HHH59z3PmE2549e5r777//vPc3xpjatWub559/3qWtXbt25pFHHnHZ76233rL6//GPfxhJZvny5VZbcnKyadKkibXdsGFDM2fOHJfjTpw40cTFxbkcd/r06ee87jP9MdxOnjzZREdHW9sfffSRCQwMNPn5+caY38OtJLN69WprzLZt24wks2bNGmOMMbfcckupf1i8//77platWuddFwAwLQEA/ssYU2nHGjp0qObOnatWrVrpySef1KpVq845Pi8vT/v371eHDh1c2jt06KBt27a5tLVo0cL6c3h4uCSpefPmLm3Z2dmSpGPHjmnXrl0aNGiQAgMDrddzzz2nXbt2uRy3bdu25b/Q/xo4cKB27txpTd1IS0tTnz59FBAQYI3x9PRUu3btrO2mTZsqODjYur7vv/9eEyZMcKlz8ODBOnDggI4fP17h2gBcWXigDAD+q1GjRnI4HH/60Fi1ar/fFzgzDJ86dcplTI8ePfTLL79o0aJFWrp0qW655RYlJSXppZdeuuA6z3zQy+FwlNlWXFwsScrPz5ck/f3vf1f79u1djuPh4eGyfWYQLa+wsDD17NlTqampql+/vr788styr56Qn5+vZ599VnfeeWepPl9f3wrXBuDKwp1bAPivkJAQxcfHKyUlRceOHSvVn5OTI0kKDQ2VJJfVA8pa1is0NFSJiYmaPXu2pk+frlmzZkn6/eEsSSoqKrLGOp1O1a5dW999953LMb777jvFxMRU+JrCw8NVu3Zt/fzzz7rmmmtcXiUPtlWWBx98UPPmzdOsWbPUsGHDUnehT58+rfXr11vbO3bsUE5OjqKjoyVJrVu31o4dO0rVec0111j/oACAP8OdWwA4Q0pKijp06KDrr79eEyZMUIsWLXT69GktXbpUr7/+urZt2yY/Pz/FxsZq0qRJql+/vrKzszV27FiX4zzzzDNq06aNmjVrpoKCAi1YsMAKcWFhYfLz89PixYtVp04d+fr6KigoSKNHj9a4cePUsGFDtWrVSqmpqdq4cWOplQvK69lnn9Wjjz6qoKAgde/eXQUFBVq/fr2OHDmiUaNGXdCxzxQfHy+n06nnnntOEyZMKNXv5eWl4cOH69VXX5Wnp6eGDRum2NhYXX/99ZJ+/5nddtttqlu3ru666y5Vq1ZN33//vTZv3qznnnuu0uoEYG/8UxgAztCgQQNt2LBBN998sx5//HFde+216tq1q5YvX67XX3/dGvfOO+/o9OnTatOmjUaMGFEqfHl7e2vMmDFq0aKF/vKXv8jDw0Nz586V9Pvc01dffVVvvvmmateurV69ekmSHn30UY0aNUqPP/64mjdvrsWLF+vzzz9Xo0aNLuiaHnzwQb311ltKTU1V8+bNddNNNyktLa3S79xWq1ZNAwcOVFFRkQYMGFCq39/fX0899ZTuvfdedejQQYGBgZo3b57VHx8frwULFmjJkiVq166dYmNjNW3aNNWrV69S6wRgbw5TmU9QAACuaIMGDdLBgwf1+eefu7SnpaVpxIgR1tQOALhYmJYAALhgubm52rRpk+bMmVMq2ALApUS4BQBcsF69emnt2rV6+OGH1bVrV3eXA+AKxrQEAAAA2AYPlAEAAMA2CLcAAACwDcItAAAAbINwCwAAANsg3AIAAMA2CLcAAACwDcItAAAAbINwCwAAANv4f8VFn7hzgDILAAAAAElFTkSuQmCC"/>
</div>
</div>
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAskAAAHWCAYAAACFXRQ+AAAAOnRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjEwLjAsIGh0dHBzOi8vbWF0cGxvdGxpYi5vcmcvlHJYcgAAAAlwSFlzAAAPYQAAD2EBqD+naQAATzFJREFUeJzt3Xt8z/X///H7e7OTw3sjOxjDnM0hDLMoYhlJKYpS5pDwmcJC7fOpOVWkCJFDPpmKj0MHH5FJCsWcJjmEkD5TzIhtDBvb6/dH371+3q9RW217S7fr5fK+XPZ6Pp+v5+vxetnl7e7l9X6+bYZhGAIAAABgcnF2AQAAAMDNhpAMAAAAWBCSAQAAAAtCMgAAAGBBSAYAAAAsCMkAAACABSEZAAAAsCAkAwAAABaEZAAAAMCCkAwAN5l27dqpYcOGzi4DAP7WCMkAik18fLxsNpv5KlWqlCpXrqy+ffvq559/dnZ5kHT58mW98cYbCgsLk7e3tzw9PVWnTh0NHTpU33//fbEc87vvvtPYsWP1448/Fsv8ztK3b1+H3/cbvfr27evsUgEUQClnFwDg1jd+/HgFBwfr8uXL2rp1q+Lj4/X1119r37598vT0dHZ5f1tnzpxRp06dlJSUpPvuu0+PPfaYypYtq0OHDmnJkiWaN2+esrOzi/y43333ncaNG6d27dqpevXqRT6/swwaNEgRERHm9rFjxxQXF6ennnpKd955p9les2ZNZ5QHoJAIyQCKXefOndW8eXNJ0pNPPqmKFSvq1Vdf1cqVK/XII484ubq/r759++qbb77RBx98oO7duzv0TZgwQf/617+cVNnN7fLly3J3d5eLi+N/xoaHhys8PNzc3rlzp+Li4hQeHq7HH3+8pMsE8CfxuAWAEpd3V+3o0aMO7QcPHlSPHj1UoUIFeXp6qnnz5lq5cqXZv3PnTtlsNi1cuDDfnGvXrpXNZtOqVavMtp9//ln9+/eXv7+/PDw81KBBA73zzjsO+23YsEE2m03Lli3Tyy+/rCpVqsjT01MdOnTQkSNHHMZWr179uv9V3q5dO7Vr186hLSsrS2PGjFGtWrXk4eGhoKAgjR49WllZWQW6RpKUlJSkO+64Q15eXgoODtacOXPMvgsXLqhMmTIaNmxYvv1++uknubq6auLEiTece9u2bVq9erUGDBiQLyBLkoeHh15//fXfPEfp16BtvRu8ZMkShYaGqly5crLb7WrUqJGmT58u6ddHcB5++GFJ0t13320+grBhwwZz/7feeksNGjSQh4eHAgMDFR0drbS0NIdj5D23vWfPHrVt21alS5dWrVq19MEHH0iSNm7cqLCwMHl5ealu3br6/PPP89VemN+PJUuW6IUXXlDlypVVunRpZWRk3PDa3siXX34pm82mjz/+OF/f4sWLZbPZlJiYKOnX61q2bFn98MMPioyMVJkyZRQYGKjx48fLMAyHfXNzczVt2jQ1aNBAnp6e8vf316BBg3Tu3LlC1wjg/yMkAyhxec+ili9f3mzbv3+/WrVqpQMHDuj555/XlClTVKZMGXXr1s0MFc2bN1eNGjW0bNmyfHMuXbpU5cuXV2RkpCTp1KlTatWqlT7//HMNHTpU06dPV61atTRgwABNmzYt3/6TJk3Sxx9/rJEjRyo2NlZbt25V7969/9D55ebm6v7779frr7+url276s0331S3bt30xhtvqGfPngWa49y5c7r33nsVGhqqyZMnq0qVKhoyZIgZ4sqWLasHH3xQS5cuVU5OjsO+//nPf2QYxm/Wn/ePjyeeeOIPneONrFu3To8++qjKly+vV199VZMmTVK7du20efNmSdJdd92lZ555RpL0z3/+U++9957ee+891a9fX5I0duxYRUdHKzAwUFOmTFH37t01d+5cdezYUVeuXHE41rlz53TfffcpLCxMkydPloeHh3r16qWlS5eqV69euvfeezVp0iRlZmaqR48eOn/+vLlvYX8/JkyYoNWrV2vkyJF65ZVX5O7uXuhr065dOwUFBWnRokX5+hYtWqSaNWs63InOyclRp06d5O/vr8mTJys0NFRjxozRmDFjHPYdNGiQRo0apdatW2v69Onq16+fFi1apMjIyHzXDEAhGABQTBYsWGBIMj7//HPj9OnTxvHjx40PPvjA8PX1NTw8PIzjx4+bYzt06GA0atTIuHz5stmWm5tr3HHHHUbt2rXNttjYWMPNzc04e/as2ZaVlWX4+PgY/fv3N9sGDBhgVKpUyThz5oxDTb169TK8vb2NixcvGoZhGF9++aUhyahfv76RlZVljps+fbohydi7d6/ZVq1aNSMqKirfebZt29Zo27atuf3ee+8ZLi4uxldffeUwbs6cOYYkY/Pmzb953dq2bWtIMqZMmeJwjk2a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jIyMfO3ff/+9fH19i6QoAAAAwJkKHZLvv/9+jR8/XleuXJEk2Ww2JScn67nnnlP37t2LvEAAAACgpBU6JE+ZMkUXLlyQn5+fLl26pLZt26pWrVoqV66cXn755eKoEQAAAChRhV7dwtvbW+vWrdPXX3+tPXv26MKFC2rWrJkiIiKKoz4AAACgxBU6JB8/flxBQUFq06aN2rRpUxw1AQAAAE5V6MctqlevrrZt2+rtt9/WuXPniqMmAAAAwKkKHZJ37typli1bavz48apUqZK6deumDz74QFlZWcVRHwAAAFDiCh2SmzZtqtdee03Jyclas2aNfH199dRTT8nf31/9+/cvjhoBAACAElXokJzHZrPp7rvv1ttvv63PP/9cwcHBWrhwYVHWBgAAADjFHw7JP/30kyZPnqwmTZqoZcuWKlu2rGbNmlWUtQEAAABOUejVLebOnavFixdr8+bNqlevnnr37q3//ve/qlatWnHUBwAAAJS4Qofkl156SY8++qhmzJih22+/vThqAgAAAJyq0CE5OTlZNputOGoBAAAAbgqFfibZZrPpq6++0uOPP67w8HD9/PPPkqT33ntPX3/9dZEXCAAAAJS0QofkDz/8UJGRkfLy8tI333xjro+cnp6uV155pcgLBAAAAEpaoUPySy+9pDlz5ujtt9+Wm5ub2d66dWvt2rWrSIsDAAAAnKHQIfnQoUO666678rV7e3srLS2tKGoCAAAAnKrQITkgIEBHjhzJ1/7111+rRo0aRVIUAAAA4EyFDskDBw7UsGHDtG3bNtlsNp04cUKLFi3SyJEjNWTIkOKoEQAAAChRhV4C7vnnn1dubq46dOigixcv6q677pKHh4dGjhypp59+ujhqBAAAAEpUoUOyzWbTv/71L40aNUpHjhzRhQsXFBISorJly+rSpUvy8vIqjjoBAACAElPoxy3yuLu7KyQkRC1btpSbm5umTp2q4ODgoqwNAAAAcIoCh+SsrCzFxsaqefPmuuOOO7RixQpJ0oIFCxQcHKw33nhDI0aMKK46AQAAgBJT4Mct4uLiNHfuXEVERGjLli16+OGH1a9fP23dulVTp07Vww8/LFdX1+KsFQAAACgRBQ7Jy5cv17vvvqv7779f+/btU+PGjXX16lV9++23stlsxVkjAAAAUKIK/LjFTz/9pNDQUElSw4YN5eHhoREjRhCQ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LVtq/Pjxaty4sa5evap169Zp9uzZOnDggLy8vNSqVStNmjRJwcHBSk1N1QsvvOAwT1xcnEJDQ9WgQQNlZWVp1apVZhj08/OTl5eXEhISVKVKFXl6esrb21ujRo3SmDFjVLNmTTVp0kQLFizQ7t278600UVjjxo3TM888I29vb3Xq1ElZWVnauXOnzp07p5iYmD8197UiIyNlt9v10ksvafz48fn63dzc9PTTT2vGjBkqVaqUhg4dqlatWqlly5aSfr1m9913n6pWraoePXrIxcVF3377rfbt26eXXnqpyOoEcOvjn9UAUMRq1KihXbt26e6779azzz6rhg0b6p577tH69es1e/Zsc9w777yjq1evKjQ0VMOHD88X4tzd3RUbG6vGjRvrrrvukqurq5YsWSLp12dzZ8yYoblz5yowMFAPPPCAJOmZZ55RTEyMnn32WTVq1EgJCQlauXKlateu/afO6cknn9T8+fO1YMECNWrUSG3btlV8fHyR30l2cXFR3759lZOToz59+uTrL126tJ577jk99thjat26tcqWLaulS5ea/ZGRkVq1apU+++wztWjRQq1atdIbb7yhatWqFWmdAG59NqMoP2UCAMCfNGDAAJ0+fVorV650aI+Pj9fw4cPNR1YAoDjxuAUA4KaQnp6uvXv3avHixfkCMgCUNEIyAOCm8MADD2j79u0aPHiw7rnnHmeXA+BvjsctAAAAAAs+uAcAAABYEJIBAAAAC0IyAAAAYEFIBgAAACwIyQAAAIAFIRkAAACwICQDAAAAFoRkAAAAwOL/AZLnfekaD+tcAAAAAElFTkSuQmCC"/>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=0f82583d-edca-46f8-bdd0-6e7c95066416">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [13]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Prepare features for clustering</span>
<span class="n">clustering_data</span> <span class="o">=</span> <span class="n">df</span><span class="p">[[</span><span class="s1">'total_price'</span><span class="p">,</span> <span class="s1">'quantity'</span><span class="p">]]</span><span class="o">.</span><span class="n">copy</span><span class="p">()</span>

<span class="c1"># Standardize the data (important for K-Means)</span>
<span class="kn">from</span> <span class="nn">sklearn.preprocessing</span> <span class="kn">import</span> <span class="n">StandardScaler</span>

<span class="n">scaler</span> <span class="o">=</span> <span class="n">StandardScaler</span><span class="p">()</span>
<span class="n">clustering_data_scaled</span> <span class="o">=</span> <span class="n">scaler</span><span class="o">.</span><span class="n">fit_transform</span><span class="p">(</span><span class="n">clustering_data</span><span class="p">)</span>

<span class="c1"># Check scaled data</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">"Scaled Data:</span><span class="se">\n</span><span class="s2">"</span><span class="p">,</span> <span class="n">clustering_data_scaled</span><span class="p">[:</span><span class="mi">5</span><span class="p">])</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>Scaled Data:
 [[-1.01038619 -1.21737699]
 [-0.8925524  -0.05591605]
 [-0.994368    0.77369891]
 [-0.76941259 -0.885531  ]
 [-0.92468889 -0.55368502]]
</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=03a8f5a5-38f2-42f8-a032-8eeb2e07f511">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [14]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="kn">from</span> <span class="nn">sklearn.cluster</span> <span class="kn">import</span> <span class="n">KMeans</span>

<span class="c1"># Find the optimal number of clusters using the Elbow Method</span>
<span class="n">inertia</span> <span class="o">=</span> <span class="p">[]</span>
<span class="n">k_range</span> <span class="o">=</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">10</span><span class="p">)</span>

<span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="n">k_range</span><span class="p">:</span>
    <span class="n">kmeans</span> <span class="o">=</span> <span class="n">KMeans</span><span class="p">(</span><span class="n">n_clusters</span><span class="o">=</span><span class="n">k</span><span class="p">,</span> <span class="n">random_state</span><span class="o">=</span><span class="mi">42</span><span class="p">)</span>
    <span class="n">kmeans</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="n">clustering_data_scaled</span><span class="p">)</span>
    <span class="n">inertia</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">kmeans</span><span class="o">.</span><span class="n">inertia_</span><span class="p">)</span>

<span class="c1"># Plot the Elbow Curve</span>
<span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">8</span><span class="p">,</span> <span class="mi">5</span><span class="p">))</span>
<span class="n">plt</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">k_range</span><span class="p">,</span> <span class="n">inertia</span><span class="p">,</span> <span class="n">marker</span><span class="o">=</span><span class="s1">'o'</span><span class="p">,</span> <span class="n">linestyle</span><span class="o">=</span><span class="s1">'--'</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">"Elbow Method for Optimal Clusters"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">"Number of Clusters (k)"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">"Inertia"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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"/>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=639f6388-82fc-487d-96a6-d66e73d6a2a0">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [15]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Train K-Means with optimal clusters</span>
<span class="n">kmeans</span> <span class="o">=</span> <span class="n">KMeans</span><span class="p">(</span><span class="n">n_clusters</span><span class="o">=</span><span class="mi">3</span><span class="p">,</span> <span class="n">random_state</span><span class="o">=</span><span class="mi">42</span><span class="p">)</span>
<span class="n">df</span><span class="p">[</span><span class="s1">'cluster'</span><span class="p">]</span> <span class="o">=</span> <span class="n">kmeans</span><span class="o">.</span><span class="n">fit_predict</span><span class="p">(</span><span class="n">clustering_data_scaled</span><span class="p">)</span>

<span class="c1"># Visualize the Clusters</span>
<span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">8</span><span class="p">,</span> <span class="mi">5</span><span class="p">))</span>
<span class="n">sns</span><span class="o">.</span><span class="n">scatterplot</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">'total_price'</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">'quantity'</span><span class="p">,</span> <span class="n">hue</span><span class="o">=</span><span class="s1">'cluster'</span><span class="p">,</span> <span class="n">data</span><span class="o">=</span><span class="n">df</span><span class="p">,</span> <span class="n">palette</span><span class="o">=</span><span class="s2">"Set1"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">"Customer Segments"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">"Total Price"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">"Quantity"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">legend</span><span class="p">(</span><span class="n">title</span><span class="o">=</span><span class="s2">"Cluster"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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"/>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=338de40f-9fe7-4460-88b9-b92fa1bb7ddf">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [16]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="kn">from</span> <span class="nn">sklearn.model_selection</span> <span class="kn">import</span> <span class="n">train_test_split</span>
<span class="kn">from</span> <span class="nn">sklearn.linear_model</span> <span class="kn">import</span> <span class="n">LinearRegression</span>
<span class="kn">from</span> <span class="nn">sklearn.metrics</span> <span class="kn">import</span> <span class="n">r2_score</span><span class="p">,</span> <span class="n">mean_squared_error</span>

<span class="c1"># Encode categorical variables</span>
<span class="n">df_encoded</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">get_dummies</span><span class="p">(</span><span class="n">df</span><span class="p">,</span> <span class="n">columns</span><span class="o">=</span><span class="p">[</span><span class="s1">'product_category'</span><span class="p">,</span> <span class="s1">'customer_type'</span><span class="p">,</span> <span class="s1">'city'</span><span class="p">],</span> <span class="n">drop_first</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>

<span class="c1"># Select features and target</span>
<span class="n">X</span> <span class="o">=</span> <span class="n">df_encoded</span><span class="p">[[</span><span class="s1">'quantity'</span><span class="p">,</span> <span class="s1">'unit_price'</span><span class="p">]</span> <span class="o">+</span> <span class="nb">list</span><span class="p">(</span><span class="n">df_encoded</span><span class="o">.</span><span class="n">columns</span><span class="p">[</span><span class="n">df_encoded</span><span class="o">.</span><span class="n">columns</span><span class="o">.</span><span class="n">str</span><span class="o">.</span><span class="n">contains</span><span class="p">(</span><span class="s1">'product_category'</span><span class="p">)])]</span>
<span class="n">y</span> <span class="o">=</span> <span class="n">df_encoded</span><span class="p">[</span><span class="s1">'total_price'</span><span class="p">]</span>

<span class="c1"># Split data</span>
<span class="n">X_train</span><span class="p">,</span> <span class="n">X_test</span><span class="p">,</span> <span class="n">y_train</span><span class="p">,</span> <span class="n">y_test</span> <span class="o">=</span> <span class="n">train_test_split</span><span class="p">(</span><span class="n">X</span><span class="p">,</span> <span class="n">y</span><span class="p">,</span> <span class="n">test_size</span><span class="o">=</span><span class="mf">0.2</span><span class="p">,</span> <span class="n">random_state</span><span class="o">=</span><span class="mi">42</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=a86b45d8-bba3-4316-bda0-fddaf955860b">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [17]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Train Linear Regression Model</span>
<span class="n">model</span> <span class="o">=</span> <span class="n">LinearRegression</span><span class="p">()</span>
<span class="n">model</span><span class="o">.</span><span class="n">fit</span><span class="p">(</span><span class="n">X_train</span><span class="p">,</span> <span class="n">y_train</span><span class="p">)</span>

<span class="c1"># Predict on test data</span>
<span class="n">y_pred</span> <span class="o">=</span> <span class="n">model</span><span class="o">.</span><span class="n">predict</span><span class="p">(</span><span class="n">X_test</span><span class="p">)</span>

<span class="c1"># Evaluate the model</span>
<span class="n">r2</span> <span class="o">=</span> <span class="n">r2_score</span><span class="p">(</span><span class="n">y_test</span><span class="p">,</span> <span class="n">y_pred</span><span class="p">)</span>
<span class="n">rmse</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">sqrt</span><span class="p">(</span><span class="n">mean_squared_error</span><span class="p">(</span><span class="n">y_test</span><span class="p">,</span> <span class="n">y_pred</span><span class="p">))</span>

<span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">"R² Score: </span><span class="si">{</span><span class="n">r2</span><span class="si">:</span><span class="s2">.2f</span><span class="si">}</span><span class="s2">"</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">"Root Mean Squared Error: </span><span class="si">{</span><span class="n">rmse</span><span class="si">:</span><span class="s2">.2f</span><span class="si">}</span><span class="s2">"</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>R² Score: 0.87
Root Mean Squared Error: 38.67
</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=91a2eea6-dba8-4894-9d9f-a5bd38cce751">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [ ]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span> 
</pre></div>
</div>
</div>
</div>
</div>
</div>
</main>
</body>
</html>



