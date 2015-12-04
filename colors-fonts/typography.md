---
layout: reference
title: typography
---

## Gateway Style Typography ##

### Text ###
<table class="reporttable reporttable-airy">
	<tr>
		<th>Name</th>
		<th>Description</th>
		<th>Example</th>
	</tr>
	<tr>
		<td>body text, &lt;p&gt;&lt;/p&gt;&lt;div&gt;&lt;/div&gt;, etc...</td>
		<td>Baseline style for page text</td>
		<td class="cnqr-force-no-wrap" style="font-size:13px">Normal Body Text</td>
	</tr>
	<tr>
		<td>.small,  &lt;small&gt;&lt;/small&gt;</td>
		<td>reduced size text. style may change depending on context (see H1-H6)</td>
		<td class="cnqr-force-no-wrap" style="font-size:13px"><span class="small">small text</span></td>
	</tr>
	<tr>
		<td>.lead</td>
		<td>increased size text, but NOT a header</td>
		<td class="cnqr-force-no-wrap" style="font-size:13px"><span class="lead">large text</span></td>
	</tr>
	<tr>
		<td>&lt;strong&gt;&lt;/strong&gt;</td>
		<td>bolded text</td>
		<td class="cnqr-force-no-wrap" style="font-size:13px"><strong>bolded text</strong></td>
	</tr>
	<tr>
		<td>&lt;em&gt;&lt;/em&gt;</td>
		<td>emphisized text</td>
		<td class="cnqr-force-no-wrap" style="font-size:13px"><em>italicized text</em></td>
	</tr>
</table>

### Headings ###
#### Modifier Classes ####

* **cnqr-first** Removes the top margin

<table class="reporttable reporttable-airy">
	<tr>
		<th>Level</th>
		<th>Usage</th>
		<th>properties</th>
		<th>Font Family</th>
		<th>Example</th>
	</tr>
	<tr>
		<td>H1</td>
		<td>All page titles<br />no more than ONE per page</td>
		<td class="cnqr-force-no-wrap">@@font-size-h1</td>
		<td class="cnqr-force-no-wrap">@@font-family-headings-1</td>
		<td class="cnqr-force-no-wrap"><h1>Now is the time...</h1></td>
	</tr>
	<tr>
		<td>H2</td>
		<td>Secondary titling</td>
		<td>@@font-size-h2</td>
		<td>@@headings-font-family</td>
		<td><h2>Now is the time...</h2></td>
	</tr>
	<tr>
		<td>H3</td>
		<td>Workhorse Title</td>
		<td>@@font-size-h3</td>
		<td>@@headings-font-family</td>
		<td><h3>Now is the time...</h3></td>
	</tr>
	<tr>
		<td>H4</td>
		<td>Usage</td>
		<td>@@font-size-h4</td>
		<td>@@headings-font-family</td>
		<td><h4>Now is the time...</h4></td>
	</tr>
	<tr>
		<td>H5</td>
		<td>(not used)</td>
		<td>@@font-size-h5</td>
		<td>@@headings-font-family</td>
		<td><h5>Now is the time...</h5></td>
	</tr>
	<tr>
		<td>H6</td>
		<td></td>
		<td>@@font-size-h6</td>
		<td>@@headings-font-family</td>
		<td><h6>Now is the time...</h6></td>
	</tr>
</table>

### Font Familiy Lists ###
<table class="reporttable reporttable-airy">
	<tr>
		<th>Name</th>
		<th>Composition</th>
		<th>Example</th>
	</tr>
	<tr>
		<td>@@font-family-base:</td>
		<td>'Helvetica Neue', Helvetica, 'Segoe UI', Arial, sans-serif</td>
		<td class="cnqr-force-no-wrap" style="font-family:'Helvetica Neue',Helvetica,'Segoe UI',Arial,sans-serif">Now is the time...</td>
	</tr>
	<tr>
		<td>@@headings-font-family</td>
		<td>'Helvetica Neue', Helvetica, 'Segoe UI Semibold', sans-serif</td>
		<td class="cnqr-force-no-wrap" style="font-family:'Helvetica Neue',Helvetica, 'Segoe UI Semibold', sans-serif;">Now is the time...</td>
	</tr>
	<tr>
		<td>@@font-family-headings-1:</td>
		<td>'OpenSans-Light',sans-serif"</td>
		<td class="cnqr-force-no-wrap" style="font-family:'OpenSans-Light',sans-serif">Now is the time...</td>
	</tr>
	<tr>
		<td>@@font-display-family:</td>
		<td>'Oswald-Regular',sans-serif</td>
		<td class="cnqr-force-no-wrap" style="font-family:'Oswald-Regular',sans-serif">0123456789</td>
	</tr>
</table>
