---
layout: reference
title: faq
---


<div class="row show-grid">
	<div class="col-md-4">
		<ul>
			<li><a href="#faq1">What is Accessiblity?</a></li>
			<li><a href="#faq2">What is 508 compliance?</a></li>
			<li><a href="#faq3">Is 508 compliance the same as accessibility?</a></li>
			<li><a href="#faq4">What is a screen reader?</a></li>
			<li><a href="#faq5">What is a screen magnifier?</a></li>
			<li><a href="#faq6">Does Accessibly mean my design isn't as pretty?</a></li>
		</ul>
	</div>
	<div class="col-md-4">
		<ul>
			<li><a href="#faq7">What Tools can I use to evaluate accessibility?</a></li>
			<li><a href="#faq8">What are the most useful manual checks?</a></li>
			<li><a href="#faq9">Which browsers should I design for?</a></li>
			<li><a href="#faq10">What does “keyboard accessible” mean?</a></li>
			<li><a href="#faq11">Why are we focusing on the close button when the dialog opens up?</a></li>
			<li><a href="#faq12">Why is the Ok button is not getting read when the dialog opens up?</a></li>
		</ul>
	</div>
	<div class="col-md-4">
		<ul>
			<li><a href="#faq13">What is a text equivalent? How do I add it to an image?</a></li>
			<li><a href="#faq14">Is the text equivalent always a description of the image?</a></li>
			<li><a href="#faq15">Do I really need the ALT attribute for every single image?</a></li>
			<li><a href="#faq16">How can I tell if contrast is sufficient?</a></li>
			<li><a href="#faq17">What is a keyboard trap?</a></li>
			<li><a href="#faq18">What does logical tab order mean?</a></li>
		</ul>
	</div>
</div>

<h4 id="faq1">What is Accessiblity?</h4>
<p>Web accessibility refers to a standard of inclusive website development based on the idea that information should be equally available to all people, regardless of physical or developmental abilities or impairments. </p>

<h4 id="faq2">What is 508 compliance?</h4>
<p><a href="http://www.section508.gov/index.cfm?FuseAction=Content&amp;ID=11#web" target="_blank">Section 508 of the U.S. Code</a> is the law that requires federal agencies and their contractors to adhere to a minimal level of accessibility. The law can be loosely interpreted and basically boils down to:</p>
<blockquote>
	<p>"the use of text labels or descriptors for graphics and certain format elements. (HTML code already provides an "Alt Text" tag for graphics which can serve as a verbal descriptor for graphics). This section also addresses the usability of multimedia presentations, image maps, style sheets, scripting languages, applets and plug-ins, and electronic forms."</p>
</blockquote>

<h4 id="faq3">Is 508 compliance the same as accessibility?</h4>
<p>No. 508 compliance is the law that law-people wrote up to try and begin to set some standards. It provides the minimum standards for what is deemed acceptable, and minimum really does not make a site fully accessible. Sure, you can make the effort to be 508 compliant, but the wording is very vague. Make the effort to be accessible, not just 508 compliant.</p>

<h4 id="faq4">What is a screen reader?</h4>
<p>People who can not see the screen, or have difficulty reading, but can hear, are able to use computers with this kind of assistive technology that produces speech (or Braille, which is read with the fingertips). Screen magnification devices (see below) also often incorporate a screen reader. Screen readers typically have numerous options, so that the user experience of a given web page will be different for each person.</p>
  <p>Some of the most widely used screen readers available at the date are:</p>
  <ul>
      <li>Windows: JAWS, Window Eyes, NVDA, Dragon</li>
      <li>Mac: Voiceover</li>
      <li>Linux: GNome-Orca</li>
      <li>Mobile: Talks (Symbian); Mobile Speak Pocket (Windows mobile); Voiceover (iPhone 3GS); Orator (Blackberry RIM)</li>
  </ul>

<h4 id="faq5">What is a screen magnifier?</h4>
<p>People who have difficulty seeing the screen can use a magnifier. It is like reading a paper document with a magnifying glass. They can use the keyboard or mouse to move the magnifier around the screen. As with a traditional magnifying glass, the person can only see a limited area of the screen at any time. As people who need screen magnification often also have difficulty with colour contrast, these systems normally also allow the user to change the colours (for example, inverting the colours or enhancing contrast).</p>
  <p>Some of the most popular screen magnifiers are:</p>
  <ul>
      <li>Magnification: ZoomText and Magic</li>
  </ul>

<h4 id="faq6">Does Accessibly mean my design isn't as pretty?</h4>
<p>This is a serious misconception. There isn't anything about being accessible that necessarily makes a design look ugly. Anything that you can do with web standards and other best practices can be done accessibly, and that makes for a lot of great design potential.</p>

<h4 id="faq7">What Tools can I use to evaluate accessibility?</h4>
<p>There is wide range of tools available including browsers, crawlers to run manual checks on entire sites, tools to annotate pages with icons, and tools for checking specific aspects. Tools may come in different languages, and for different platforms. Different tools can check against different guidelines and may allow the user to create custom checks.</p>
<p>We have compiled a good list that can be found <a href="/UI/docs/Accessibility/Tools" target="_blank">here</a>. That been said, <a href="https://addons.mozilla.org/en-us/firefox/addon/openajax-accessibility-exte/" target="_blank">OpenAjax Alliance (OAA) Accessibility Evalutation</a> is the tool of choice as it evaluates web pages for compliance to WCAG 2.0 Success criteria and allows web devleopers to explore and inspect the accessibility of the web resources they are developing.</p>


<h4 id="faq8">What are the most useful manual checks?</h4>
<ul>
      <li>General: try navigating with a screen reader and different browsers.</li>
      <li>Images and non-text content: alt text, images of text.</li>
      <li>Document structure: headings, lists and tables.</li>
      <li>Layout and presentation: contrast, text size, stylesheets turned off, movement.</li>
      <li>Behaviour and scripting: keyboard access.</li>
      <li>Metadata and understanding: page titles, link text.</li>
      <li>Forms: labels, error messages.</li>
  </ul>

<h4 id="faq9">Which browsers should I design for?</h4>
<p>Design for Web standards, such as HTML, CSS and DOM. Modern browsers conform to these standards and so designing for the standard will help ensure an optimum experience on all browsers. It is a mistake to design for a specific browser.</p>
  <p>For testing, the priority should go to IE8 as it is the standard Browser used by the US Government.</p>

<h4 id="faq10">What does “keyboard accessible” mean?</h4>
<p>In practice, this means ensuring that content can be operated using any input device. Normally input devices are the keyboard and the mouse, or devices that emulate them.</p>
  <p>Some users navigate through links and other interactive elements of a page using the tab or some other key. But scripting can alter this behaviour, and if it is not done carefully, can prevent the user interacting with the content.</p>

<h4 id="faq11">Why are we focusing on the close button when the dialog opens up?</h4>
<p>Per WCAG 2.0 standards:</p>
<blockquote><p>“When a modal dialog opens focus goes to the first focusable item in the dialog. Determining the first focusable item must take into account elements which receive focus by default (form fields and links) as well as items which may have a tabindex attribute with a positive value. If there is no focusable item in the dialog, focus is placed on the dialog container element.”</p></blockquote>
<p>We are focusing on the close button when the messagebox opens up, because it just happens it is the first focusable element. If there is no close button and the messagebox has a link in its content, the focus will go to that element.</p>

<h4 id="faq12">Why the Ok button is not getting read when the dialog opens up?</h4>
<p>Per WCAG 2.0 standards:</p>
<blockquote><p>“The Alert dialog has an aria-labelledby that references the title of the dialog. If there is not a visible title, use an appropriate aria-label instead.
The element with role alertdialog has an aria-describedby referring to the message element that has role document.”</p></blockquote>
<p>So when the dialog opens up, both the title and the content are getting read. The Ok button is in the footer, that’s why it is not getting read.</p>
<p>But if the user presses Tab, he will get to it as per WCAG 2.0 standards:</p>
<blockquote><p>“Tab Focus must be held within the dialog until it is cancelled or submitted. As the user presses tab to move within items in the dialog, pressing tab with focus on the last focusable item in the dialog will move focus back to the first focusable item in the dialog. 
Shift+Tab Likewise, if the user is shift-tabbing through elements in the dialog, pressing shift-tab with focus on the first focusable item in the dialog will move focus to the last item in the dialog. “</p></blockquote>

<p>Here is an example of how JAWS reads the Log out dialog:</p>

<ul>
	<li>The dialog is labeled by the title which is in this case “Confirm”.</li>
	<li>The dialog is described by the content which is in this case “Are you sure you want to log out”.</li>
	<li>The first focusable element is the “Close” button.</li>
</ul>

<p>So Jaws is going to read:  </p>
<ul>
	<li>FF reads: “aria-labelledby” + “role” + “aria-describedby” + “focused element”</li>
	<li>IE8 reads: “aria-labelledby” + “role” + “focused element” + “aria-describedby”</li>
</ul>
<p>Result: “confirm” + “dialog” + “Are you sure you want to log out” + “Close button”.</p>
<p>The Concur messagebox are following WCAG 2.0 standards to the letter.</p> 
<p>Of course there are bugs as screen-reader technology and aria attributes are fairly new and we do our best to bypass these bugs and bend current technology to make our content not only 508 compliant but as accessible as possible.</p>


<h4 id="faq13">What is a text equivalent? How do I add it to an image?</h4>
<p>A text equivalent is a text that describes anything that is not itself text, such as pictures, video, sound, form controls, scripts, and colours. This is important because a browser or assistive technology can transform text to suit the user&rsquo;s needs, as speech, as text in different font styles, sizes, and colours, or in other languages. It is especially important for people who can&rsquo;t see images, either because they have a sight disability or because they haven&rsquo;t downloaded them. In HTML the text equivalent is provided with the <code>alt</code> attribute. Other technologies can use different methods to provide the alternatives, such as accessibility panels or properties.</p>

<h4 id="faq14">Is the text equivalent always a description of the image?</h4>
<p>The text equivalent should convey the same information and functionality as the element itself. If an image is scripted to work as a button, then tell the user what it does. With some images, the designer has to decide whether it is relevant or not. Too much information can be as bad as too little.</p>

<h4 id="faq15">Do I really need the ALT attribute for every single image?</h4>
<p><b>Yes.</b> If the image is a non-essential image, you still need to have the alt attribute, otherwise the screenreader will speak the name of the image. For example, if you had concur.gif, a person listening to your web page would hear "image, concur.gif". The only appropriate alt for a non-essential image is alt="". <b>There is no space between the quotes.</b></p>

<h4 id="faq16">How can I tell if contrast is sufficient?</h4>
<p>WCAG 2.0 gives a minimum contrast ratio (4.5) for text, images and other visual content. <a href="https://addons.mozilla.org/en-US/firefox/addon/wcag-contrast-checker/" target="_blank">Contrast Checker </a> is a good tool to use to check contrast. You can run it in this <a href="http://localhost/UI/docs/Accessibility/Contrast" target="_blank">demo page</a> to check what tests pass and what tests fail.</p>

<h4 id="faq17">What is a keyboard trap?</h4>
<p>Normally a user navigates onto a link and then off again and on to the next with no difficulty. However, a script activated by a link or some other interactive element can prevent the keyboard moving onto the next item, leaving the user trapped. So if you use scripting, always check that you can navigate through the whole page using the keyboard.</p>

<h4 id="faq18">What does logical tab order mean?</h4>
<p>As a user navigates through the page using the tab key, jumping from one link to another, it can be difficult to see the position of the current link (the focus) even if it is highlighted. This &ldquo;tab order&rdquo; usually follows the order of the links in the markup. However, if content is positioned differently using CSS, the focus may jump from top to bottom, or around the screen unpredictably, leaving the user confused. This can also be caused by scripts. If you use scripts or CSS positioning, always try navigating through the page with the keyboard to check this tab order, or use a tool to display it (as a series of numbers on the links).</p>
