---
layout: default
jsLib: prototypejs
---

<table class="reporttable reporttable-lg">
	<tbody><tr>
		<th>Type</th>
		<th>Example</th>
	</tr>

	<tr>
		<td>
		<button type="button" 
			data-toggle="popover"
			data-placement="left"
			data-title="Popover Left Title"
			data-type="info"
			data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
			Info
		</button> 
		</td>
		<td>
			<h5>HTML</h5>
{% highlight html linenos %}
<button type="button" 
	data-toggle="popover"
	data-placement="left"
	data-title="Popover Left Title"
	data-type="info"
	data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
	Info
</button> 
{% endhighlight %}
</td>
	</tr>

	<tr>
		<td>
		<button type="button" 
			class="btn btn-success"
			data-toggle="popover"
			data-placement="bottom"
			data-title="Popover Success"
			data-type="success"
			data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
			Success
		</button> 

		</td>
		<td>
			<h5>HTML</h5>
{% highlight html linenos %}
<button type="button" 
	class="btn btn-success"
	data-toggle="popover"
	data-placement="bottom"
	data-title="Popover Success"
	data-type="success"
	data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
	Success
</button> 
{% endhighlight %}			
		</td>
	</tr>

	<tr>
		<td>
		<button
			class="btn btn-warning"
			data-toggle="popover"
			data-placement="top"
			data-title="Popover Warning"
			data-type="warning"
			data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
			Warning
		</button> 
		</td>
		<td>
			<h5>HTML</h5>
{% highlight html linenos %}
<button
	class="btn btn-warning"
	data-toggle="popover"
	data-placement="top"
	data-title="Popover Warning"
	data-type="warning"
	data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
	Warning
</button> 
{% endhighlight %}			
		</td>
	</tr>

	<tr>
		<td>
		<button
			class="btn btn-danger"
			data-toggle="popover"
			data-placement="right"
			data-title="Popover Danger"
			data-type="danger"
			data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
			Danger
		</button>
		</td>
		<td>
			<h5>HTML</h5>
{% highlight html linenos %}
<button
	class="btn btn-danger"
	data-toggle="popover"
	data-placement="right"
	data-title="Popover Danger"
	data-type="danger"
	data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
	Danger
</button>
{% endhighlight %}			
		</td>
	</tr>

	<tr>
		<td>
		<button type="button" 
			class="btn btn-default cnqr-muted"
			data-toggle="popover"
			data-placement="left"
			data-type="info"
			data-content="No title">
			Info
		</button> 

		</td>
		<td>
			<h5>HTML</h5>
{% highlight html linenos %}
<button type="button" 
	class="btn btn-default cnqr-muted"
	data-toggle="popover"
	data-placement="left"
	data-type="info"
	data-content="No title">
	Default With No Title
</button> 
{% endhighlight %}			
		</td>
	</tr>

	<tr>
		<td>
		<button type="button" 
			class="btn btn-default cnqr-muted"
			data-toggle="popover"
			data-placement="left"
			data-type="info"
			data-content="#cnqr-hig-popup-content">
			Element As Content
		</button> 
		
		<div id="cnqr-hig-popup-content" class="cnqr-hide">hello from cnqr-hig-popup-content!</div>
		</td>
		<td>
			<h5>HTML</h5>
{% highlight html linenos %}
<button type="button" 
	class="btn btn-default cnqr-muted"
	data-toggle="popover"
	data-placement="left"
	data-type="info"
	data-content="#cnqr-hig-popup-content">
	Element As Content
</button> 
<div id="cnqr-hig-popup-content" class="cnqr-hide">hello from cnqr-hig-popup-content!</div>
{% endhighlight %}			
		</td>
	</tr>
	<tr>
		<td>
		<button type="button" 
			class="btn btn-default cnqr-muted"
			data-toggle="popover"
			data-placement="left"
			data-type="info"
			data-url="/UI/docs/Widgets/GetPopOverContent">
			AJAX Content
		</button> 
		
		</td>
		<td>
			<h5>HTML</h5>
{% highlight html linenos %}
<button type="button" 
	class="btn btn-default cnqr-muted"
	data-toggle="popover"
	data-placement="left"
	data-type="info"
	data-url="/UI/docs/Widgets/GetPopOverContent">
	AJAX Content
</button> 
{% endhighlight %}			
		</td>
	</tr>

</tbody></table>
