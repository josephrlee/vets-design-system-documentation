---
layout: component
title: "Featured content"
status: use-deployed
intro-text: "The featured content component helps Veterans quickly identify must-read information on a page. Use this component to highlight a small chunk of the most important information on a page, like eligibility criteria or coverage under a particular VA benefit."
sketch-link: https://www.sketch.com/s/610156b6-f281-4497-81f3-64454fc72156/p/5D59FDA9-A9F3-492C-AF41-F48CF5117F04
anchors:
  - anchor: Examples
  - anchor: Usage
  - anchor: Variations
  - anchor: Code usage
  - anchor: Content considerations
  - anchor: Accessibility considerations
web-component: va-featured-content
---

## Examples

{% include storybook-preview.html height="250px" story="components-va-featured-content--default" link_text="va-featured-content" %}

## Usage

### When to use featured content

* **Highlight the most important information.** The Featured content component is for calling out key details that readers shouldn’t miss. It was originally intended to hold eligibility data exclusively. The content should be "evergreen", not time sensitive.

### When to consider something else

* **Basic overview information.** This component is not intended for basic overview information.
* **Related content.** Don't use this component to highlight related information on, and drive Veterans to, other pages. Use [related or major links]({{ site.baseurl }}/components/link/collection#related-links), [media cards]({{ site.baseurl }}/components/card#media), or stories (depending on template options) instead for this purpose.
* **Table of contents.** Do not use a Featured content component for a table of contents. Use the [On this page]({{ site.baseurl }}/components/on-this-page) component instead for in-page navigation.
* **Dynamic highlight.** If you're highlighting something that was dynamically added to the page in response to a user action, use a variation of an [Alert]({{ site.baseurl }}/components/alert) component.
* **Time sensitive.** If you have a message that will appear only for a defined period of time, use an [Alert]({{ site.baseurl }}/components/alert) component instead.
* **Sibling content.** Use [accordions]({{ site.baseurl }}/components/accordion) to hold chunks of sibling content. For example, accordions are used in forms on the review screen.
* **Additional context.** To reveal helpful background information in a form use the  [Additional information]({{ site.baseurl }}/components/additional-info) component. Additional info is especially useful when the content is closely tied to a particular message or input on the screen. The lighter design prevents breaking up the visual progression as the user navigates the form. These can also serve as alternative to where accordions feel too heavy.

### Placement

Featured content is found towards the top of the page after the h1 title of the page and [intro text]({{ site.baseurl }}/foundation/typography#paragraphs). 

### How to use the Featured content component 

* Features should use a `h3` or `h4` heading depending on what the appropriate heading level is for your page based on the content of your page. 
* Also supports open text, such as `<p>`, `<ul>`, and `<ol>`, `<strong>`, `<em>`, and `<a>`

## Variations

### Instances of this component in production

#### Eligibility

{% include component-example.html alt="An example of an eligibility featured content block in the Health care eligibility page." file="/images/components/featured-content/eligibility.png" caption="The featured content block is mainly intended for use in highlighting eligibility on VA.gov." width="75%" %}

{% capture example_like_this_1 %}
  {% include component-example.html alt="Example of the Link, Collection, Related links component to show a list of links." file="/images/components/link/collection-major.png" caption="Use the Major links variation of the Link - Collection component for a collection of links." %}
{% endcapture %}

{% capture example_not_this_1 %}
  {% include component-example.html alt="An example of a Featured content triptych." file="/images/components/featured-content/triptych.png" caption="Use of this component is not recommended to replace a Card component." %}
{% endcapture %}

{% include _like-this-not-this.html like_this=example_like_this_1 not_this=example_not_this_1 %}

{% capture example_like_this_2 %}
  {% include component-example.html alt="Example of the Related link component to show a list of links." file="/images/components/link/collection-related.png" caption="Use the Related links variation of the Link - Collection component for a collection of links." reverse=true %}
{% endcapture %}

{% capture example_not_this_2 %}
  {% include component-example.html alt="An example of a spotlight content block in the VA Pittsburgh health care page." file="/images/components/featured-content/spotlight.png" caption="Use of this component is not recommended for linking to related content." %}
{% endcapture %}

{% include _like-this-not-this.html like_this=example_like_this_2 not_this=example_not_this_2 %}

## Code usage

Code for this component is shown in Storybook. Follow the link provided in [examples](#examples).

## Content considerations

* **Keep content brief.** If there are more than 5 bullet points, the bullet points are longer than 20 words, or the bullet points require a header, image or button consider using simple body text, headings, and lists instead.