---
layout: default
jsLib: jquery
---

<table class="reporttable">
	<tr>
		<th>Type</th>
		<th>Example Code</th>
	</tr>
	<tr>
		<td>
			<label for="calendar.input">@singleLabel</label>
			@Html.DateTextBox(
				"calendar.input", 
				DateTime.Now, 
				null, 
				new { Class="form-control" },
				new { minDate = 0}
			)
		</td>
		<td>
<h5>.Net Helper</h5>
{% highlight c# linenos%}
	@Html.DateTextBox(
		"calendar",				// Name
		DateTime.Now,				// Optional DateTime value
		null,					// Optional Group name string 
		new { Class="form-control" },		// Optional htmlAttributes Object
		new { minDate = 0}			// Optional datePickerOptions object
	)
{% endhighlight %}
		</td>
	</tr>
	<tr>
		<td>
			<div>
				<label for="@calendarName1">Start Date</label>
				@Html.DateTextBox(
					calendarName1, 
					DateTime.Now, 
					linkedCalGroup, 
					new { Class="form-control" },
					new { minDate = 0, groupMinDate = 3}
				)
			</div>

			<div>
				<label for="@calendarName2">End Date</label>
				@Html.DateTextBox(
					calendarName2, 
					DateTime.Now, 
					linkedCalGroup, 
					new { Class="form-control" },
					null
				)
			</div>
		</td>
		<td>
<h5>.Net Helper</h5>
{% highlight c# linenos%}
	@Html.DateTextBox
		// Should be unique (otherwise, add an id to htmlAttributes)
		"@calendarName1",		
		
		// Start with today's date				
		DateTime.Now,
		
		// This value is used to link calendars together				
		"@linkedCalGroup",						
		new { Class="form-control"},
		
		// groupMinDate determines the linked calendar's mininum begin
		// number of days. In this demo, if you choose today's date in 	
		// the first linked calendar, the second will begin 3 days later		
		new { minDate = 0, groupMinDate = 3}	
	)											
											
	@@Html.DateTextBox(
		// Should be unique (otherwise, add an id to htmlAttributes)
		"@calendarName2",		
		
		// Start with today's date					
		DateTime.Now, 
		
		// This value is used to link calendars together
		"@linkedCalGroup",
		
		// Add a custom class						
		new { Class="form-control" }
	)
{% endhighlight %}
		</td>
	</tr>
</table>

### Accessibilty ###
You can use keyboard shortcuts to drive the datepicker:
* **page up/down** - previous/next month
* **ctrl+page up/down** - previous/next year
* **ctrl+home** - current month or open when closed
* **ctrl+left/right** - previous/next day
* **ctrl+up/down** - previous/next week
* **enter** - accept the selected date
* **ctrl+end** - close and erase the date
* **escape** - close the datepicker without selection
