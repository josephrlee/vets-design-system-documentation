---
layout: component
title: Pagination
status: use-deployed
sketch-link: https://www.sketch.com/s/610156b6-f281-4497-81f3-64454fc72156/p/ABBAABE0-2108-4DBA-8FF5-01F00A06F082/canvas
intro-text: "Pagination is navigation for paginated content."
anchors:
  - anchor: Examples
  - anchor: Usage
  - anchor: Code usage
web-component: va-pagination
---

## Example

{% include storybook-preview.html story="components-va-pagination--default" link_text="va-pagination" %}

## Usage

### When to use pagination

* When it is not feasible to show all ordered data on a single page. Examples of content that should be paginated include search results or other multi-page collections of related items. 

### When to consider something else

* If your content has meaningful groupings or categories.
* Steps in a sequence
* Short collections
* When it is undesirable to have the user pause for navigation. Some alternatives include the infinite scroll pattern or simple un-numbered navigation.

{% include component-docs.html component_name=page.web-component %}