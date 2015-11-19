---
layout: reference
title: faq
requireCss: /static/less/cnqr-view/docs.less
---

<ul>
  <li>
    <p>
      <ac:link ac:anchor="Q1">
        <ac:plain-text-link-body><![CDATA[What is this "Styleguide" thing?]]></ac:plain-text-link-body>
      </ac:link>
    </p>
  </li>
  <li>
    <p>
      <ac:link ac:anchor="Q2">
        <ac:plain-text-link-body><![CDATA[Do I have to follow the styleguide?]]></ac:plain-text-link-body>
      </ac:link>
    </p>
  </li>
  <li>
    <p>
      <ac:link ac:anchor="Q3">
        <ac:plain-text-link-body><![CDATA[What colors can I use for typography?]]></ac:plain-text-link-body>
      </ac:link>
    </p>
  </li>
  <li>
    <p>
      <ac:link ac:anchor="Q4">
        <ac:plain-text-link-body><![CDATA[How much vertical space should I use between two widgets?]]></ac:plain-text-link-body>
      </ac:link>
    </p>
  </li>
  <li>
    <p>
      <ac:link ac:anchor="Q5">
        <ac:plain-text-link-body><![CDATA[When should I use the orange buttons?]]></ac:plain-text-link-body>
      </ac:link>
    </p>
  </li>
  <li>
    <p>
      <ac:link ac:anchor="Q6">
        <ac:plain-text-link-body><![CDATA[How did we choose the colors in our palette?]]></ac:plain-text-link-body>
      </ac:link>
    </p>
  </li>
  <li>
    <p>
      <ac:link ac:anchor="Q7">
        <ac:plain-text-link-body><![CDATA[What if my question isn’t answered in the styleguide?]]></ac:plain-text-link-body>
      </ac:link>
    </p>
  </li>
  <li>
    <p>
      <ac:link ac:anchor="Q8">
        <ac:plain-text-link-body><![CDATA[What if my design requires something new?]]></ac:plain-text-link-body>
      </ac:link>
    </p>
  </li>
</ul>
<p> </p>
<hr/>
<p> </p>
<p>
  <ac:macro ac:name="anchor">
    <ac:default-parameter>Q1</ac:default-parameter>
  </ac:macro>
</p>
<ac:macro ac:name="panel">
  <ac:parameter ac:name="bgColor">#ffffff</ac:parameter>
  <ac:parameter ac:name="titleBGColor">#dddddd</ac:parameter>
  <ac:parameter ac:name="title">What is this "Styleguide" thing?</ac:parameter>
  <ac:parameter ac:name="borderStyle">solid</ac:parameter>
  <ac:parameter ac:name="borderColor">#cccccc</ac:parameter>
  <ac:parameter ac:name="borderWidth">1px</ac:parameter>
  <ac:parameter ac:name="titleColor">#000000</ac:parameter>
  <ac:rich-text-body>
    <p>
      <span style="color: rgb(0,0,0);">The styleguide is our roadmap for consistency. Whether designing a large new feature, or a small update to an existing feature, using the styleguide will ensure that what we design feels like it all came from the same place and time.</span>
    </p>
  </ac:rich-text-body>
</ac:macro>
<p> </p>
<p>
  <ac:macro ac:name="anchor">
    <ac:default-parameter>Q2</ac:default-parameter>
  </ac:macro>
</p>
<ac:macro ac:name="panel">
  <ac:parameter ac:name="bgColor">#ffffff</ac:parameter>
  <ac:parameter ac:name="titleBGColor">#dddddd</ac:parameter>
  <ac:parameter ac:name="title">Do I have to follow the styleguide?</ac:parameter>
  <ac:parameter ac:name="borderStyle">solid</ac:parameter>
  <ac:parameter ac:name="borderColor">#cccccc</ac:parameter>
  <ac:parameter ac:name="borderWidth">1px</ac:parameter>
  <ac:parameter ac:name="titleColor">#000000</ac:parameter>
  <ac:rich-text-body>
    <p>
      <span style="color: rgb(0,0,0);">
        <strong>Short answer</strong>: Yes.</span>
      <span> </span>
    </p>
    <p>
      <span style="color: rgb(0,0,0);">
        <strong>Long answer</strong>: Still yes. BUT, there is still some wiggle room to design great features and be innovative. The styleguide gives you a framework for the majority of UI elements, allowing you to focus on the really important issues.</span>
    </p>
  </ac:rich-text-body>
</ac:macro>
<p> </p>
<p>
  <ac:macro ac:name="anchor">
    <ac:default-parameter>Q3</ac:default-parameter>
  </ac:macro>
</p>
<ac:macro ac:name="panel">
  <ac:parameter ac:name="bgColor">#ffffff</ac:parameter>
  <ac:parameter ac:name="titleBGColor">#dddddd</ac:parameter>
  <ac:parameter ac:name="title">What colors can I use for typography?</ac:parameter>
  <ac:parameter ac:name="borderStyle">solid</ac:parameter>
  <ac:parameter ac:name="borderColor">#cccccc</ac:parameter>
  <ac:parameter ac:name="borderWidth">1px</ac:parameter>
  <ac:parameter ac:name="titleColor">#000000</ac:parameter>
  <ac:rich-text-body>
    <h2>
      <span style="color: rgb(0,0,0);">What colors can I use for typography?</span>
    </h2>
    <p>
      <span style="color: rgb(0,0,0);">Easy question! #333333 for general text, and #2379BF for text links.</span>
    </p>
    <p>
      <span style="color: rgb(0,0,0);">
        <strong>More in depth answer:</strong> #333333 is the default text color, but if you need to reference for development, just note the @text-color less variable in your visual spec. For text links, reference @brand-secondary-highlight. </span>
      <span style="line-height: 1.4285715;"> </span>
      <span style="color: rgb(0,0,0);">It is possible, however, to use other grey colors for less prominent text. Simply choose a grey value with a color contrast with a ratio of 4.5:1 for small text, and 3:1 for large text (16px or greater) over our @grey-lightest color (or white, if applicable). </span>
      <span style="line-height: 1.4285715;"> </span>
      <span style="color: rgb(0,0,0);"> </span>
    </p>
    <p>
      <span style="color: rgb(0,0,0);">See <a href="http://webaim.org/resources/contrastchecker/">http://webaim.org/resources/contrastchecker/</a> </span>
    </p>
  </ac:rich-text-body>
</ac:macro>
<p> </p>
<p>
  <ac:macro ac:name="anchor">
    <ac:default-parameter>Q4</ac:default-parameter>
  </ac:macro>
</p>
<ac:macro ac:name="panel">
  <ac:parameter ac:name="bgColor">#ffffff</ac:parameter>
  <ac:parameter ac:name="titleBGColor">#dddddd</ac:parameter>
  <ac:parameter ac:name="title">How much vertical space should their be between two widgets?</ac:parameter>
  <ac:parameter ac:name="borderStyle">solid</ac:parameter>
  <ac:parameter ac:name="borderColor">#cccccc</ac:parameter>
  <ac:parameter ac:name="borderWidth">1px</ac:parameter>
  <ac:parameter ac:name="titleColor">#000000</ac:parameter>
  <ac:rich-text-body>
    <p>
      <span style="color: rgb(0,0,0);">We usually use a margin of 4, 8, 16, 32, or 64, depending on what makes sense. </span>
    </p>
    <p>
      <strong>
        <span style="color: rgb(0,0,0);">Example:</span> </strong>
    </p>
    <ul>
      <li>
        <span style="color: rgb(0,0,0);">32px between primary page headings and the next content (h1 and whatever comes after it)</span>
      </li>
      <li>
        <span style="color: rgb(0,0,0);">4px between a label and text field</span>
      </li>
    </ul>
    <p>
      <span style="color: rgb(0,0,0);"> </span>
    </p>
    <p>
      <span style="color: rgb(0,0,0);">This should help get you started, but the downloadable layered .psd files have the margins in-place. </span>
    </p>
  </ac:rich-text-body>
</ac:macro>
<p> </p>
<p>
  <ac:macro ac:name="anchor">
    <ac:default-parameter>Q5</ac:default-parameter>
  </ac:macro>
</p>
<ac:macro ac:name="panel">
  <ac:parameter ac:name="bgColor">#ffffff</ac:parameter>
  <ac:parameter ac:name="titleBGColor">#dddddd</ac:parameter>
  <ac:parameter ac:name="title">When should I use the orange button?</ac:parameter>
  <ac:parameter ac:name="borderStyle">solid</ac:parameter>
  <ac:parameter ac:name="borderColor">#cccccc</ac:parameter>
  <ac:parameter ac:name="borderWidth">1px</ac:parameter>
  <ac:parameter ac:name="titleColor">#000000</ac:parameter>
  <ac:rich-text-body>
    <p>
      <span style="color: rgb(0,0,0);">The orange button should be reserved for only the most important actions. There should only be one on a page at a time (search results are an exception. See the buttons section). Some pages won't even have an orange button, because they'll just be composed of in-page interaction buttons. </span>
    </p>
  </ac:rich-text-body>
</ac:macro>
<p> </p>
<p>
  <ac:macro ac:name="anchor">
    <ac:default-parameter>Q6</ac:default-parameter>
  </ac:macro>
</p>
<ac:macro ac:name="panel">
  <ac:parameter ac:name="bgColor">#ffffff</ac:parameter>
  <ac:parameter ac:name="titleBGColor">#dddddd</ac:parameter>
  <ac:parameter ac:name="title">How did we choose the colors in our palette?</ac:parameter>
  <ac:parameter ac:name="borderStyle">solid</ac:parameter>
  <ac:parameter ac:name="borderColor">#cccccc</ac:parameter>
  <ac:parameter ac:name="borderWidth">1px</ac:parameter>
  <ac:parameter ac:name="titleColor">#000000</ac:parameter>
  <ac:rich-text-body>
    <p>
      <span style="color: rgb(0,0,0);">That's another great question. The current color palette started with</span>
      <span style="color: rgb(0,0,0);"> a stable/trustworthy color built off our Concur brand logo color. We added</span>
      <span style="color: rgb(0,0,0);"> a vibrant/active color for the most important actions, and a wide selection of greys that give us a ton of flexibility. Then we made them all 508 compliant. The color palette we have looks great and is accessible out of the box without any special considerations. Win.</span>
    </p>
  </ac:rich-text-body>
</ac:macro>
<p> </p>
<p>
  <ac:macro ac:name="anchor">
    <ac:default-parameter>Q7</ac:default-parameter>
  </ac:macro>
</p>
<ac:macro ac:name="panel">
  <ac:parameter ac:name="bgColor">#ffffff</ac:parameter>
  <ac:parameter ac:name="titleBGColor">#dddddd</ac:parameter>
  <ac:parameter ac:name="title">What if my question isn't in the styleguide?</ac:parameter>
  <ac:parameter ac:name="borderStyle">solid</ac:parameter>
  <ac:parameter ac:name="borderColor">#cccccc</ac:parameter>
  <ac:parameter ac:name="borderWidth">1px</ac:parameter>
  <ac:parameter ac:name="titleColor">#000000</ac:parameter>
  <ac:rich-text-body>
    <p>
      <span style="color: rgb(0,0,0);">Chances are, it is. However, if you can't find an answer, feel free to ask! Just contact </span>
      <a href="mailto:bryceb@concur.com">bryceb@concur.com</a>
      <span style="color: rgb(0,0,0);"> with your question. </span>
    </p>
  </ac:rich-text-body>
</ac:macro>
<p> </p>
<p>
  <ac:macro ac:name="anchor">
    <ac:default-parameter>Q8</ac:default-parameter>
  </ac:macro>
</p>
<ac:macro ac:name="panel">
  <ac:parameter ac:name="bgColor">#ffffff</ac:parameter>
  <ac:parameter ac:name="titleBGColor">#dddddd</ac:parameter>
  <ac:parameter ac:name="title">What if my design requires something new?</ac:parameter>
  <ac:parameter ac:name="borderStyle">solid</ac:parameter>
  <ac:parameter ac:name="borderColor">#cccccc</ac:parameter>
  <ac:parameter ac:name="borderWidth">1px</ac:parameter>
  <ac:parameter ac:name="titleColor">#000000</ac:parameter>
  <ac:rich-text-body>
    <p>
      <span style="color: rgb(0,0,0);">We're working on a process for identifying and vetting new styles. Watch this space for a great answer in the March time-frame. </span>
    </p>
    <div>
      <span style="color: rgb(0,0,0);">
        <br/>
      </span>
    </div>
  </ac:rich-text-body>
</ac:macro>
