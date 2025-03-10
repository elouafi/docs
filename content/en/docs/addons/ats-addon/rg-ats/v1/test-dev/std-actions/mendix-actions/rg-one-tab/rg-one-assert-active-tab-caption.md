---
title: "Assert Active Tab Caption"
url: /addons/ats-addon/rg-one-assert-active-tab-caption/
---

## 1 Description

Asserts a given value for the caption of the active tab page.

## 2 Supported widgets

* TabContainer

## 3 Usage

Pass the tab widget name and the tab caption  you want to assert as parameter for the action.
Optionally you can provide a WebElement as search context, to narrow down the search for the tab widget, if there are two or more tab widgets with the same name.

## 4 Input Parameters

Name | Datatype | Required | Description
--- | --- | --- | ---
Widget Name | String | yes | The name of the tab widget
Tab Caption | String | yes | The caption of the tab
Search Context | WebElement | no | Limit the search for the DataGrid row to the given WebElement
