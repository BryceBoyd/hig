---
layout: reference
title: helper classes
---

## Helper Classes (Available In All Themes) ##

### Quick Floats ###

* **.pull-right -** float right.
* **.pull-left -** float left.

### Show/Hide ###

* **.cnqr-hide -** hide content (using display:none)
* **.cnqr-show -** show content (using display:block)
* **.cnqr-show-inline-block -** show content (using display:inline-block) *rarely needed*

### Alignment ###

* **text-left** Left aligned text.
* **text-center** Center aligned text.
* **text-right** Right aligned text.
* **text-justify** Justified text.
* **text-nowrap** No wrap text.
* **center-block** Align a block center

### Cursors ###

* **.cnqr-cursor-pointer -** set cursor to pointer (using cursor:pointer)
* **.cnqr-cursor-default -** set cursor to pointer (using cursor:default)
* **.cnqr-cursor-help -** set cursor to help (using cursor:default)

### Misc. ###

* **.cnqr-full-width -** set width to 100% (using width:100%)

### Open definition Gateway Helper Classes ###

There are no global styles associated with these.

* **.cnqr-first -** Generally used to strip or lessen padding and/or margins, due to the fact the element is the first of its type
* **.cnqr-last -** Generally used to strip or lessen padding and/or margins, due to the fact the element is the last of its type
* **.cnqr-condensed -** Generally used to strip or lessen padding and/or margins.
* **.cnqr-expanded -** Generally used to increase padding and/or margins.
* **.cnqr-inner -** Generally used to provide a wrapping container, such as for padding, or for DOM manipulation
* **.cnqr-outer -** Used in conjunction with .inner, when 2 layers of wrapping (vertically centering, for example) or DOM manipulation
* **.cnqr-scrollable -** Generally used when making an area scrollable.

### Gateway Tiles ###

There are no global styles associated with these.

Bootstrap row/spanX elements are not designed to be re-flowable elements. If you have collections of elements that is of an indeterminate amount, and might need to reflow, then a different system is needed.

Bootstrap provides one. It's called "thumbnails", but it is rudimentary.

We have expanded bootstrap thumbnails and developed "tiles". Currently there are 4 types of tiles (and there were likely be lots more). 
These are defined in \cnqr-custom\less\_tiles.less file.

1. **.cnqr-tiles** generic tiles, based on Bootstrap thumbnails
2. **.cnqr-.data-input** tiles that contain form input elements, like for expense header here
3. **.cnqr-tiles.chicklet** rounded corner tiles for document containers (e.g. expense reports)
4. **.cnqr-tiles.thumb** tiles for thumbnail images
5. **.cnqr-tiles.task** tiles seen in the dashboard

### Partially Defined Gateway Helper Classes ###

A few examples of some of the variations of these are below

* **.cnqr-muted -** Generally used to de-emphasize
* **.cnqr-create -** For creation or new actions

### .cnqr-muted ###

Generally used to de-emphasize

<table class="reporttable">
	<tr>
		<th>Element</th>
		<th>Original Element</th>
		<th>Element with .cnqr-muted</th>
	</tr>
	<tr>
		<td>button</td>
		<td><button class="btn btn-default" type="submit">Button</button></td>
		<td><button class="btn btn-default cnqr-muted" type="submit">Button</button></td>
	</tr>
	<tr>
		<td>button toolbar</td>
		<td>
			<div class="btn-toolbar">
				<button class="btn btn-default" type="submit">Button 1</button>
				<button class="btn btn-default" type="submit">Button 2</button>
			</div>
		</td>
		<td>
			<div class="btn-toolbar cnqr-muted">
				<button class="btn btn-default" type="submit">Button 1</button>
				<button class="btn btn-default" type="submit">Button 2</button>
			</div>
		</td>
	</tr>
	<tr>
		<td>fieldset</td>
		<td>
			<fieldset>
				<legend>legend</legend>
				Some text
			</fieldset>
		</td>
		<td>
			<fieldset class="cnqr-muted">
				<legend>legend</legend>
				Some text
			</fieldset>
		</td>
	</tr>
</table>

### .cnqr-create ###

For creation or new actions

<table class="reporttable" role="grid">
	<tr>
		<th>Element</th>
		<th>Original Element</th>
		<th>Element with .cnqr-create</th>
	</tr>
	<tr>
		<td>Link</td>
		<td><a role=button href="#">Link</a></td>
		<td><a role=button href="#" class="cnqr-create">Link</a></td>
	</tr>
	<tr>
		<td>button</td>
		<td><button class="btn btn-primary cnqr-muted" type="submit">Button</button></td>
		<td><button class="btn btn-primary cnqr-muted cnqr-create" type="submit">Button</button></td>
	</tr>
	<tr>
		<td>tiles</td>
		<td>
			<ul class="cnqr-tiles chicklet">
				<li style="width:200px">
					<a class="cnqr-outer" role=button href="#"><div class="status not_submitted">Unsubmitted</div><div class="cnqr-inner">text</div></a>
				</li>
			</ul>
		</td>
		<td>
			<ul class="cnqr-tiles chicklet">
				<li class="cnqr-create" style="width:200px">
					<div class="cnqr-outer">
						<a class="cnqr-inner" role=button href="#"><div class="cnqr-inner"><div class="icon-plus-2" aria-hidden="true"></div>Create a new report </div></a>
					</div>
				</li>
			</ul>
		</td>
	</tr>
	<tr>
		<td>table rows</td>
		<td>
			<table class="reporttable">
				<tr>
					<th>column 1</th>
					<th>column 2</th>
				</tr>
				<tr>
					<td>text</td>
					<td>text</td>
				</tr>
				<tr>
					<td>text</td>
					<td>text</td>
				</tr>
			</table>
		</td>
		<td>
			<table class="reporttable">
				<tr>
					<th>column 1</th>
					<th>column 2</th>
				</tr>
				<tr class="cnqr-create">
					<td colspan="2">
						<div class="cnqr-inner">
							<span class="icon-plus-2" aria-hidden="true"></span>
							<span class="">Create a new expense</span>
						</div>
					</td>
				</tr>
				<tr>
					<td>text</td>
					<td>text</td>
				</tr>
			</table>
		</td>
	</tr>
	<tr>
		<td>H1</td>
		<td>
			<h1>Hello world</h1>
		</td>
		<td>
			<h1><span class="cnqr-create">Hello world</span></h1>
		</td>
	</tr>
</table>
