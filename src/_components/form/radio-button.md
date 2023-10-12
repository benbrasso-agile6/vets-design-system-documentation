---
layout: component
permalink: /components/form/radio-button
has-parent: /components/form/
title: Radio button
research-title: Form controls
intro-text: Radio buttons allow users to select exactly one choice from a group.
sketch-link: https://www.sketch.com/s/a52734dd-00d0-44f1-9c9e-ff4016130e5c/p/AF7CD21C-2DF3-4CA4-B678-473A929B9615/canvas
status: use-deployed
uswds-v3: default
web-component: va-radio
anchors:
  - anchor: Examples - v1
  - anchor: Examples - v3
  - anchor: Usage
  - anchor: How to use
  - anchor: Code usage
  - anchor: Accessibility considerations
---

## Examples - v1

### Default

{% include storybook-preview.html story="components-va-radio--default" link_text="va-radio" %}

### Hint text

{% include storybook-preview.html story="components-va-radio--with-hint-text" link_text="va-radio with hint text" %}

### Label header

{% include storybook-preview.html story="components-va-radio--label-header" link_text="va-radio with label header" %}

### Description text

{% include storybook-preview.html story="components-va-radio--with-description-text" link_text="va-radio with description text" %}

### Tile

{% include storybook-preview.html height="250px" story="components-va-radio--tile" link_text="va-radio tile" %}

### Error

{% include storybook-preview.html story="components-va-radio--error" link_text="va-radio error" %}

### Internationalization

{% include storybook-preview.html height="200px" story="components-va-radio--internationalization" link_text="va-radio internationalization" %}

## Examples - v3

### Default

{% include storybook-preview.html height="300px" story="uswds-va-radio--default" link_text="va-radio v3 default and additional variations" %}

## Usage

<a class="vads-c-action-link--blue" href="https://designsystem.digital.gov/components/radio-buttons/">Refer to the U.S. Web Design System for usage guidance</a>

### Choosing between variations

* Use the [Hint text](#hint-text) variation to provide additional information that pertains to the question being asked or all of the options presented.
* Use the [Label header](#label-header) variation when a heading is required within the `legend` that acts as a label for the radio buttons. This can aid users in navigating the form questions, particularly in the [sub-task pattern]({{ site.baseurl }}/patterns/help-users-to/complete-a-sub-task)
* Use the [Description text](#description-text) variation to provide additional details about one or more radio button options. This variation is superseded by the Tile variation.
* Use the [Tile](#tile) variation to provide additional details about one or more radio button options within a large and well defined tap target. 

### Errors

* Radio buttons typically appear inside of `<fieldset>`s. The class name of `usa-input-error` may be placed on the `<fieldset>` that contains all of the radio buttons.
* The error message is placed just below the `<legend>`.
* See [form error handling]({{ site.baseurl }}/components/form/#error-handling) for additional guidance.

{% include snippet.html content='html/error-radio-buttons.html' %}

{% include component-docs.html component_name=page.web-component %}

## Accessibility considerations

<a class="vads-c-action-link--blue" href="https://designsystem.digital.gov/components/radio-buttons/#accessibility-radio-buttons">Refer to the U.S. Web Design System for accessibility guidance</a>