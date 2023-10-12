---
layout: component
permalink: /components/form/number-input
has-parent: /components/form/
title: Number input
research-title: Form controls
sketch-link: https://www.sketch.com/s/a52734dd-00d0-44f1-9c9e-ff4016130e5c/p/4C89A45B-E8D8-44ED-B79A-E64F34303F03/canvas
intro-text: "Number input elements are used for numeric inputs."
status: use-deployed
uswds-v3: default
web-component: va-number-input
anchors:
  - anchor: Examples
  - anchor: Usage
  - anchor: How to use
  - anchor: Code usage
  - anchor: Accessibility considerations
---

## Examples

<va-alert
    class="vads-u-margin-bottom--1"
    close-btn-aria-label="Close notification"
    disable-analytics="false"
    full-width="false"
    slim
    status="warning"
    uswds
    visible="true"
  >
    <React.Fragment key=".0">
      <p class="vads-u-margin-y--0">
        The v1 and v3 variations of this component are identical, excluding the Currency variation which will be added to v3 at a later date. This component does not exist in the USWDS. Teams should switch to the v3 variation in preparation for global color and typography changes that the v3 variation will accept. 
      </p>
    </React.Fragment>
  </va-alert>

### Default

{% include storybook-preview.html story="uswds-va-number-input--default" link_text="va-number-input v3 default" %}

### Currency

{% include storybook-preview.html story="components-va-number-input--with-currency" link_text="va-number-input with currency" %}

### Hint text

{% include storybook-preview.html story="uswds-va-number-input--with-hint-text" link_text="va-number-input with hint text v3" %}

### Valid range

{% include storybook-preview.html story="uswds-va-number-input--valid-range" link_text="va-number-input v3 with valid range" %}

### Error

{% include storybook-preview.html story="uswds-va-number-input--error" link_text="va-number-input v3 error" %}

### Required

{% include storybook-preview.html story="uswds-va-number-input--required" link_text="va-number-input v3 required" %}

### Internationalization

{% include storybook-preview.html story="uswds-va-number-input--internationalization" link_text="va-number-input v3 internationalization" %}

### Widths

{% include storybook-preview.html story="uswds-va-number-input--widths" link_text="va-number-input v3 widths" height="800px" %}

## Usage

### When to use number input

- When a number should be the only accepted value within an input element.
- If you can’t reasonably predict a user’s answer to a prompt and there might be wide variability in users’ answers.
- When users want to be able to paste in a response.

### When to consider something else

- When users are choosing from a specific set of options.
- A number is not the only accepted value for the input. 
- The number should be a type other than number, ie: telephone numbers

### How to use 

- Number input always has the type of `number` and provides a `min` and `max` attribute to set a range on the component. 
- Only show error validation messages or stylings after a user has interacted with a particular field.
- Avoid using placeholder text that appears within a input field before a user starts typing. If placeholder text is no longer visible after a user clicks into the field, users will no longer have that text available when they need to review their entries. (People who have cognitive or visual disabilities have additional problems with placeholder text.)

### Choosing between variations

* **Error.** Highlights the text input field where the user has made an error that needs to be corrected.
* **Required.** Indicates to the user that the text input field is required in order to submit the form.
* **With Hint Text.** Provides a short hint to the user on what to enter into the field.
* **Valid Range.** A combination of a max and min value indicating an acceptable number range of what can be entered into the field.
* **Internationalization.** Demonstrates how this components changes when used with the language toggle.
* **With Currency.** Indicates to the user the expected input is US currency.
* **Widths.** Indicates to the user the expected length of text input by sizing the field relative to what is expected.

### Native Events

- Native onInput and onBlur events are available on this component. They can be used by adding the event handler to your component and it will then listen to the event and respond accordingly when the event fires.

{% include component-docs.html component_name=page.web-component %}

## Accessibility considerations

- Avoid `placeholder` text for accessibility reasons. Most browsers’ default rendering of placeholder text does not provide a high enough contrast ratio.
- Avoid breaking numbers with distinct sections (such as phone numbers, Social Security Numbers, or credit card numbers) into separate input fields. For example, use one input for phone number, not three (one for area code, one for local code, and one for number). Each field needs to be labeled for a screen reader and the labels for fields broken into segments are often not meaningful.
