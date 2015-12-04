---
layout: reference
title: panels
---

## Panel (Available in all themes) ##

### Basic Usage ###

Our panels follow the basic Bootstrap panel container convention (<a href="http://getbootstrap.com/components/#panels">Bootstrap Panels</a>), except with each class prefixed with "cnqr-"

### Panel with optional heading ###

By default, all the .cnqr-panel does is apply some basic border and padding to contain some content.

Easily add a heading container to your panel with <code>.cnqr-panel-heading</code>. You may also include any <code>&lt;h1&gt;</code>-<code>&lt;h6&gt;</code> with a <code>.panel-title</code> class to add a pre-styled heading.

### Types ###
<table class="reporttable">
	<tr>
		<th style="width:30%">Type</th>
		<th style="width:70%">Example</th>
	</tr>
	<tr>
		<td>
			<h5>Default</h5>
			<div class="cnqr-panel cnqr-panel-default">
				<div class="cnqr-panel-heading">
					Panel Heading (optional)
				</div>
				<div class="cnqr-panel-body">
					Panel content
				</div>
			</div>
			<br/>
			<h5>Default, muted</h5>
			<div class="cnqr-panel cnqr-panel-default cnqr-muted">
				<div class="cnqr-panel-heading">
					Panel Heading (optional)
				</div>
				<div class="cnqr-panel-body">
					Panel content
				</div>
			</div>

		</td>
		<td>
			<h5>HTML</h5>
{% highlight html %}
<div class="cnqr-panel cnqr-panel-default">
	<div class="cnqr-panel-heading">
		Panel Heading (optional)
	</div>
	<div class="cnqr-panel-body">
		Panel content
	</div>
</div>					
{% endhighlight %}

{% highlight html %}
<div class="cnqr-panel cnqr-panel-default cnqr-muted">
	<div class="cnqr-panel-heading">
		Panel Heading (optional)
	</div>
	<div class="cnqr-panel-body">
		Panel content
	</div>
</div>					
{% endhighlight %}
		</td>
	</tr>
	<tr>
		<td>
			<h5>Primary</h5>
			<div class="cnqr-panel cnqr-panel-primary">
				<div class="cnqr-panel-heading">
					Panel Heading (optional)
				</div>
				<div class="cnqr-panel-body">
					Panel content
				</div>
			</div>
			<br/>
			<h5>Primary, muted</h5>
			<div class="cnqr-panel cnqr-panel-primary cnqr-muted">
				<div class="cnqr-panel-heading">
					Panel Heading (optional)
				</div>
				<div class="cnqr-panel-body">
					Panel content
				</div>
			</div>

		</td>
		<td>
			<h5>HTML</h5>
{% highlight html %}
<div class="cnqr-panel cnqr-panel-primary">
	<div class="cnqr-panel-heading">
		Panel Heading (optional)
	</div>
	<div class="cnqr-panel-body">
		Panel content
	</div>
</div>

<div class="cnqr-panel cnqr-panel-primary cnqr-muted">
	<div class="cnqr-panel-heading">
		Panel Heading (optional)
	</div>
	<div class="cnqr-panel-body">
		Panel content
	</div>
</div>				
{% endhighlight %}

		</td>
	</tr>
	<tr>
		<td>
			<h5>Success</h5>
			<div class="cnqr-panel cnqr-panel-success">
				<div class="cnqr-panel-heading">
					Panel Heading (optional)
				</div>
				<div class="cnqr-panel-body">
					Panel content
				</div>
			</div>
		</td>
		<td>
			<h5>HTML</h5>
{% highlight html %}
<div class="cnqr-panel cnqr-panel-success">
	<div class="cnqr-panel-heading">
		Panel Heading (optional)
	</div>
	<div class="cnqr-panel-body">
		Panel content
	</div>
</div>			
{% endhighlight %}
		</td>
	</tr>
	<tr>
		<td>
			<h5>Info</h5>
			<div class="cnqr-panel cnqr-panel-info">
				<div class="cnqr-panel-heading">
					Panel Heading (optional)
				</div>
				<div class="cnqr-panel-body">
					Panel content
				</div>
			</div>
		</td>
		<td>
			<h5>HTML</h5>
{% highlight html %}
<div class="cnqr-panel cnqr-panel-info">
	<div class="cnqr-panel-heading">
		Panel Heading (optional)
	</div>
	<div class="cnqr-panel-body">
		Panel content
	</div>
</div>		
{% endhighlight %}
		</td>
	</tr>
	<tr>
		<td>
			<h5>Warning</h5>
			<div class="cnqr-panel cnqr-panel-warning">
				<div class="cnqr-panel-heading">
					Panel Heading (optional)
				</div>
				<div class="cnqr-panel-body">
					Panel content
				</div>
			</div>
		</td>
		<td>
			<h5>HTML</h5>
{% highlight html %}
<div class="cnqr-panel cnqr-panel-warning">
	<div class="cnqr-panel-heading">
		Panel Heading (optional)
	</div>
	<div class="cnqr-panel-body">
		Panel content
	</div>
</div>		
{% endhighlight %}
		</td>
	</tr>
	<tr>
		<td>
			<h5>Danger</h5>
			<div class="cnqr-panel cnqr-panel-danger">
				<div class="cnqr-panel-heading">
					Panel Heading (optional)
				</div>
				<div class="cnqr-panel-body">
					Panel content
				</div>
			</div>
		</td>
		<td>
			<h5>HTML</h5>
{% highlight html %}
<div class="cnqr-panel cnqr-panel-danger">
	<div class="cnqr-panel-heading">
		Panel Heading (optional)
	</div>
	<div class="cnqr-panel-body">
		Panel content
	</div>
</div>		
{% endhighlight %}
		</td>
	</tr>
</table>
