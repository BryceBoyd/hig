---
layout: default
title: Badges
requireCss: /static/less/cnqr-view/docs.less
---

## Badges (Available in all themes ##

### Basic Usage ###

Our badges follow the basic Bootstrap badge convention (<a href="http://getbootstrap.com/components/#badges">Bootstrap Badges</a>)

### Types ###

| Types         | Display                       |  HTML                         | 
| ------------- |-------------------------------|-------------------------------|
| **Alone**     | <span class="badge">42</span> | ```<span class="badge">42</span>```|

<table>
	<tr>
		<th style="width:30%">Type</th>
		<th style="width:70%">Example</th>
	</tr>
	<tr>
		<td>
			<h5>Alone</h5>
			<span class="badge">42</span>
		</td>
		<td>
			<h5>HTML</h5>
			<pre class="brush: xml; toolbar: false;">
				<span class="badge">42</span>
			</pre>
		</td>
	</tr>
	<tr>
		<td>
			<h5>In a link</h5>
			<a href="#">Inbox <span class="badge">42</span></a>
		</td>
		<td>
			<h5>HTML</h5>
			<pre class="brush: xml; toolbar: false;">
				<a href="#">Inbox <span class="badge">42</span></a>
			</pre>
		</td>
	</tr>
	<tr>
		<td>
			<h5>In a button</h5>
			<p><button type="button"> Messages <span class="badge">4</span></button></p>
			<p><button type="button" class="btn btn-default"> Messages <span class="badge">4</span></button></p>
			<p><button type="button" class="btn btn-primary"> Messages <span class="badge">4</span></button></p>
			<p><button type="button" class="btn btn-success"> Messages <span class="badge">4</span></button></p>
			<p><button type="button" class="btn btn-info"> Messages <span class="badge">4</span></button></p>
			<p><button type="button" class="btn btn-warning"> Messages <span class="badge">4</span></button></p>
			<p><button type="button" class="btn btn-danger"> Messages <span class="badge">4</span></button></p>
		</td>
		<td>
			<h5>HTML</h5>
			<pre class="brush: xml; toolbar: false;">
				<button type="button"> Messages <span class="badge">4</span></button>

				<button type="button" class="btn btn-default"> Messages <span class="badge">4</span></button>

				<button type="button" class="btn btn-primary"> Messages <span class="badge">4</span></button>

				<button type="button" class="btn btn-success"> Messages <span class="badge">4</span></button>

				<button type="button" class="btn btn-info"> Messages <span class="badge">4</span></button>

				<button type="button" class="btn btn-warning"> Messages <span class="badge">4</span></button>

				<button type="button" class="btn btn-danger"> Messages <span class="badge">4</span></button>
			</pre>
		</td>
	</tr>

</table>
