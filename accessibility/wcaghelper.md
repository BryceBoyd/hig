---
layout: reference
title: wcag helper
requireCss: /static/less/cnqr-view/docs.less
---

To turn on the WCAG Helper:

* Go to your environment **<a href="/demo.asp" target="_blank">config page</a>**
* Go to "Accessibility options"
* Set "Enable 508 / WCAG Detection CSS File" to "True"
* Submit

The WCAG Helper will flag the following errors:

* <a href="#error1">ERROR: iframe has no <code>title</code></a>
* <a href="#error2">ERROR: Replace server-side image map</a>
* <a href="#error3">ERROR: Img with no <code>alt</code> tag</a>
* <a href="#error4">ERROR: Provide <code>alt</code> attribute for all areas of an image map</a>
* ERROR: Item has image <code>role</code> without an alternative
* ERROR: image has no source
* <a href="#error7">ERROR: javascript only links must have <code>role=button</code></a>
* ERROR: fieldsets must have legends
* <a href="#error9">ERROR: Image input requires <code>alt</code> attribute</a>
* ERROR: dir attribute has invalid value
* ERROR: <code>title</code> element is empty
* ERROR: HTML element requires <code>lang</code> attribute
* ERROR: replace empty TH element with TD</a>
* ERROR: nested table found. Likely missing <code>role="presentation"</code>
* ERROR: only one TR in this table. Likely missing <code>role="presentation"</code>
* ERROR: List markup invalid
* ERROR: Definition list markup invalid
* ERROR: Definition must follow term

### ERROR: iframe has no <code>title</code> ###
The iframe <code>title</code> attribute provides a label so users can determine which frame to enter and explore in detail. It does not label the individual page (frame) or inline frame (iframe) in the frameset.</p><p>Note that the <code>title</code> attribute labels frames, and is different from the <code>title</code> element which labels documents. Both should be provided, since the first facilitates navigation among frames and the second clarifies the user's current location.

The <code>title</code> attribute is not interchangeable with the <code>name</code> attribute. The <code>title</code> labels the frame for users; the <code>name</code> labels it for scripting and window targeting. The <code>name</code> is not presented to the user, only the <code>title</code> is.

| A flagged Iframe with no <code>title</code> | Iframe with <code>title</code> |
| --------------------------------------------|--------------------------------|
|<iframe src="/UI/docs/Accessibility/WCAGHelperIframeExample" id="notitleiframe"></iframe> | <iframe src="/UI/docs/Accessibility/WCAGHelperIframeExample" id="titleiframe" title="Iframe with Title"></iframe> |

### ERROR: Replace server-side image map ####
These are sometimes still seen, if rarely. Travel codebase doesn't have any element with <code>ismap</code> attribute, but I'm not sure about Travel Manager.

### ERROR: Img with no <code>alt</code> tag ###
Every image must have an <code>alt</code> attribute. This is a requirement of HTML standard. Images without an <code>alt</code> attribute are likely inaccessible.

If an image is used strictly for decoration purposes, then the <code>alt</code> value must be empty.

**Note:** Having a "null" <code>alt</code> attribute is not the same as having no <code>alt</code> attribute.

| A flagged Image with no <code>alt</code> | Image with <code>alt</code> |
| -----------------------------------------| ----------------------------|
| <img src="/images/themes/bluefrog/banner_new.jpg" id="bannerImageNoAlt"/> | <img src="/images/themes/bluefrog/banner_new.jpg" id="bannerImageWithAlt" alt="Concur"/> |

### ERROR: Provide <code>alt</code> attribute for all areas of an image map ###
To ensure the accessibility of client side image maps, engineers should ensure that <code>alt</code> attributes are defined for each active <code>area</code> defined within a <code>map</code> element. The <code>alt</code> attribute should provide a concise description of the content to be found or function to be performed at the target destination of the <code>area</code> element.

### ERROR: javascript only links must have <code>role=button</code> ###

From <a href="/UI/docs/Accessibility/BestPractices/#bp3" target="_blank">/UI/docs/Accessibility/BestPractices</a>,
<q cite="/UI/docs/Accessibility/BestPractices/#bp3">Anchor tags are native links, but they can act as either a link or a button. When an anchor tag is used as a button, it is imperative to add role="button" as an attribute so it can be recognized as a button by screen readers.</q>

### ERROR: Image input requires <code>alt</code> attribute ###
For input elements of type 'image', the <code>alt</code> attribute of the <code>input</code> element is used to provide a functional label. This label indicates the button's function, but does not attempt to describe the image. The label is especially important if there are multiple submit buttons on the page that each lead to different results.

The <code>input</code> element is used to create many kinds of form controls. Although the HTML and XHTML DTDs permits the <code>alt</code> attribute on all of these, it should be used only on image submit buttons. User agent support for this attribute on other types of form controls is not well defined, and other mechanisms are used to label these controls.


| <code>input</code>  without an <code>alt</code> attribute | <code>input</code>  with an <code>alt</code> attribute |
| --------------------------------------------------------- | ------------------------------------------------------ |
| <input type="image" name="submit" src="/Images/ButtonMailDown.gif" /> | <input type="image" name="submit" src="/Images/ButtonMailDown.gif" alt="Search for hotels" /> |
