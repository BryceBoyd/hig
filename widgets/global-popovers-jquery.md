---
layout: default
jsLib: jquery
---

<table class="reporttable reporttable-lg">
	<tbody><tr>
		<th>Type</th>
		<th>Example</th>
	</tr>

	<tr>
		<td>
			<button data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus." data-type="info" data-title="Popover Info" data-placement="top" data-toggle="popover" class="ui-button ui-button-info ui-corner-all" type="button">
				Info
			</button>
		</td>
		<td>
			<h5>HTML</h5>
{% highlight html linenos %}			
<button 
	data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus." 
	data-type="info" 
	data-title="Popover Info" 
	data-placement="top" 
	data-toggle="popover" 
	class="ui-button ui-button-info ui-corner-all" 
	type="button"
>
	Info
</button>	
{% endhighlight %}
</td>
	</tr>

	<tr>
		<td>
			<button data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus." data-type="success" data-title="Popover Success" data-placement="left" data-toggle="popover" class="ui-button ui-button-success ui-corner-all" type="button">
			Success
			</button>
		</td>
		<td>
			<h5>HTML</h5>
{% highlight html linenos %}				
<button 
	data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus." 
	data-type="success" 
	data-title="Popover Success" 
	data-placement="left" 
	data-toggle="popover" 
	class="ui-button ui-button-success ui-corner-all" 
	type="button"
>
	Success
</button>
{% endhighlight %}			
		</td>
	</tr>

	<tr>
		<td>
			<button data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus." data-type="warning" data-title="Popover Warning" data-placement="right" data-toggle="popover" class="ui-button ui-button-warning ui-corner-all" type="button">
				Warning
			</button>
		</td>
		<td>
			<h5>HTML</h5>
{% highlight html linenos %}		
<button 
	data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus." 
	data-type="warning" 
	data-title="Popover Warning" 
	data-placement="right" 
	data-toggle="popover" 
	class="ui-button ui-button-warning ui-corner-all" type="button"
>
	Warning
</button>
{% endhighlight %}			
		</td>
	</tr>

	<tr>
		<td>
			<button data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus." data-type="danger" data-title="Popover Danger" data-placement="bottom" data-toggle="popover" class="ui-button ui-button-danger ui-corner-all" type="button">
				Danger
			</button>
		</td>
		<td>
			<h5>HTML</h5>
{% highlight html linenos  %}			
<button 
	data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus." 
	data-type="danger" 
	data-title="Popover Danger" 
	data-placement="bottom" 
	data-toggle="popover" 
	class="ui-button ui-button-danger ui-corner-all" 
	type="button"
>
	Danger
</button>
{% endhighlight %}			
		</td>
	</tr>

	<tr>
		<td>
			<button data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus." data-placement="bottom" data-toggle="popover" class="ui-button ui-corner-all cnqr-muted" type="button">
				Default With No Title
			</button>
		</td>
		<td>
			<h5>HTML</h5>
{% highlight html linenos  %}
<button 
	data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus." 
	data-placement="bottom" 
	data-toggle="popover" 
	class="ui-button ui-corner-all cnqr-muted" 
	type="button"
>
	Default With No Title
</button>
{% endhighlight %}			
		</td>
	</tr>

	<tr>
		<td>
			<button data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus." data-title="PopOver with title" data-placement="left" data-toggle="popover" class="ui-button ui-corner-all cnqr-muted" type="button">
				Default With Title
			</button>
		</td>
		<td>
			<h5>HTML</h5>
{% highlight html linenos  %}			
<button 
	data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus." 
	data-title="PopOver with title" 
	data-placement="left" 
	data-toggle="popover" 
	class="ui-button ui-corner-all cnqr-muted" 
	type="button"
>
	Default With Title
</button>
{% endhighlight %}	
		</td>
	</tr>

	<tr>
		<td>
			<button data-width="400" data-content="#cnqr-hig-popup-content" data-title="Element As Content" data-placement="left" data-toggle="popover" class="ui-button ui-corner-all cnqr-muted" type="button">
				Element As Content
			</button>
<div id="cnqr-hig-popup-content" class="cnqr-hide">hello from cnqr-hig-popup-content!</div>			
		</td>
		<td>
			<h5>HTML</h5>
{% highlight html linenos  %}			
<button 
	data-width="400" 
	data-content="#cnqr-hig-popup-content" 
	data-title="Element As Content" 
	data-placement="left" 
	data-toggle="popover" 
	class="ui-button ui-corner-all cnqr-muted" 
	type="button"
>
	Element As Content
</button>
			
<div id="cnqr-hig-popup-content" class="cnqr-hide">
	hello from cnqr-hig-popup-content!
</div>			
{% endhighlight %}				
		</td>
	</tr>

	<tr>
		<td>
			<button data-url="/UI/docs/Widgets/GetPopOverContent" data-placement="right" data-title="AJAX Content" data-toggle="popover" class="ui-button ui-corner-all cnqr-muted" type="button">
				AJAX Content
			</button>
		</td>
		<td>
			<h5>HTML</h5>
{% highlight html linenos %}				
<button 
	data-url="/UI/docs/Widgets/GetPopOverContent" 
	data-placement="right" 
	data-title="AJAX Content" 
	data-toggle="popover" 
	class="ui-button ui-corner-all cnqr-muted" 
	type="button"
>
	AJAX Content
</button>
{% endhighlight %}				
		</td>
	</tr>

	<tr>
		<td>
			<h4>Validation Popover</h4>
			<p>Validation Popover are initialized on focus, click, and mouse events</p>
			<div class="divcell">
				<!-- DO NOT COPY THIS CODE. THIS CODE GETS GENERATED BY MODEL DATA ANNOTATIONS ATTRIBUTES. THIS STATIC EXAMPLE IS ONLY USED AS AN EXAMPLE -->
					<p>The following input has a label</p>
					<label class="cnqr-validation-label-error" for="Address">Address&nbsp;<span class="field-required">*</span></label>		
					<div class="editor-field">
						<input type="text" data-showclosebtn="false" data-type="danger" data-title="Error" data-content="Please enter a value for the Address." data-class="cnqr-tooltip-validation" data-showon="mouseover" data-toggle="popover" class="input-validation-error" data-val="true" data-val-required="Please enter a value for the Address." id="Address" name="Address" value="">
						<span style="display: none;" class="field-validation-error" data-valmsg-for="Address" data-valmsg-replace="true"></span>
					</div>
				<!-- -->
			</div>
			<div class="divcell"></div>
			<div class="divcell">
				<!-- DO NOT COPY THIS CODE. THIS CODE GETS GENERATED BY MODEL DATA ANNOTATIONS ATTRIBUTES. THIS STATIC EXAMPLE IS ONLY USED AS AN EXAMPLE -->
					<p>The following input has NO label</p>
					<div class="editor-field">
						<input type="text" data-showclosebtn="false" data-type="danger" data-title="Error" data-content="Please enter a value for the Address" data-class="cnqr-tooltip-validation" data-showon="mouseover" data-toggle="popover" class="input-validation-error" data-val="true" data-val-required="Please enter a value for the Address" id="noLabel" name="NoLabel" value="">
						<span style="display: none;" class="field-validation-error" data-valmsg-for="Address" data-valmsg-replace="true"></span>
					</div>
				<!-- -->
			</div>
		</td>
		<td>
			<h5>HTML</h5>
{% highlight html linenos%}	
<!-- DO NOT COPY THIS CODE. 
THIS CODE GETS GENERATED BY MODEL DATA ANNOTATIONS ATTRIBUTES. 
THIS STATIC EXAMPLE IS ONLY USED AS AN EXAMPLE 
-->
<div class="divcell">
	<p>The following input has a label</p>
	<label class="cnqr-validation-label-error" for="Address">
		Address&nbsp;
		<span class="field-required">*</span>
	</label>		
	<div class="editor-field">
		<input type="text" 
			data-showclosebtn="false" 
			data-type="danger" 
			data-title="Error" 
			data-content="Please enter a value for the Address." 
			data-class="cnqr-tooltip-validation" 
			data-showon="mouseover" 
			data-toggle="popover" 
			data-val="true" 
			data-val-required="Please enter a value for the Address." 
			class="input-validation-error" 
			id="Address" 
			name="Address" 
			value=""
		>
		<span 
			style="display: none;" 
			class="field-validation-error" 
			data-valmsg-for="Address" 
			data-valmsg-replace="true">
		</span>
	</div>
</div>
<br>
<br>
<!-- DO NOT COPY THIS CODE. 
THIS CODE GETS GENERATED BY MODEL DATA ANNOTATIONS ATTRIBUTES. 
THIS STATIC EXAMPLE IS ONLY USED AS AN EXAMPLE 
-->
<div class="divcell">
	<p>The following input has NO label</p>
	<div class="editor-field">
		<input 
			type="text" 
			data-showclosebtn="false" 
			data-type="danger" 
			data-title="Error" 
			data-content="Please enter a value for the Address" 
			data-class="cnqr-tooltip-validation" 
			data-showon="mouseover" 
			data-toggle="popover" 
			class="input-validation-error" 
			data-val="true" 
			data-val-required="Please enter a value for the Address" 
			id="noLabel" 
			name="NoLabel" 
			value=""
		>
		<span 
			style="display: none;" 
			class="field-validation-error" 
			data-valmsg-for="Address" 
			data-valmsg-replace="true">
		</span>
	</div>
</div>
{% endhighlight %}	
		</td>
	</tr>
</tbody></table>
