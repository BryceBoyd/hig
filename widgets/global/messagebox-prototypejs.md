---
layout: default
jsLib: prototypejs
---

<table class="reporttable">
	<tr>
		<th>Type</th>
		<th>Example Code</th>
	</tr>
	<tr>
		<td><input type="button" class="btn btn-default cnqr-muted" onclick="CNQR.MessageBox.confirm('Lorem ipsum dolor sit amet, consectetur adipiscing elit.', {title:'Sample message title'})" value="Confirm" />
</td>
		<td>
		<h3> HTML </h3>
		{% highlight javascript %}
			<input type="button" class="btn btn-default cnqr-muted" onclick="CNQR.MessageBox.confirm('Lorem ipsum dolor sit amet, consectetur adipiscing elit.', {title:'Sample message title'})" value="Confirm Dialog" />
		{% endhighlight %}	
		</td>
	</tr>
	<tr>
		<td><input type="button" class="btn btn-success" value="Success" onclick="CNQR.MessageBox.alert('Nullam sagittis tincidunt malesuada.', {title:'Error message', icon:CNQR.MessageBox.UpArrowIcon})">
</td>
		<td>
		<h3> HTML </h3>
		{% highlight javascript %}
			<input type="button" class="btn btn-success" value="Success" onclick="CNQR.MessageBox.alert('Nullam sagittis tincidunt malesuada.', {title:'Error message', icon:CNQR.MessageBox.UpArrowIcon})">
		{% endhighlight %}	
		</td>
	</tr>	
	<tr>
		<td><input type="button" class="btn btn-info" value="Info" onclick="CNQR.MessageBox.alert('Phasellus tristique tristique blandit. Nullam pellentesque porttitor orci. Nunc eros turpis, ultrices ut consequat in, rhoncus vitae metus. Pellentesque sit amet rutrum augue, a placerat odio. Mauris blandit pharetra sapien, id placerat orci tempus eget. Aliquam interdum neque a metus molestie, ut rhoncus justo hendrerit. In aliquam porttitor mauris at luctus. In ullamcorper tristique hendrerit.', {title:'Info message', icon:CNQR.MessageBox.InfoIcon})">
</td>
		<td>
		<h3> HTML </h3>
		{% highlight javascript %}
		<input type="button" class="btn btn-info" value="Info" onclick="CNQR.MessageBox.alert('Phasellus tristique tristique blandit. Nullam pellentesque porttitor orci. Nunc eros turpis, ultrices ut consequat in, rhoncus vitae metus. Pellentesque sit amet rutrum augue, a placerat odio. Mauris blandit pharetra sapien, id placerat orci tempus eget. Aliquam interdum neque a metus molestie, ut rhoncus justo hendrerit. In aliquam porttitor mauris at luctus. In ullamcorper tristique hendrerit.', {title:'Info message', icon:CNQR.MessageBox.InfoIcon})">
		{% endhighlight %}	
		</td>
	</tr>	
	<tr>
		<td><input type="button" class="btn btn-warning" value="Warning" onclick="CNQR.MessageBox.alert('Nunc lobortis, nisi eget rhoncus pellentesque, eros mauris gravida nisi, a aliquet dolor odio quis nisi. Donec sed lectus eu diam malesuada placerat eget non ipsum. Ut auctor nisi ac nibh convallis dignissim.', {title:'Warning message'})">
</td>
		<td>
		<h3> HTML </h3>
		{% highlight javascript %}
		<input type="button" class="btn btn-warning" value="Warning" onclick="CNQR.MessageBox.alert('Nunc lobortis, nisi eget rhoncus pellentesque, eros mauris gravida nisi, a aliquet dolor odio quis nisi. Donec sed lectus eu diam malesuada placerat eget non ipsum. Ut auctor nisi ac nibh convallis dignissim.', {title:'Warning message'})">
		{% endhighlight %}	
		</td>
	</tr>	
	<tr>
		<td><input type="button" class="btn btn-danger" value="Error" onclick="CNQR.MessageBox.alert('Aliquam vestibulum risus porta arcu egestas rhoncus. Nulla vehicula, elit eget porta ultricies,', {title:'Error message', icon:CNQR.MessageBox.ErrorIcon})">
</td>
		<td>
		<h3> HTML </h3>
		{% highlight javascript %}
		<input type="button" class="btn btn-danger" value="Error" onclick="CNQR.MessageBox.alert('Aliquam vestibulum risus porta arcu egestas rhoncus. Nulla vehicula, elit eget porta ultricies,', {title:'Error message', icon:CNQR.MessageBox.ErrorIcon})">
		{% endhighlight %}	
		</td>
	</tr>	

</table>
