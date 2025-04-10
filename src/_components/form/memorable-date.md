---
layout: component
permalink: /components/form/memorable-date
has-parent: /components/form/
title: Memorable date
research-title: Memorable Date
intro-text: "Three text fields are the easiest way for users to enter most dates."
status: use-with-caution-available
sketch-link: https://www.sketch.com/s/610156b6-f281-4497-81f3-64454fc72156/p/F8230127-0500-4C1A-BBBB-821299A5BDFF/
web-component: va-memorable-date
anchors:
  - anchor: Examples
  - anchor: Usage
  - anchor: How to use
  - anchor: Code usage
  - anchor: Accessibility considerations
  - anchor: Component checklist
---

## Examples

### Default

{% include storybook-preview.html height="200px" story="components-va-memorable-date--default" link_text="va-memorable-date" %}

### Extra hint text

{% include storybook-preview.html height="200px" story="components-va-memorable-date--extra-hint-text" link_text="va-memorable-date with extra hint text" %}

### Custom validation

{% include storybook-preview.html height="200px" story="components-va-memorable-date--custom-validation" link_text="va-memorable-date with custom validation" %}

### Error

{% include storybook-preview.html height="200px" story="components-va-memorable-date--error" link_text="va-memorable-date error" %}

### Internationalization

{% include storybook-preview.html height="200px" story="components-va-memorable-date--internationalization" link_text="va-memorable-date internationalization" %}

## Usage

### When to use date inputs
- Appropriate for most dates.

### When to consider something else

- Consider a date picker for scheduling. If users are trying to schedule something, the date picker might make more sense. Be sure to also provide an option for text entry as well.

**Note:** We do not currently have a calendar picker as part of the design system. For reference, visit the VA online scheduling tool (VAOS) to see an experimental version of a calendar picker. 

### Usability Guidance
- Label each field. Be sure each field is properly labeled — some countries enter dates in day, month, year order.
- Avoid select elements. It may be tempting to switch all or some of these text fields to select elements, but these tend to be more difficult to use than text boxes.

### How to use date inputs

- The year input is set to accept only a four-digit number while the month and day inputs can accept up to a two-digit number.
- Always use back-end validation on dates for correctness.

{% include component-docs.html component_name=page.web-component %}

## Accessibility considerations

- Follow input guidance. These text fields should follow the accessibility guidelines for all text inputs.
- Don’t auto-advance focus. Do not use JavaScript to auto advance the focus from one field to the next. This makes it difficult for keyboard-only users to navigate and correct mistakes.
- Use “text” instead of “number” inputs. Research indicates that numeric inputs still carry many usability problems, according to the gov.uk Technology in Government blog.

{% include _component-checklist.html component_name=page.web-component %}