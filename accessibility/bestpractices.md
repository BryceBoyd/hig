---
layout: reference
title: best practices
requireCss: /static/less/cnqr-view/docs.less
---

<ul>
	<li><a href="#bp1">Tabbable Vs Non-Tabbable elements</a></li>
	<li><a href="#bp2">Aria-label Vs screen-reader-only Vs screen-reader-only-focusable</a></li>
	<li><a href="#bp3">Anchor tags acting as buttons</a></li>
	<li><a href="#bp4">Supply "alt" tags for images</a></li>
	<li><a href="#bp5">Supply empty "alt" tags for unessential images</a></li>
	<li><a href="#bp6">Create Meaningful Links</a></li>
	<li><a href="#bp7">Allow users to skip over navigational links</a></li>
	<li><a href="#bp8">Use Frames Sparingly if at all, and give them titles</a></li>
	<li><a href="#bp9">Associate Labels with Form Elements</a></li>
	<li><a href="#bp10">Make sure you can navigate through your site using the keyboard only</a></li>
	<li><a href="#bp11">Data Tables - Use Headers</a></li>
	<li><a href="#bp12">Hover( Mouse users ) VS Focus ( Keyboard Users )</a></li>
</ul>

  <h3 id="bp1">Tabbable Vs Non-Tabbable elements</h3>
<ul>
	<li>By default, only links and form fields are tabbable from the keyboard. If a non-focusable element convey information, add tabindex=0 so it can be focused on via the keyboard and falls into the tabbing flow of the document</li>
	<li>On the other hand, tabindex=-1 will remove the element from the tabbing flow of the document </li>
	<li>Adding a positive tabindex should be avoided at all cost. in most cases, positive tabindex values are not necessary, and are only required in cases where the tab order is not ideal, and when the tab order cannot be changed by rearranging the content in HTML. Additionally, the tab order must be manually reconfigured each time a new element is added on the page. </li>
</ul>
<table class="reporttable reporttable-lg">
	<tr>
		<th>Description</th>
		<th>Examples</th>
	</tr>
	<tr>

		<td>
			<p>An anchor tag without an href is not tabbable.</p>
			<p>So if an anchor tag has a text node, but can't be focused on, the user will lose valuable information if he is tabbing using they keyboard.</p>
			<a role="button">Non-Tabbable link</a>
			<p>We can make this anchor tag tabbable by adding tabindex=0 or href="javascript:void()" </p>
			<a role="button" tabindex="0">Tabbable link</a>
		</td>
		<td>
			<h5>HTML</h5>
			<pre class="brush: xml; toolbar: false;">
				<a role="button">
					Non-Tabbable element
				</a>
				<a role="button" tabindex="0">
					Tabbable element
				</a>
			</pre>
		</td>
	</tr>
</table>

  <h3 id="bp2">aria-label Vs screen-reader-only Vs screen-reader-only-focusable</h3>
<ul>
	<li>
		<b>aria-label Vs screen-reader-only:</b> both aria-label attribute and screen-reader-only css class are used to provide an element with a label that is only available to screen readers. However, aria-label is preferred over screen-reader-only css class as it saves us an element ( Please see the example below ).
	</li>
	<li>
		<b>screen-reader-only-focusable:</b> Used to hide elements that need to show only on focus, as it is the case for "Skip" links.
	</li>
</ul>
  <p>Note that our screen reader (sr) classes are similar to Bootstrap screen reader classes (<a href="http://getbootstrap.com/css/#helper-classes-screen-readers">Bootstrap screen-readers helper classes</a>)</p>
<table class="reporttable reporttable-lg">
	<tr>
		<th>Type</th>
		<th>Example</th>
	</tr>

	<tr>
		<td>
			<p><em><small>screen-reader-only</small></em></p>
			<label class="screen-reader-only" for="fake-search">Enter Airport</label>
			<input type="text" id="fake-search"/>
		</td>
		<td>
			<h5>HTML</h5>
			<pre class="brush: xml; toolbar: false;">
				<label class="screen-reader-only" for="fake-search">Enter Airport</label>
				<input type="text" id="fake-search"/>
			</pre>
		</td>
	</tr>
	<tr>
		<td>
			<p><em><small>aria-label</small></em></p>
			<input type="text" aria-label="Enter Hotel"/>
		</td>
		<td>
			<h5>HTML</h5>
			<pre class="brush: xml; toolbar: false;">
				<input type="text" aria-label="Enter Hotel"/>
			</pre>
		</td>
	</tr>
	<tr>
		<td>
			<p><em>Set the cursor in the above input field and tab to focus on this hidden, but focusable link. <small>Similar to Bootstrap's .sr-only.sr-only-focusable class combination.</small></em></p>
			<a class="screen-reader-only-focusable" href="#main-content">Skip Nav</a>
		</td>
		<td>
			<h5>HTML</h5>
			<pre class="brush: xml; toolbar: false;">
				<a class="screen-reader-only-focusable" href="#main-content">Skip Nav</a>
			</pre>
		</td>
	</tr>
	<tr>
		<td>
			<p><em>For fieldsets, we use the screen-reader-only on the parent fieldset (rather than the legend element), due to desire for alternate margins </em></p>
			<fieldset class="screen-reader-only">
				<legend>Legend</legend>
				Content
			</fieldset>
		</td>
		<td>
			<h5>HTML</h5>
			<pre class="brush: xml; toolbar: false;">
				<fieldset class="screen-reader-only">
					<legend>Legend</legend>
					Content
				</fieldset>
			</pre>
		</td>
	</tr>
</table>

  <h3 id="bp3">Anchor tags acting as buttons</h3>
  <ul>
	<li><b>role=button:</b> Anchor tags are native links, but they can act as either a link or a button. When an anchor tag is used as a button, it is imperative to add role="button" as an attribute so it can be recognized as a button by screen readers.  </li>
	<li><b>tabindex=0:</b> Also, most anchor tags who act as buttons won't have an href. They will have an event attached to them. This causes a problem since the element is not Tabbable. Check <a href="#tabbableVsNonTabbable">Tabbable Vs Non-Tabbable elements</a> on how to solve this issue.</li>
	<li><b>aria-label:</b> Some pages might have multiple anchor tags with the same text, as it is the case for the Travel Widget "Search" buttons. This causes confusion while using screen readers as the buttons text don't have enough meaning. aria-label can be used, which overrides the element inner text, to give elements a unique text.</li>
</ul>
<table class="reporttable reporttable-lg">
	<tr>
		<th>Type</th>
		<th>Example</th>

	</tr>
	<tr>
		<td>
			<a aria-label="Search for Flights" id="searchForFlights" name="searchForFlights" class="searchbutton btn btn-primary" role="button" tabindex="0">Search</a>
		</td>
		<td>
			<h5>HTML</h5>
			<pre class="brush: xml; toolbar: false;">
				<a 	aria-label="Search for Flights" 
					role="button" 
					tabindex="0"
				>Search</a>>
			</pre>
		</td>
	</tr>
	<tr>
		<td>
			<a aria-label="Search for Hotels" id="searchForHotels" name="searchForHotels" class="searchbutton btn btn-primary" role="button" tabindex="0">Search</a>
		</td>
		<td>
			<h5>HTML</h5>
			<pre class="brush: xml; toolbar: false;">
				<a 	aria-label="Search for Hotels" 
					role="button" 
					tabindex="0"
				>Search</a>>
			</pre>
		</td>
	</tr>
</table>

<h3 id="bp4">Supply "alt" tags for images</h3>
<table class="reporttable reporttable-lg">
	<tr>
		<th>Type</th>

		<th>Example</th>
	</tr>
	<tr>
		<td>
			<img id="bannerimage" alt="Concur" src="/images/themes/bluefrog/banner_new.jpg">
		</td>
		<td>
			<h5>HTML</h5>
			<pre class="brush: xml; toolbar: false;">
				<img id="bannerimage" 
					 alt="Concur" 
					 src="/banner_new.jpg"
				>
			</pre>
		</td>
	</tr>
</table>

<h3 id="bp5">Supply empty "alt" tags for unessential images</h3>
<table class="reporttable reporttable-lg">
	<tr>

		<th>Type</th>
		<th>Example</th>
	</tr>
	<tr>
		<td>
			<a data-toggle="tooltip" href="javascript:void(0)" role="button" class="cnqr-tooltip cnqr-cursor-help">
				<span class="screen-reader-only">Quick Help - Departure Date</span>
				<img alt="" src="/images/ot_tip.gif" style="vertical-align:middle" data-toggle="tooltip">
			</a>
		</td>
		<td>
			<h5>HTML</h5>
			<pre class="brush: xml; toolbar: false;">
				<a data-toggle="tooltip" href="javascript:void(0)" role="button" class="cnqr-tooltip cnqr-cursor-help">
					<span class="screen-reader-only">Quick Help - Departure Date</span>
					<img alt="" src="/images/ot_tip.gif" style="vertical-align:middle" data-toggle="tooltip">
				</a>
			</pre>
		</td>
	</tr>
</table>

<h3 id="bp6">Create Meaningful Links</h3>
<table class="reporttable reporttable-lg">

	<tr>
		<th>Type</th>
		<th>Example</th>
	</tr>
	<tr>
		<td>
			<p>Bad Example: <a href="http://www.concur.com/">click here</a></p>
		</td>
		<td>
			<h5>HTML</h5>
			<pre class="brush: xml; toolbar: false;">
				<a href="http://www.concur.com/">click here</a>
			</pre>
		</td>
	</tr>

	<tr>
		<td>
			<p>Good Example: <a href="http://www.concur.com/">Concur Technologies</a></p>
		</td>
		<td>
			<h5>HTML</h5>
			<pre class="brush: xml; toolbar: false;">
				<a href="http://www.concur.com/">Concur Technologies</a>
			</pre>
		</td>
	</tr>

	<tr>
		<td>
			<p>Good Example: <a aria-label="Concur Technologies" href="http://www.concur.com/">click here</a></p>
		</td>
		<td>
			<h5>HTML</h5>
			<pre class="brush: xml; toolbar: false;">
				<a aria-label="Concur Technologies" href="http://www.concur.com/">click here</a>					
			</pre>
		</td>
	</tr>
</table>

<h3 id="bp7">Allow users to skip over navigational links</h3>
<table class="reporttable reporttable-lg">
	<tr>
		<th>Type</th>
		<th>Example</th>
	</tr>
	<tr>
		<td>
			<p>Tab here:</p>
			<a href="#cnqr-app-content" class="screen-reader-only-focusable">Skip navigation links</a>
		</td>
		<td>
			<h5>HTML</h5>
			<pre class="brush: xml; toolbar: false;">
				<a href="#cnqr-app-content" class="screen-reader-only-focusable">Skip navigation links</a>
			</pre>
		</td>
	</tr>
</table>

<h3 id="bp8">Use Frames Sparingly if at all, and give them titles</h3>
<table class="reporttable reporttable-lg">
	<tr>
		<th>Type</th>
		<th>Example</th>
	</tr>
	<tr>
		<td>
			<p>Bad Example: Iframe with no <code>title</code></p>
			<iframe src="/UI/docs/Accessibility/WCAGHelperIframeExample" id="notitleiframe"></iframe>
		</td>
		<td>
			<h5>HTML</h5>
			{% highlight html %}
				<iframe src="/UI/docs/Accessibility/WCAGHelperIframeExample" id="notitleiframe"></iframe>
			{% endhighlight  %}
		</td>
	</tr>
	<tr>
		<td>
			<p>Good Example: Iframe with <code>title</code></p>
			<iframe src="/UI/docs/Accessibility/WCAGHelperIframeExample" id="notitleiframe" title="Iframe with Title"></iframe>
		</td>
		<td>
			<h5>HTML</h5>
			{% highlight html %}
				<iframe src="/UI/docs/Accessibility/WCAGHelperIframeExample" id="notitleiframe" title="Iframe with Title"></iframe>
			{% endhighlight %}
		</td>
	</tr>
</table>

<h3 id="bp9">Associate Labels with Form Elements</h3>
<h5>Example</h5>
<div id="WorkAddress" class="cnqr-panel cnqr-panel-default">
   <div class="cnqr-panel-heading">
	  <h2>
		 Work Address
	  </h2>
   </div>
   <div class="cnqr-panel-body">
	  <div class="divrow clearfix">
		 <div style="width:50%;" class="divcell">
			<label for="WorkAddr">Street<span class="screen-reader-only">Work Address</span></label><br>
			<textarea style="width:100%" cols="40" wrap="virtual" id="WorkAddr" name="WorkAddr" rows="2" origval="209 Madison St., Suite 400">209 Madison St., Suite 400</textarea>
		 </div>
	  </div>
	  <div class="divrow clearfix">
		 <div class="divcell">
			<label for="WorkCity">City<span class="screen-reader-only">Work Address</span></label><br>
			<input type="text" autocomplete="off" value="Alexandria" id="WorkCity" style="width:175px" maxlength="30" size="20" name="WorkCity" origval="Alexandria">
		 </div>
		 <div class="divcell">
			<label for="WorkState">State<span class="screen-reader-only">Work Address</span></label><br>
			<input type="text" autocomplete="off" value="VA" id="WorkState" style="width:150px"  maxlength="30" size="13" name="WorkState" origval="VA">
		 </div>
		 <div class="divcell">
			<label for="WorkZip">Postal Code<span class="screen-reader-only">Work Address</span></label><br>
			<input type="text" autocomplete="off" value="22314" style="width:125px" maxlength="20" size="10" id="WorkZip" name="WorkZip" origval="22314">
		 </div>
		 <div class="divcell">
			<label for="WorkCountry">Country<span class="screen-reader-only">Work Address</span></label><br>
			<select name="WorkCountry" id="WorkCountry" origval="US">
			   <option value="US" selected="selected">United States of America</option>
			</select>
		 </div>
	  </div>
   </div>
</div>
<div id="HomeAddress" class="cnqr-panel cnqr-panel-default">
   <div class="cnqr-panel-heading">
	  <h2>Home Address</h2>
   </div>
   <div class="cnqr-panel-body">
	  <div style="width:50%;" class="divcell">
		 <label for="HomeAddr">Street<span class="screen-reader-only">Home Address</span></label>
		 <textarea cols="40" style="width:100%" id="HomeAddr" name="HomeAddr" rows="2" >9017 Vernon View Drive</textarea>
	  </div>
	  <div class="divrow clearfix">
		 <div class="divcell">
			<label for="HomeCity">City<span class="screen-reader-only">Home Address</span></label><br>
			<input type="text" autocomplete="off" value="Alexandria" maxlength="30" size="20" style="width:100%" id="HomeCity" name="HomeCity" origval="Alexandria">
		 </div>
		 <div class="divcell">
			<label for="HomeState">State<span class="screen-reader-only">Home Address</span></label><br>
			<input type="text" autocomplete="off" value="VA" maxlength="30" size="15" style="width:100%" id="HomeState" name="HomeState" origval="VA">
		 </div>
		 <div class="divcell">
			<label for="HomeZip">Postal Code<span class="screen-reader-only">Home Address</span></label><br>
			<input type="text" autocomplete="off" value="22308" maxlength="20" size="10" style="width:100%" id="HomeZip" name="HomeZip" origval="22308">
		 </div>
		 <div class="divcell">
			<label for="HomeCountry">Country<span class="screen-reader-only">Home Address</span></label><br>
			<select  id="HomeCountry" name="HomeCountry">
			   <option value="">&nbsp;</option>
			   <option value="US" selected="selected">United States of America</option>
			</select>
		 </div>
	  </div>
   </div>
</div>

<h5>HTML</h5>
{% highlight html %}
	<div id="WorkAddress" class="cnqr-panel cnqr-panel-default">
	   <div class="cnqr-panel-heading">
		  <h2>
			 Work Address
		  </h2>
	   </div>
	   <div class="cnqr-panel-body">
		  <div class="divrow clearfix">
			 <div class="divcell">
				<label for="WorkAddr">Street<span class="screen-reader-only">Work Address</span></label><br>
				<textarea style="width:100%" cols="40" wrap="virtual" id="WorkAddr" name="WorkAddr" rows="2" origval="209 Madison St., Suite 400">209 Madison St., Suite 400</textarea>
			 </div>
		  </div>
		  <div class="divrow clearfix">
			 <div class="divcell">
				<label for="WorkCity">City<span class="screen-reader-only">Work Address</span></label><br>
				<input type="text" autocomplete="off" value="Alexandria" id="WorkCity" style="width:175px" maxlength="30" size="20" name="WorkCity" origval="Alexandria">
			 </div>
			 <div class="divcell">
				<label for="WorkState">State<span class="screen-reader-only">Work Address</span></label><br>
				<input type="text" autocomplete="off" value="VA" id="WorkState" style="width:150px"  maxlength="30" size="13" name="WorkState" origval="VA">
			 </div>
			 <div class="divcell">
				<label for="WorkZip">Postal Code<span class="screen-reader-only">Work Address</span></label><br>
				<input type="text" autocomplete="off" value="22314" style="width:125px" maxlength="20" size="10" id="WorkZip" name="WorkZip" origval="22314">
			 </div>
			 <div class="divcell">
				<label for="WorkCountry">Country<span class="screen-reader-only">Work Address</span></label><br>
				<select name="WorkCountry" id="WorkCountry" origval="US">
				   <option value="US" selected="selected">United States of America</option>
				</select>
			 </div>
		  </div>
	   </div>
	</div>
	<div id="HomeAddress" class="cnqr-panel cnqr-panel-default">
	   <div class="cnqr-panel-heading">
		  <h2>Home Address</h2>
	   </div>
	   <div class="cnqr-panel-body">
		  <div class="divcell">
			 <label for="HomeAddr">Street<span class="screen-reader-only">Home Address</span></label>
			 <textarea cols="40" style="width:100%" id="HomeAddr" name="HomeAddr" rows="2" >9017 Vernon View Drive</textarea>
		  </div>
		  <div class="divrow clearfix">
			 <div class="divcell">
				<label for="HomeCity">City<span class="screen-reader-only">Home Address</span></label><br>
				<input type="text" autocomplete="off" value="Alexandria" maxlength="30" size="20" style="width:100%" id="HomeCity" name="HomeCity" origval="Alexandria">
			 </div>
			 <div class="divcell">
				<label for="HomeState">State<span class="screen-reader-only">Home Address</span></label><br>
				<input type="text" autocomplete="off" value="VA" maxlength="30" size="15" style="width:100%" id="HomeState" name="HomeState" origval="VA">
			 </div>
			 <div class="divcell">
				<label for="HomeZip">Postal Code<span class="screen-reader-only">Home Address</span></label><br>
				<input type="text" autocomplete="off" value="22308" maxlength="20" size="10" style="width:100%" id="HomeZip" name="HomeZip" origval="22308">
			 </div>
			 <div class="divcell">
				<label for="HomeCountry">Country<span class="screen-reader-only">Home Address</span></label><br>
				<select  id="HomeCountry" name="HomeCountry">
				   <option value="">&nbsp;</option>
				   <option value="US" selected="selected">United States of America</option>
				</select>
			 </div>
		  </div>
	   </div>
	</div>			
{% endhighlight %}

<h3 id="bp10">Make sure you can navigate through your site using the keyboard only</h3>
<p>Take your mouse and put it in your drawer. Now, navigate your website with your keyboard alone!</p>

<h3 id="bp11">Data Tables - Use Headers</h3>
<table class="reporttable reporttable-lg">
	<tr>
		<th>Type</th>
		<th>Example</th>
	</tr>
	<tr>
		<td>
			<TABLE>
				<caption> Amount and brand of Tequilla consumed </caption>
				<tbody>
					<TR>
					   <TH id=”tableHeader1” >Name</TH>
						<TH id=”tableHeader2” >Serving Size (oz)</TH>
						<TH id=”tableHeader3” >Brand</TH>
					</TR>
					<TR>
						<TD headers=”tableHeader1” >Val</TD>
						<TD headers=”tableHeader2” >15</TD>
						<TD headers=”tableHeader3” >Jose Cuervo</TD>
					</TR>
					<TR>
						<TD headers=”tableHeader1” >Andrew</TD>
						<TD headers=”tableHeader2” >5</TD>
						<TD headers=”tableHeader3” >Bulldog</TD>
					</TR>
				</tbody>
			</TABLE>
		</td>
		<td>
			<h5>HTML</h5>
			{% highlight html %}
				<TABLE>
					<caption> Amount and brand of Tequilla consumed </caption>
					<tbody>
						<TR>
						   <TH id=”tableHeader1” >Name</TH>
							<TH id=”tableHeader2” >Serving Size (oz)</TH>
							<TH id=”tableHeader3” >Brand</TH>
						</TR>
						<TR>
							<TD headers=”tableHeader1” >Val</TD>
							<TD headers=”tableHeader2” >15</TD>
							<TD headers=”tableHeader3” >Jose Cuervo</TD>
						</TR>
						<TR>
							<TD headers=”tableHeader1” >Andrew</TD>
							<TD headers=”tableHeader2” >5</TD>
							<TD headers=”tableHeader3” >Bulldog</TD>
						</TR>
					</tbody>
				</TABLE>					
			{% endhighlight %}
		</td>
	</tr>

	<h3 id="bp12">Hover( Mouse users ) VS Focus ( Keyboard Users )</h3>
	<p>While styling elements, we should make sure that Hover and Focus have the exact same styling/behavior so both Mouse and Keyboard users share the same user experience.</p>

</table>
