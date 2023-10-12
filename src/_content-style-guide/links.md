---
layout: content-style-guide
title: Links
intro-text: Links should tell our audience what action to take, where to go next, or what information to expect when they select the link.
anchors:
  - anchor: Considerations
  - anchor: Link text
  - anchor: Formatting
  - anchor: Linking to documents and other file sources
  - anchor: Linking to external sites
---

## Considerations

* We use links to connect Veterans with related information that may be helpful. 
* We also use links to help us centralize information, rather than repeating content in multiple places. This helps us update content more efficiently and keep content accurate.
* Too many embedded links can be distracting or overwhelming to people with traumatic brain injuries or other cognitive impairments.
* External links can be disorienting for all people, but especially people who use screen readers. We want to be clear about where links are taking people.
* For issues not covered in this style guide, refer to the U.S. Web Design System (USWDS) on links. [Review link guidance on the USWDS website]({{ site.uswds_link }}/components/link/)

## Link text

* Use natural and descriptive language.
* Describe the purpose of the link and the destination if it’s taking the reader outside of VA.gov.
* Don’t make the link so long that the relevant words get lost.
* Avoid "Click here," since not all people are physically clicking links. 
* Avoid generic link text like "Learn more" and "Read more" by themselves.
* Avoid using words that assume certain abilities, like "See," "Hear," and "Watch."

<div class="do-dont">
<div class="do-dont__do">
<h3 class="do-dont__heading">Like this</h3>
<div class="do-dont__content" markdown="1">
  
__Use natural language, and link relevant words__
  
If your disability gets worse, you can file for an increase in compensation.  
[File for a VA disability compensation increase](https://va.gov/disability/how-to-file-claim/)
  
Apply for a United States burial flag to place over a casket or coffin, or place with an urn.  
[Learn more about burial flags](https://www.va.gov/burials-memorials/memorial-items/burial-flags/)

</div>
</div>
<div class="do-dont__dont">
<h3 class="do-dont__heading">Not this</h3>
<div class="do-dont__content" markdown="1">
  
__Avoid "click here" and generic CTA text__

[Click here](https://va.gov/disability/how-to-file-claim/) to file for a VA disability compensation increase if your disability gets worse.

Apply for a United States burial flag to place over a casket or coffin, or place with an urn. 
[Learn more](https://www.va.gov/burials-memorials/memorial-items/burial-flags/)
  
</div>
</div>
</div>

## Formatting

* Don't punctuate link text. Exception: Question marks and colons are OK if they're part of the link copy.
* Create space between different links. Clustering links together can make it hard for users to select the intended link, especially on a touch screen device, like a smartphone.
* In general, put a link on a separate line to help it stand out. Exception: Putting a link at the end of a sentence is OK if space is limited, like intro copy or alerts.

{% capture example_like_this_1 %}
__Put links on their own line__
<ul>
  <li>Trouble breathing</li>
  <li>Persistent (continuing) pain or pressure in the chest</li>
  <li>Bluish lips or face</li>
</ul>
<a href="https://www.cdc.gov/coronavirus/2019-ncov/symptoms-testing/symptoms.html">Check COVID-19 symptoms on the CDC website</a>
{% endcapture %}

{% capture example_not_this_1 %}
__Avoid linking each item in a list to the same destination__
<ul>
  <li><a href="https://www.cdc.gov/coronavirus/2019-ncov/symptoms-testing/symptoms.html">Trouble breathing</a></li>
  <li><a href="https://www.cdc.gov/coronavirus/2019-ncov/symptoms-testing/symptoms.html">Persistent (continuing) pain or pressure in the chest</a></li>
  <li><a href="https://www.cdc.gov/coronavirus/2019-ncov/symptoms-testing/symptoms.html">Bluish lips or face</a></li>
</ul>
{% endcapture %}
{% include _like-this-not-this.html like_this=example_like_this_1 not_this=example_not_this_1 %}

### Use CTA links to call out actions

CTA links are standalone hyperlinks that are calls to an action, but that don't warrant a [primary button CTA]({{ site.baseurl }}/content-style-guide/button-labels). 

We generally reserve button CTAs to launch an application, to sign in, or other primary, essential actions on a page. But there are other kinds of actions that may call for a CTA as a text link, like downloading a form or learning about important information (like eligibility or copay rates, etc.). 

<div class="do-dont">
<div class="do-dont__do">
<h3 class="do-dont__heading">Like this</h3>
<div class="do-dont__content" markdown="1">
  
__In this example, the link is an action related to the topic, but it isn't the primary CTA, which is to use the online application.__

You can apply online or mail your Application for Burial Benefits (VA Form 21P-530).

<a 
  href="#VBA-21P-530-ARE.pdf"
  download="VBA-21P-530-ARE.pdf" 
  type="application/pdf">
    <i aria-hidden="true" class="fas fa-download vads-u-padding-right--1" role="img"></i>
      Download VA Form 21P-530 <dfn>(<abbr title="Portable Document Format">PDF</abbr>, 5 pages)</dfn>
</a>
  
</div>
</div>
<div class="do-dont__dont">
<h3 class="do-dont__heading">Not this</h3>
<div class="do-dont__content" markdown="1">
  
__In this example, the action gets lost as an embedded text link.__
  
You can apply online or mail your [Application for Burial Benefits (VA Form 21P-530)](https://www.vba.va.gov/pubs/forms/VBA-21P-530-ARE.pdf).

</div>
</div>
</div>

## Linking to documents and other file sources
* Avoid linking to PDFs as much as possible. 
* If a link opens a calendar, YouTube video, XLS, or other file format, add the relevant icon from the Components section in the Design System. [Review examples of link variations in the Components section]({{ site.baseurl }}/components/links/)

## Linking to external sites

* **Use text that tells the reader where the link takes them.** Example: [Check COVID-19 symptoms on the CDC website](https://www.cdc.gov/coronavirus/2019-ncov/symptoms-testing/symptoms.html)
* **Open external links in a new tab or window.** Links to external sites should have an attribute in the source code to open in a new tab. (This is what that looks like: `target="_blank"` .) External links should also have `rel="noreferrer"` as an attribute.
* **Consider using an aria-label to create a screen reader-only label.** Aria-labels can be helpful in specialized instances where there's a clear reason to use separate text for people who use screen readers. The aria-label may append or replace text within a link to provide context about where the link goes.
* **Don’t use the “new window” icon for external links since it can cause confusion.** In content we avoid use of the "new window" icon. Within components, for brevity, use of the icon is acceptable.
* **Open internal links in the same tab or window.** Links within the VA.gov domain should open in the current tab or window. Exception: Some VA sub-domains provide a distinct experience from VA.gov, so they open in a new tab. For these exceptions, add “(opens in new tab)” to the link text.

### VA sub-domain exceptions that open in a new tab or window

These sub-domains currently open in a new tab, and we should clarify that in the link text. Example: “Learn more on our ebenefits website (opens in new tab)” This list is periodically re-evaluated and updated. 

  * [myhealth.va.gov](http://myhealth.va.gov/)
  * [ebenefits.va.gov](http://ebenefits.va.gov/)
  * [www.accesstocare.va.gov](http://www.accesstocare.va.gov/)
  * [www.gibill.va.gov/wave](http://www.gibill.va.gov/wave)
  * [www.blogs.va.gov](http://www.blogs.va.gov/)
  * [www.data.va.gov](http://www.data.va.gov/)
  * [mobile.va.gov](http://mobile.va.gov/)
  * [www.accesstocare.va.gov](http://www.accesstocare.va.gov/)
  * [www.oit.va.gov](http://www.oit.va.gov/)
