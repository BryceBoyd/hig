---
layout: reference
title: Form Elements
---

## Gateway Style Form Elements ##

Class "form-control" required when sizing form elements (large or small). It is optional for default element size

### HTML Form Element Controls sizing ###
<table class="reporttable">
	<tr>
		<th>CSS System</th>
		<th>Button Class</th>
		<th>Button (for comparison)</th>
		<th>Text Input </th>
		<th>Select</th>
		<th>Select<br/>(with size or multiple attribute)</th>
		<th>Checkbox</th>
		<th>Radio</th>
		<th>Textarea</th>
		<th>Input Class</th>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-lg</td>
		<td><button class="btn btn-default btn-lg" type="submit">Button</button></td>
		<td><input class="form-control input-lg" type="text" value="Input"></td>
		<td>
			<select class="form-control input-lg">
				<option>Option 1</option>
				<option>Option 2</option>
				<option>Option 3</option>
			</select>
		</td>
		<td>
			<select size="3" class="form-control input-lg">
				<option>Option 1</option>
				<option>Option 2</option>
				<option>Option 3</option>
			</select>
		</td>
		<td class="text-center">N/A</td>
		<td class="text-center">N/A</td>
		<td><textarea class="form-control input-lg">Hello World</textarea></td>
		<td>.form-control .input-lg</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn</td>
		<td><button class="btn btn-default" type="submit">Button</button></td>
		<td><input class="form-control" type="text" value="Input"></td>
		<td>
			<select class="form-control">
				<option>Option 1</option>
				<option>Option 2</option>
				<option>Option 3</option>
			</select>
		</td>
		<td>
			<select size="3" class="form-control">
				<option>Option 1</option>
				<option>Option 2</option>
				<option>Option 3</option>
			</select>
		</td>
		<td class="text-center">N/A</td>
		<td class="text-center">N/A</td>
		<td><textarea class="form-control">Hello World</textarea></td>
		<td>.form-control</td>
	</tr>
	<tr>
		<td>None</td>
		<td>[unclassed]</td>
		<td><button type="submit">Button</button></td>
		<td><input type="text" value="Input"></td>
		<td>
			<select>
				<option>Option 1</option>
				<option>Option 2</option>
				<option>Option 3</option>
			</select>
		</td>
		<td>
			<select size="3">
				<option>Option 1</option>
				<option>Option 2</option>
				<option>Option 3</option>
			</select>
		</td>
		<td class="text-center"><input type="checkbox" /></td>
		<td class="text-center"><input type="radio"/></td>
		<td><textarea>Hello World</textarea></td>
		<td>[unclassed]</td>
	</tr>

	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-sm</td>
		<td><button class="btn btn-default btn-sm" type="submit">Button</button></td>
		<td><input class="form-control input-sm" type="text" value="Input"></td>
		<td>
			<select class="form-control input-sm">
				<option>Option 1</option>
				<option>Option 2</option>
				<option>Option 3</option>
			</select>
		</td>
		<td>
			<select size="3" class="form-control input-sm">
				<option>Option 1</option>
				<option>Option 2</option>
				<option>Option 3</option>
			</select>
		</td>
		<td class="text-center">N/A</td>
		<td class="text-center">N/A</td>
		<td><textarea class="form-control input-sm">Hello World</textarea></td>
		<td>.form-control .input-sm</td>
	</tr>

	<tr>
		<td>disabled attribute</td>
		<td>.btn .btn-sm</td>
		<td><button class="btn btn-default" type="submit" disabled="disabled">Button</button></td>
		<td><input class="form-control" type="text" value="Input" disabled="disabled"></td>
		<td>
			<select class="form-control" disabled="disabled">
				<option>Option 1</option>
				<option>Option 2</option>
				<option>Option 3</option>
			</select>
		</td>
		<td>
			<select size="3" class="form-control" disabled="disabled">
				<option>Option 1</option>
				<option>Option 2</option>
				<option>Option 3</option>
			</select>
		</td>
		<td class="text-center"><input type="checkbox" disabled="disabled"/></td>
		<td class="text-center"><input type="radio" disabled="disabled"/></td>
		<td><textarea class="form-control" disabled="disabled">Hello World</textarea></td>
		<td>.form-control</td>
	</tr>
	
	<tr>
		<td>readonly attribute</td>
		<td>.btn .btn-sm</td>
		<td>N/A</td>
		<td><input class="form-control" type="text" value="Input" readonly="readonly"></td>
		<td class="text-center">N/A</td>
		<td class="text-center">N/A</td>
		<td class="text-center">N/A</td>
		<td class="text-center">N/A</td>
		<td><textarea class="form-control" readonly="readonly">Hello World</textarea></td>
		<td>.form-control</td>
	</tr>

</table>
	
### Complex Controls sizing ###
<table class="reporttable">
	<tr>
		<th>CSS System</th>
		<th>Button Class</th>
		<th>Button (for comparison)</th>
		<th>Text Input (for comparison)</th>
		<th>File Input</th>
		<th>File Input with path</th>
		<th>Input Group</th>
		<th>Input Class</th>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-lg</td>
		<td><button class="btn btn-default btn-lg" type="submit">Button</button></td>
		<td><input class="form-control input-lg" type="text" value="Input"></td>
		<td><span class="btn btn-default btn-lg btn-file">Browse... <input type="file"></span></td>
		<td>
			<div class="input-group input-group-lg">
				<span class="input-group-btn">
					<span class="btn btn-default btn-file">Browse... <input type="file"></span>
				</span>
				<input class="form-control" type="text" value="Input">
			</div>
		</td>
		<td>
			<div class="input-group input-group-lg">
				<a class="input-group-addon icon-calendar cnqr-condensed" role="button"></a>
				<input type="text" value="08/04/2015" title="MM/dd/yyyy" name="calendar" maxlength="20" id="calendar" data-type="date" class="form-control hasDatepicker" autocomplete="off">
			</div>
		</td>
		<td>.form-control .input-lg</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn</td>
		<td><button class="btn btn-default" type="submit">Button</button></td>
		<td><input class="form-control" type="text" value="Input"></td>
		<td><span class="btn btn-default btn-file">Browse... <input type="file"></span></td>
		<td>
			<div class="input-group">
				<span class="input-group-btn">
					<span class="btn btn-default btn-file">Browse... <input type="file"></span>
				</span>
				<input class="form-control" type="text" value="Input">
			</div>
		</td>
		<td>
			<div class="input-group">
				<a class="input-group-addon icon-calendar cnqr-condensed" role="button"></a>
				<input type="text" value="08/04/2015" title="MM/dd/yyyy" name="calendar" maxlength="20" id="calendar" data-type="date" class="form-control hasDatepicker" autocomplete="off">
			</div>
		</td>
		<td>.form-control</td>
	</tr>
	<tr>
		<td>None</td>
		<td>[unclassed]</td>
		<td><button type="submit">Button</button></td>
		<td><input type="text" value="Input"></td>
		<td>N/A</td>
		<td><input type="file"></td>
		<td>N/A</td>
		<td>[unclassed]</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-sm</td>
		<td><button class="btn btn-default btn-sm" type="submit">Button</button></td>
		<td><input class="form-control input-sm" type="text" value="Input"></td>
		<td><span class="btn btn-default btn-sm btn-file">Browse... <input type="file"></span></td>
		<td>
			<div class="input-group input-group-sm">
				<span class="input-group-btn">
					<span class="btn btn-default btn-file">Browse... <input type="file"></span>
				</span>
				<input class="form-control" type="text" value="Input">
			</div>
		</td>
		<td>
			<div class="input-group input-group-sm">
				<a class="input-group-addon icon-calendar cnqr-condensed" role="button"></a>
				<input type="text" value="08/04/2015" title="MM/dd/yyyy" name="calendar" maxlength="20" id="calendar" data-type="date" class="form-control hasDatepicker" autocomplete="off">
			</div>
		</td>
		<td>.form-control .input-sm</td>
	</tr>
</table>

### Fieldset styling ###

Alternate ways to style fieldsets

<table class="reporttable">
	<tr>
		<th>Type</th>
		<th>Description</th>
		<th></th>
		<th>with .cnqr-first</th>
		<th>with .screen-reader-only</th>
		<th>with .screen-reader-only.cnqr-first</th>

	</tr>
	<tr>
		<td>Default</td>
		<td>no css class</td>
		<td style="vertical-align:top">
			<p>Example paragraph</p>
			<fieldset>
				<legend>Legend</legend>
				Content
			</fieldset>
		</td>
		<td style="vertical-align:top">
			<p>Example paragraph</p>
			<fieldset class="cnqr-first">
				<legend>Legend</legend>
				Content
			</fieldset>
		</td>
		<td style="vertical-align:top">
			<fieldset class="screen-reader-only">
				<legend>Legend</legend>
				Content
			</fieldset>
		</td>
		<td style="vertical-align:top">
			<fieldset class="cnqr-first screen-reader-only">
				<legend>Legend</legend>
				Content
			</fieldset>
		</td>
	</tr>
	<tr>
		<td>.cnqr-fieldset</td>
		<td>style like classic fieldset</td>
		<td style="vertical-align:top">
			<p>Example paragraph</p>
			<fieldset class="cnqr-fieldset">
				<legend>Legend</legend>
				Content
			</fieldset>
		</td>
		<td style="vertical-align:top">
			<p>Example paragraph</p>
			<fieldset class="cnqr-fieldset cnqr-first">
				<legend>Legend</legend>
				Content
			</fieldset>
		</td>
		<td style="vertical-align:top">
			<fieldset class="cnqr-fieldset screen-reader-only">
				<legend>Legend</legend>
				Content
			</fieldset>
		</td>
		<td style="vertical-align:top">
			<fieldset class="cnqr-fieldset cnqr-first screen-reader-only">
				<legend>Legend</legend>
				Content
			</fieldset>
		</td>
	</tr>
	<tr>
		<td>.cnqr-muted</td>
		<td>remove background color and borders</td>
		<td style="vertical-align:top">
			<p>Example paragraph</p>
			<fieldset class="cnqr-muted">
				<legend>Legend</legend>
				Content
			</fieldset>
		</td>
		<td style="vertical-align:top">
			<p>Example paragraph</p>
			<fieldset class="cnqr-muted cnqr-first">
				<legend>Legend</legend>
				Content
			</fieldset>
		</td>
		<td style="vertical-align:top">
			<fieldset class="cnqr-muted screen-reader-only">
				<legend>Legend</legend>
				Content
			</fieldset>
		</td>
		<td style="vertical-align:top">
			<fieldset class="cnqr-muted cnqr-first screen-reader-only">
				<legend>Legend</legend>
				Content
			</fieldset>
		</td>
	</tr>
</table>

### Checkbox and Radio Button Styling ###

Interacting (Clicking, selecting) labels causes the interaction to be sent to the associated input.
 Using this, we can make the label element "stand-in" for a hidden-from-view chekcbox and radio button, 
 and then use a css ":before" pseudo selector to content to style in front of the label.

This approach works pretty well, but it messes up tab key interact, so we add a bit of javascript to fix that.

If you are having issues, add leave the class "form-control" off of the checkboxes/radio buttons, and they will not be restyled.

---

<div class="row">
	<div class="col-md-6">
		<h4>This...</h4>
		<input type="checkbox" class="native-input" id="cb1"/>
		<label for="cb1">A checkbox</label>
	</div>
	<div class="col-md-6">
		<h4>...Turns into this by default.</h4>
		<input type="checkbox" class="form-control" id="cb2"/>
		<label for="cb2">A checkbox</label>
	</div>
</div>

---

<div class="row">
	<div class="col-md-6">
		<h4>This...</h4>
		<input type="radio" id="rb1"/>
		<label for="rb1">A radio button</label>
	</div>
	<div class="col-md-6">
		<h4>...Turns into this by default.</h4>
		<input type="radio" class="form-control" id="rb2"/>
		<label for="rb2">A radio button</label>
	</div>
</div>
