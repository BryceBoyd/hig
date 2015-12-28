---
layout: reference
title: Global - Tooltips
---

<table class="reporttable">
	<tr>
		<th>Type</th>
		<th>Example</th>
	</tr>
	<tr>
		<td>
			<h4>Helper Tooltip with plain text</h4>
			<p>Helper Tootips are initliazed on <i><u><strong>click</strong></u></i> event</p>
			<div class="divcell">
				<span class="cnqr-show">
					<label for="DepAirport">@OTGetUserMessage("TravelTemplates", "DepartureCity")</label>
					@Html.ToolTip(OTGetUserMessage("Profile", "AirportSelectorHelp"))
				</span>
				@Html.AirportAutoComplete("DepAirport", null, null,null,null,true)
			</div>
		</td>
		<td>
			<h5>HTML</h5>
{% highlight html linenos%}
<div class="divcell">
  <span class="cnqr-show">
  	<label for="DepAirport">
  		@@OTGetUserMessage("TravelTemplates", "DepartureCity")
  	</label>
  
  	/**
  	@@Html.ToolTip Parameters:
  	* String text               |   Tooltip text
  	* Object htmlAttributes     |   Optional html attributes
  	*/
  	@@Html.ToolTip(OTGetUserMessage("Profile", "AirportSelectorHelp"))
  </span>
  @@Html.AirportAutoComplete("DepAirport", null, null,null,null,true)
</div>
{% endhighlight %}
		</td>
	</tr>
	<tr>
		<td>
			<h4>Helper Tooltip with HTML</h4>
			<p>Helper Tootips are initialized on <i><u><strong>click</strong></u></i> event</p>
			<div class="divcell clearfix">
				<p>
					@OTGetUserMessage("CompanyAdmin", "IfAEAUnavailable"):
					@Html.ToolTip( OTGetUserMessage( "CompanyAdmin", "IfAEAUnavailableTip1") + htmlContent ) 
				</p>
				<input id="example1" type="radio" value="USE_LLF" name="example1">
				<label for="example1">Lowest Logical Fare</label>
			</div>
		</td>
		<td>
			<h5>HTML</h5>
			{% highlight html linenos%}
				<div class="divcell clearfix">
					<p>
						@@OTGetUserMessage("CompanyAdmin", "IfAEAUnavailable"):

						/**
						@@Html.ToolTip Parameters:
						* String text               |   Tooltip text
						* Object htmlAttributes     |   Optional html attributes
						*/
						@@Html.ToolTip( 
							OTGetUserMessage( "CompanyAdmin", "IfAEAUnavailableTip1") + htmlContent 
						) 
					</p>
					<input id="example1" type="radio" value="USE_LLF" name="example1">
					<label for="example1">Lowest Logical Fare</label>
				</div>
			{% endhighlight%}
		</td>
	</tr>
</table>

