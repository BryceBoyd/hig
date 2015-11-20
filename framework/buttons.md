---
layout: reference
title: Buttons
requireCss: /static/less/cnqr-view/docs.less
---

## Gateway Style Buttons ##

### Overview ###
Not all buttons are equal. In the Concur ecosystem, there are "workhorse" buttons, and "Call to action" buttons. This page will explain how to correctly design using buttons, the different button sizes and variations, and implementation details and best practices. 

### Call To Action Buttons ###

<button class="btn btn-primary btn-lg" type="submit">Purchase Now!</button><br />

* Reserved only for the most important/primary actions (ex: Sign up now!, Submit Report, Book This Trip, etc.). 
* Not all pages require a CTA, 
* For most pages, only one CTA should appear on a given page. 
* Search result pages may have one CTA per result. This helps the user locate happy path.
* Button sizes are determined in the table below as V2 Base, V1 Small, V1 X-small.

### Workhorse Buttons ###

<button class="btn btn-default" type="submit">Workhorse</button><br />

* Used for all actions/interactions within a feature (ex: Browse, Next, Add, Edit). This includes Drop Down Buttons.  
* Button sizes are determined in the table below as V2 Base, V1 Small, V1 X-small. 

### Implementation ###
* *Boostrap Style:* In most cases, use the Bootstrap-style button.
* *JQuery Style:* In JQuery Widgets, use the JQuery-style button

### Types ###
<table class="reporttable">
	<tr>
		<th>CSS System</th>
		<th>Button Class</th>
		<th>Link</th>
		<th>Button</th>
		<th>Input</th>
		<th>Submit</th>
		<th>Button group</th>
		<th>Button&nbsp;split&nbsp;group&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</th>
	</tr>
	<tr>
		<td>None</td>
		<td>[unclassed]</td>
		<td><a role=button href="#">Link</a></td>
		<td><button type="submit">Button</button></td>
		<td><input type="button" value="Input"></td>
		<td><input  type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>

	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-default</td>
		<td><a class="btn btn-default" role=button href="#">Link</a></td>
		<td><button class="btn btn-default" type="submit">Button</button></td>
		<td><input class="btn btn-default" type="button" value="Input"></td>
		<td><input class="btn btn-default" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-default dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-default">Drop Down</button>
				<button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-default disabled</td>
		<td><a class="btn btn-default disabled" role=button href="#">Link</a></td>
		<td><button disabled class="btn btn-default" type="submit">Button</button></td>
		<td><input disabled class="btn btn-default" type="button" value="Input"></td>
		<td><input disabled class="btn btn-default" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-default disabled dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button disabled class="btn btn-default">Drop Down</button>
				<button disabled type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-default .cnqr-muted</td>
		<td><a class="btn btn-default cnqr-muted" role=button href="#">Link</a></td>
		<td><button class="btn btn-default cnqr-muted" type="submit">Button</button></td>
		<td><input class="btn btn-default cnqr-muted" type="button" value="Input"></td>
		<td><input class="btn btn-default cnqr-muted" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-default cnqr-muted dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-default cnqr-muted">Drop Down</button>
				<button type="button" class="btn btn-default cnqr-muted dropdown-toggle" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-default .cnqr-muted disabled</td>
		<td><a class="btn btn-default cnqr-muted disabled" role=button href="#">Link</a></td>
		<td><button disabled class="btn btn-default cnqr-muted" type="submit">Button</button></td>
		<td><input disabled class="btn btn-default cnqr-muted" type="button" value="Input"></td>
		<td><input disabled class="btn btn-default cnqr-muted" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button disabled data-toggle="dropdown" data-filter="whatToGet" class="btn btn-default cnqr-muted dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button disabled class="btn btn-default cnqr-muted">Drop Down</button>
				<button disabled type="button" class="btn btn-default cnqr-muted dropdown-toggle" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-corner-all</td>
		<td><a class="ui-button ui-corner-all" role=button href="#">Link</a></td>
		<td><button class="ui-button ui-corner-all" type="submit">Button</button></td>
		<td><input class="ui-button ui-corner-all" type="button" value="Input"></td>
		<td><input class="ui-button ui-corner-all" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-corner-all disabled</td>
		<td><a class="ui-button ui-corner-all disabled" role=button href="#">Link</a></td>
		<td><button disabled class="ui-button ui-corner-all" type="submit">Button</button></td>
		<td><input disabled class="ui-button ui-corner-all" type="button" value="Input"></td>
		<td><input disabled class="ui-button ui-corner-all" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-corner-all cnqr-muted</td>
		<td><a class="ui-button ui-corner-all cnqr-muted" role=button href="#">Link</a></td>
		<td><button class="ui-button ui-corner-all cnqr-muted" type="submit">Button</button></td>
		<td><input class="ui-button ui-corner-all cnqr-muted" type="button" value="Input"></td>
		<td><input class="ui-button ui-corner-all cnqr-muted" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-corner-all cnqr-muted disabled</td>
		<td><a class="ui-button ui-corner-all cnqr-muted disabled" role=button href="#">Link</a></td>
		<td><button disabled class="ui-button ui-corner-all cnqr-muted" type="submit">Button</button></td>
		<td><input disabled class="ui-button ui-corner-all cnqr-muted" type="button" value="Input"></td>
		<td><input disabled class="ui-button ui-corner-all cnqr-muted" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-primary</td>
		<td><a class="btn btn-primary" role=button href="#">Link</a></td>
		<td><button class="btn btn-primary" type="submit">Button</button></td>
		<td><input class="btn btn-primary" type="button" value="Input"></td>
		<td><input class="btn btn-primary" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-primary dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-primary">Drop Down</button>
				<button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-primary disabled</td>
		<td><a class="btn btn-primary disabled" role=button href="#">Link</a></td>
		<td><button disabled class="btn btn-primary" type="submit">Button</button></td>
		<td><input disabled class="btn btn-primary" type="button" value="Input"></td>
		<td><input disabled class="btn btn-primary" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-primary disabled dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-primary disabled">Drop Down</button>
				<button type="button" class="btn btn-primary dropdown-toggle disabled" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-primary .cnqr-muted</td>
		<td><a class="btn btn-primary cnqr-muted" role=button href="#">Link</a></td>
		<td><button class="btn btn-primary cnqr-muted" type="submit">Button</button></td>
		<td><input class="btn btn-primary cnqr-muted" type="button" value="Input"></td>
		<td><input class="btn btn-primary cnqr-muted" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-primary cnqr-muted dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-primary cnqr-muted">Drop Down</button>
				<button type="button" class="btn btn-primary cnqr-muted dropdown-toggle" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-primary .cnqr-muted disabled</td>
		<td><a class="btn btn-primary cnqr-muted disabled" role=button href="#">Link</a></td>
		<td><button disabled class="btn btn-primary cnqr-muted" type="submit">Button</button></td>
		<td><input disabled class="btn btn-primary cnqr-muted" type="button" value="Input"></td>
		<td><input disabled class="btn btn-primary cnqr-muted" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button disabled data-toggle="dropdown" data-filter="whatToGet" class="btn btn-primary cnqr-muted dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button disabled class="btn btn-primary cnqr-muted">Drop Down</button>
				<button disabled type="button" class="btn btn-primary cnqr-muted dropdown-toggle" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-primary .ui-corner-all</td>
		<td><a class="ui-button ui-button-primary ui-corner-all" role=button href="#">Link</a></td>
		<td><button class="ui-button ui-button-primary ui-corner-all" type="submit">Button</button></td>
		<td><input class="ui-button ui-button-primary ui-corner-all" type="button" value="Input"></td>
		<td><input class="ui-button ui-button-primary ui-corner-all" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-primary .ui-corner-all disabled</td>
		<td><a class="ui-button ui-button-primary ui-corner-all disabled" role=button href="#">Link</a></td>
		<td><button disabled class="ui-button ui-button-primary ui-corner-all" type="submit">Button</button></td>
		<td><input disabled class="ui-button ui-button-primary ui-corner-all" type="button" value="Input"></td>
		<td><input disabled class="ui-button ui-button-primary ui-corner-all" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-primary .ui-corner-all cnqr-muted</td>
		<td><a class="ui-button ui-button-primary ui-corner-all cnqr-muted" role=button href="#">Link</a></td>
		<td><button class="ui-button ui-button-primary ui-corner-all cnqr-muted" type="submit">Button</button></td>
		<td><input class="ui-button ui-button-primary ui-corner-all cnqr-muted" type="button" value="Input"></td>
		<td><input class="ui-button ui-button-primary ui-corner-all cnqr-muted" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-primary .ui-corner-all cnqr-muted disabled</td>
		<td><a class="ui-button ui-button-primary ui-corner-all cnqr-muted disabled" role=button href="#">Link</a></td>
		<td><button disabled class="ui-button ui-button-primary ui-corner-all cnqr-muted" type="submit">Button</button></td>
		<td><input disabled class="ui-button ui-button-primary ui-corner-all cnqr-muted" type="button" value="Input"></td>
		<td><input disabled class="ui-button ui-button-primary ui-corner-all cnqr-muted" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-success</td>
		<td><a class="btn btn-success" role=button href="#">Link</a></td>
		<td><button class="btn btn-success" type="submit">Button</button></td>
		<td><input class="btn btn-success" type="button" value="Input"></td>
		<td><input class="btn btn-success" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-success dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-success">Drop Down</button>
				<button type="button" class="btn btn-success dropdown-toggle" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-success disabled</td>
		<td><a class="btn btn-success disabled" role=button href="#">Link</a></td>
		<td><button disabled class="btn btn-success" type="submit">Button</button></td>
		<td><input disabled class="btn btn-success" type="button" value="Input"></td>
		<td><input disabled class="btn btn-success" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-success disabled dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-success disabled">Drop Down</button>
				<button type="button" class="btn btn-success disabled dropdown-toggle" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-success .cnqr-muted</td>
		<td><a class="btn btn-success cnqr-muted" role=button href="#">Link</a></td>
		<td><button class="btn btn-success cnqr-muted" type="submit">Button</button></td>
		<td><input class="btn btn-success cnqr-muted" type="button" value="Input"></td>
		<td><input class="btn btn-success cnqr-muted" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-success cnqr-muted dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-success cnqr-muted">Drop Down</button>
				<button type="button" class="btn btn-success cnqr-muted dropdown-toggle" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-success .cnqr-muted disabled</td>
		<td><a class="btn btn-success cnqr-muted disabled" role=button href="#">Link</a></td>
		<td><button disabled class="btn btn-success cnqr-muted" type="submit">Button</button></td>
		<td><input disabled class="btn btn-success cnqr-muted" type="button" value="Input"></td>
		<td><input disabled class="btn btn-success cnqr-muted" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button disabled data-toggle="dropdown" data-filter="whatToGet" class="btn btn-success cnqr-muted dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button disabled class="btn btn-success cnqr-muted">Drop Down</button>
				<button disabled type="button" class="btn btn-success cnqr-muted dropdown-toggle" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-success .ui-corner-all</td>
		<td><a class="ui-button ui-button-success ui-corner-all" role=button href="#">Link</a></td>
		<td><button class="ui-button ui-button-success ui-corner-all" type="submit">Button</button></td>
		<td><input class="ui-button ui-button-success ui-corner-all" type="button" value="Input"></td>
		<td><input class="ui-button ui-button-success ui-corner-all" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-success .ui-corner-all disabled</td>
		<td><a class="ui-button ui-button-success ui-corner-all disabled" role=button href="#">Link</a></td>
		<td><button disabled class="ui-button ui-button-success ui-corner-all" type="submit">Button</button></td>
		<td><input disabled class="ui-button ui-button-success ui-corner-all" type="button" value="Input"></td>
		<td><input disabled class="ui-button ui-button-success ui-corner-all" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-success .ui-corner-all cnqr-muted</td>
		<td><a class="ui-button ui-button-success ui-corner-all cnqr-muted" role=button href="#">Link</a></td>
		<td><button class="ui-button ui-button-success ui-corner-all cnqr-muted" type="submit">Button</button></td>
		<td><input class="ui-button ui-button-success ui-corner-all cnqr-muted" type="button" value="Input"></td>
		<td><input class="ui-button ui-button-success ui-corner-all cnqr-muted" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-success .ui-corner-all cnqr-muted disabled</td>
		<td><a class="ui-button ui-button-success ui-corner-all cnqr-muted disabled" role=button href="#">Link</a></td>
		<td><button disabled class="ui-button ui-button-success ui-corner-all cnqr-muted" type="submit">Button</button></td>
		<td><input disabled class="ui-button ui-button-success ui-corner-all cnqr-muted" type="button" value="Input"></td>
		<td><input disabled class="ui-button ui-button-success ui-corner-all cnqr-muted" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-info</td>
		<td><a class="btn btn-info" role=button href="#">Link</a></td>
		<td><button class="btn btn-info" type="submit">Button</button></td>
		<td><input class="btn btn-info" type="button" value="Input"></td>
		<td><input class="btn btn-info" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-info dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-info">Drop Down</button>
				<button type="button" class="btn btn-info dropdown-toggle" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-info disabled</td>
		<td><a class="btn btn-info disabled" role=button href="#">Link</a></td>
		<td><button disabled class="btn btn-info" type="submit">Button</button></td>
		<td><input disabled class="btn btn-info" type="button" value="Input"></td>
		<td><input disabled class="btn btn-info" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-info disabled dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-info disabled">Drop Down</button>
				<button type="button" class="btn btn-info dropdown-toggle disabled" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-info .cnqr-muted</td>
		<td><a class="btn btn-info cnqr-muted" role=button href="#">Link</a></td>
		<td><button class="btn btn-info cnqr-muted" type="submit">Button</button></td>
		<td><input class="btn btn-info cnqr-muted" type="button" value="Input"></td>
		<td><input class="btn btn-info cnqr-muted" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-info cnqr-muted dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-info cnqr-muted">Drop Down</button>
				<button type="button" class="btn btn-info dropdown-toggle cnqr-muted" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-info .cnqr-muted disabled</td>
		<td><a class="btn btn-info cnqr-muted disabled" role=button href="#">Link</a></td>
		<td><button disabled class="btn btn-info cnqr-muted" type="submit">Button</button></td>
		<td><input disabled class="btn btn-info cnqr-muted" type="button" value="Input"></td>
		<td><input disabled class="btn btn-info cnqr-muted" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button disabled data-toggle="dropdown" data-filter="whatToGet" class="btn btn-info cnqr-muted dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button disabled class="btn btn-info cnqr-muted">Drop Down</button>
				<button disabled type="button" class="btn btn-info dropdown-toggle cnqr-muted" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-info .ui-corner-all</td>
		<td><a class="ui-button ui-button-info ui-corner-all" role=button href="#">Link</a></td>
		<td><button class="ui-button ui-button-info ui-corner-all" type="submit">Button</button></td>
		<td><input class="ui-button ui-button-info ui-corner-all" type="button" value="Input"></td>
		<td><input class="ui-button ui-button-info ui-corner-all" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-info .ui-corner-all disabled</td>
		<td><a class="ui-button ui-button-info ui-corner-all disabled" role=button href="#">Link</a></td>
		<td><button disabled class="ui-button ui-button-info ui-corner-all" type="submit">Button</button></td>
		<td><input disabled class="ui-button ui-button-info ui-corner-all" type="button" value="Input"></td>
		<td><input disabled class="ui-button ui-button-info ui-corner-all" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-info .ui-corner-all cnqr-muted</td>
		<td><a class="ui-button ui-button-info ui-corner-all cnqr-muted" role=button href="#">Link</a></td>
		<td><button class="ui-button ui-button-info ui-corner-all cnqr-muted" type="submit">Button</button></td>
		<td><input class="ui-button ui-button-info ui-corner-all cnqr-muted" type="button" value="Input"></td>
		<td><input class="ui-button ui-button-info ui-corner-all cnqr-muted" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-info .ui-corner-all cnqr-muted disabled</td>
		<td><a class="ui-button ui-button-info ui-corner-all cnqr-muted disabled" role=button href="#">Link</a></td>
		<td><button disabled class="ui-button ui-button-info ui-corner-all cnqr-muted" type="submit">Button</button></td>
		<td><input disabled class="ui-button ui-button-info ui-corner-all cnqr-muted" type="button" value="Input"></td>
		<td><input disabled class="ui-button ui-button-info ui-corner-all cnqr-muted" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-warning</td>
		<td><a class="btn btn-warning" role=button href="#">Link</a></td>
		<td><button class="btn btn-warning" type="submit">Button</button></td>
		<td><input class="btn btn-warning" type="button" value="Input"></td>
		<td><input class="btn btn-warning" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-warning dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-warning">Drop Down</button>
				<button type="button" class="btn btn-warning dropdown-toggle" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-warning disabled</td>
		<td><a class="btn btn-warning disabled" role=button href="#">Link</a></td>
		<td><button disabled class="btn btn-warning" type="submit">Button</button></td>
		<td><input disabled class="btn btn-warning" type="button" value="Input"></td>
		<td><input disabled class="btn btn-warning" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-warning disabled dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-warning disabled">Drop Down</button>
				<button type="button" class="btn btn-warning dropdown-toggle disabled" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-warning .cnqr-muted</td>
		<td><a class="btn btn-warning cnqr-muted" role=button href="#">Link</a></td>
		<td><button class="btn btn-warning cnqr-muted" type="submit">Button</button></td>
		<td><input class="btn btn-warning cnqr-muted" type="button" value="Input"></td>
		<td><input class="btn btn-warning cnqr-muted" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-warning cnqr-muted dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-warning cnqr-muted">Drop Down</button>
				<button type="button" class="btn btn-warning dropdown-toggle cnqr-muted" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-warning .cnqr-muted disabled</td>
		<td><a class="btn btn-warning cnqr-muted disabled" role=button href="#">Link</a></td>
		<td><button disabled class="btn btn-warning cnqr-muted" type="submit">Button</button></td>
		<td><input disabled class="btn btn-warning cnqr-muted" type="button" value="Input"></td>
		<td><input disabled class="btn btn-warning cnqr-muted" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button disabled data-toggle="dropdown" data-filter="whatToGet" class="btn btn-warning cnqr-muted dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button disabled class="btn btn-warning cnqr-muted">Drop Down</button>
				<button disabled type="button" class="btn btn-warning dropdown-toggle cnqr-muted" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-warning .ui-corner-all</td>
		<td><a class="ui-button ui-button-warning ui-corner-all" role=button href="#">Link</a></td>
		<td><button class="ui-button ui-button-warning ui-corner-all" type="submit">Button</button></td>
		<td><input class="ui-button ui-button-warning ui-corner-all" type="button" value="Input"></td>
		<td><input class="ui-button ui-button-warning ui-corner-all" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-warning .ui-corner-all disabled</td>
		<td><a class="ui-button ui-button-warning ui-corner-all disabled" role=button href="#">Link</a></td>
		<td><button disabled class="ui-button ui-button-warning ui-corner-all" type="submit">Button</button></td>
		<td><input disabled class="ui-button ui-button-warning ui-corner-all" type="button" value="Input"></td>
		<td><input disabled class="ui-button ui-button-warning ui-corner-all" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-warning .ui-corner-all cnqr-muted</td>
		<td><a class="ui-button ui-button-warning ui-corner-all cnqr-muted" role=button href="#">Link</a></td>
		<td><button class="ui-button ui-button-warning ui-corner-all cnqr-muted" type="submit">Button</button></td>
		<td><input class="ui-button ui-button-warning ui-corner-all cnqr-muted" type="button" value="Input"></td>
		<td><input class="ui-button ui-button-warning ui-corner-all cnqr-muted" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-warning .ui-corner-all cnqr-muted disabled</td>
		<td><a class="ui-button ui-button-warning ui-corner-all cnqr-muted disabled" role=button href="#">Link</a></td>
		<td><button disabled class="ui-button ui-button-warning ui-corner-all cnqr-muted" type="submit">Button</button></td>
		<td><input disabled class="ui-button ui-button-warning ui-corner-all cnqr-muted" type="button" value="Input"></td>
		<td><input disabled class="ui-button ui-button-warning ui-corner-all cnqr-muted" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-danger</td>
		<td><a class="btn btn-danger" role=button href="#">Link</a></td>
		<td><button class="btn btn-danger" type="submit">Button</button></td>
		<td><input class="btn btn-danger" type="button" value="Input"></td>
		<td><input class="btn btn-danger" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-danger dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-danger">Drop Down</button>
				<button type="button" class="btn btn-danger dropdown-toggle" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-danger disabled</td>
		<td><a class="btn btn-danger disabled" role=button href="#">Link</a></td>
		<td><button disabled class="btn btn-danger" type="submit">Button</button></td>
		<td><input disabled class="btn btn-danger" type="button" value="Input"></td>
		<td><input disabled class="btn btn-danger" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-danger disabled dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-danger disabled">Drop Down</button>
				<button type="button" class="btn btn-danger dropdown-toggle disabled" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-danger .cnqr-muted</td>
		<td><a class="btn btn-danger cnqr-muted" role=button href="#">Link</a></td>
		<td><button class="btn btn-danger cnqr-muted" type="submit">Button</button></td>
		<td><input class="btn btn-danger cnqr-muted" type="button" value="Input"></td>
		<td><input class="btn btn-danger cnqr-muted" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-danger cnqr-muted dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-danger cnqr-muted">Drop Down</button>
				<button type="button" class="btn btn-danger dropdown-toggle cnqr-muted" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-danger .cnqr-muted disabled</td>
		<td><a class="btn btn-danger cnqr-muted disabled" role=button href="#">Link</a></td>
		<td><button disabled class="btn btn-danger cnqr-muted" type="submit">Button</button></td>
		<td><input disabled class="btn btn-danger cnqr-muted" type="button" value="Input"></td>
		<td><input disabled class="btn btn-danger cnqr-muted" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button disabled data-toggle="dropdown" data-filter="whatToGet" class="btn btn-danger cnqr-muted dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button disabled class="btn btn-danger cnqr-muted">Drop Down</button>
				<button disabled type="button" class="btn btn-danger dropdown-toggle cnqr-muted" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-danger .ui-corner-all</td>
		<td><a class="ui-button ui-button-danger ui-corner-all" role=button href="#">Link</a></td>
		<td><button class="ui-button ui-button-danger ui-corner-all" type="submit">Button</button></td>
		<td><input class="ui-button ui-button-danger ui-corner-all" type="button" value="Input"></td>
		<td><input class="ui-button ui-button-danger ui-corner-all" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-danger .ui-corner-all disabled</td>
		<td><a class="ui-button ui-button-danger ui-corner-all disabled" role=button href="#">Link</a></td>
		<td><button disabled class="ui-button ui-button-danger ui-corner-all" type="submit">Button</button></td>
		<td><input disabled class="ui-button ui-button-danger ui-corner-all" type="button" value="Input"></td>
		<td><input disabled class="ui-button ui-button-danger ui-corner-all" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-danger .ui-corner-all cnqr-muted</td>
		<td><a class="ui-button ui-button-danger ui-corner-all cnqr-muted" role=button href="#">Link</a></td>
		<td><button class="ui-button ui-button-danger ui-corner-all cnqr-muted" type="submit">Button</button></td>
		<td><input class="ui-button ui-button-danger ui-corner-all cnqr-muted" type="button" value="Input"></td>
		<td><input class="ui-button ui-button-danger ui-corner-all cnqr-muted" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-danger .ui-corner-all cnqr-muted disabled</td>
		<td><a class="ui-button ui-button-danger ui-corner-all cnqr-muted disabled" role=button href="#">Link</a></td>
		<td><button disabled class="ui-button ui-button-danger ui-corner-all cnqr-muted" type="submit">Button</button></td>
		<td><input disabled class="ui-button ui-button-danger ui-corner-all cnqr-muted" type="button" value="Input"></td>
		<td><input disabled class="ui-button ui-button-danger ui-corner-all cnqr-muted" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>





	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-neutral</td>
		<td><a class="btn btn-neutral" role=button href="#">Link</a></td>
		<td><button class="btn btn-neutral" type="submit">Button</button></td>
		<td><input class="btn btn-neutral" type="button" value="Input"></td>
		<td><input class="btn btn-neutral" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-neutral dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-neutral">Drop Down</button>
				<button type="button" class="btn btn-neutral dropdown-toggle" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-neutral disabled</td>
		<td><a class="btn btn-neutral disabled" role=button href="#">Link</a></td>
		<td><button disabled class="btn btn-neutral" type="submit">Button</button></td>
		<td><input disabled class="btn btn-neutral" type="button" value="Input"></td>
		<td><input disabled class="btn btn-neutral" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-neutral disabled dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-neutral disabled">Drop Down</button>
				<button type="button" class="btn btn-neutral dropdown-toggle disabled" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-neutral .cnqr-muted</td>
		<td><a class="btn btn-neutral cnqr-muted" role=button href="#">Link</a></td>
		<td><button class="btn btn-neutral cnqr-muted" type="submit">Button</button></td>
		<td><input class="btn btn-neutral cnqr-muted" type="button" value="Input"></td>
		<td><input class="btn btn-neutral cnqr-muted" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-neutral cnqr-muted dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-neutral cnqr-muted">Drop Down</button>
				<button type="button" class="btn btn-neutral dropdown-toggle cnqr-muted" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-neutral .cnqr-muted disabled</td>
		<td><a class="btn btn-neutral cnqr-muted disabled" role=button href="#">Link</a></td>
		<td><button disabled class="btn btn-neutral cnqr-muted" type="submit">Button</button></td>
		<td><input disabled class="btn btn-neutral cnqr-muted" type="button" value="Input"></td>
		<td><input disabled class="btn btn-neutral cnqr-muted" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button disabled data-toggle="dropdown" data-filter="whatToGet" class="btn btn-neutral cnqr-muted dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button disabled class="btn btn-neutral cnqr-muted">Drop Down</button>
				<button disabled type="button" class="btn btn-neutral dropdown-toggle cnqr-muted" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-neutral .ui-corner-all</td>
		<td><a class="ui-button ui-button-neutral ui-corner-all" role=button href="#">Link</a></td>
		<td><button class="ui-button ui-button-neutral ui-corner-all" type="submit">Button</button></td>
		<td><input class="ui-button ui-button-neutral ui-corner-all" type="button" value="Input"></td>
		<td><input class="ui-button ui-button-neutral ui-corner-all" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-neutral .ui-corner-all disabled</td>
		<td><a class="ui-button ui-button-neutral ui-corner-all disabled" role=button href="#">Link</a></td>
		<td><button disabled class="ui-button ui-button-neutral ui-corner-all" type="submit">Button</button></td>
		<td><input disabled class="ui-button ui-button-neutral ui-corner-all" type="button" value="Input"></td>
		<td><input disabled class="ui-button ui-button-neutral ui-corner-all" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-neutral .ui-corner-all cnqr-muted</td>
		<td><a class="ui-button ui-button-neutral ui-corner-all cnqr-muted" role=button href="#">Link</a></td>
		<td><button class="ui-button ui-button-neutral ui-corner-all cnqr-muted" type="submit">Button</button></td>
		<td><input class="ui-button ui-button-neutral ui-corner-all cnqr-muted" type="button" value="Input"></td>
		<td><input class="ui-button ui-button-neutral ui-corner-all cnqr-muted" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-neutral .ui-corner-all cnqr-muted disabled</td>
		<td><a class="ui-button ui-button-neutral ui-corner-all cnqr-muted disabled" role=button href="#">Link</a></td>
		<td><button disabled class="ui-button ui-button-neutral ui-corner-all cnqr-muted" type="submit">Button</button></td>
		<td><input disabled class="ui-button ui-button-neutral ui-corner-all cnqr-muted" type="button" value="Input"></td>
		<td><input disabled class="ui-button ui-button-neutral ui-corner-all cnqr-muted" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>










	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-link</td>
		<td><a class="btn btn-link" role=button href="#">Link</a></td>
		<td><button class="btn btn-link" type="submit">Button</button></td>
		<td><input class="btn btn-link" type="button" value="Input"></td>
		<td><input class="btn btn-link" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-link dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-link disabled</td>
		<td><a class="btn btn-link disabled" role=button href="#">Link</a></td>
		<td><button disabled class="btn btn-link" type="submit">Button</button></td>
		<td><input disabled class="btn btn-link" type="button" value="Input"></td>
		<td><input disabled class="btn btn-link" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-link disabled dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-link .cnqr-muted</td>
		<td><a class="btn btn-link cnqr-muted" role=button href="#">Link</a></td>
		<td><button class="btn btn-link cnqr-muted" type="submit">Button</button></td>
		<td><input class="btn btn-link cnqr-muted" type="button" value="Input"></td>
		<td><input class="btn btn-link cnqr-muted" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-link cnqr-muted dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn .btn-link .cnqr-muted disabled</td>
		<td><a class="btn btn-link cnqr-muted disabled" role=button href="#">Link</a></td>
		<td><button disabled class="btn btn-link cnqr-muted" type="submit">Button</button></td>
		<td><input disabled class="btn btn-link cnqr-muted" type="button" value="Input"></td>
		<td><input disabled class="btn btn-link cnqr-muted" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button disabled data-toggle="dropdown" data-filter="whatToGet" class="btn btn-link cnqr-muted dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-link .ui-corner-all</td>
		<td><a class="ui-button ui-button-link ui-corner-all" role=button href="#">Link</a></td>
		<td><button class="ui-button ui-button-link ui-corner-all" type="submit">Button</button></td>
		<td><input class="ui-button ui-button-link ui-corner-all" type="button" value="Input"></td>
		<td><input class="ui-button ui-button-link ui-corner-all" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-link .ui-corner-all disabled</td>
		<td><a class="ui-button ui-button-link ui-corner-all disabled" role=button href="#">Link</a></td>
		<td><button disabled class="ui-button ui-button-link ui-corner-all" type="submit">Button</button></td>
		<td><input disabled class="ui-button ui-button-link ui-corner-all" type="button" value="Input"></td>
		<td><input disabled class="ui-button ui-button-link ui-corner-all" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-link .ui-corner-all cnqr-muted</td>
		<td><a class="ui-button ui-button-link ui-corner-all cnqr-muted" role=button href="#">Link</a></td>
		<td><button class="ui-button ui-button-link ui-corner-all cnqr-muted" type="submit">Button</button></td>
		<td><input class="ui-button ui-button-link ui-corner-all cnqr-muted" type="button" value="Input"></td>
		<td><input class="ui-button ui-button-link ui-corner-all cnqr-muted" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button .ui-button-link .ui-corner-all cnqr-muted disabled</td>
		<td><a class="ui-button ui-button-link ui-corner-all cnqr-muted disabled" role=button href="#">Link</a></td>
		<td><button disabled class="ui-button ui-button-link ui-corner-all cnqr-muted" type="submit">Button</button></td>
		<td><input disabled class="ui-button ui-button-link ui-corner-all cnqr-muted" type="button" value="Input"></td>
		<td><input disabled class="ui-button ui-button-link ui-corner-all cnqr-muted" type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
	</tr>
</table>

<h3>Boostrap Sizes</h3>
<p>Class "btn" required when sizing buttons (large or small). It is optional for default button size</p>
<table class="reporttable">
	<tr>
		<th>CSS System</th>
		<th>Button Class</th>
		<th>Link</th>
		<th>Button</th>
		<th>Input</th>
		<th>Submit</th>
		<th>Button group</th>
		<th>Button&nbsp;split&nbsp;group&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</th>
		<th>Compare</th>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn.btn-lg</td>
		<td><a class="btn btn-default btn-lg" role=button href="#">Link</a></td>
		<td><button class="btn btn-default btn-lg" type="submit">Button</button></td>
		<td><input class="btn btn-default btn-lg" type="button" value="Input"></td>
		<td><input class="btn btn-default btn-lg" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-default btn-lg dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-default btn-lg">Drop Down</button>
				<button type="button" class="btn btn-default btn-lg dropdown-toggle" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td><input type="text" class="form-control input-lg" style="width:125px"></td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn</td>
		<td><a class="btn btn-default" role=button href="#">Link</a></td>
		<td><button class="btn btn-default" type="submit">Button</button></td>
		<td><input class="btn btn-default" type="button" value="Input"></td>
		<td><input class="btn btn-default" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-default dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-default">Drop Down</button>
				<button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td><input type="text" class="form-control"></td>
	</tr>
	<tr>
		<td>None</td>
		<td>[unclassed]</td>
		<td><a class="" role=button href="#">Link</a></td>
		<td><button type="submit">Button</button></td>
		<td><input type="button" value="Input"></td>
		<td><input type="submit" value="Submit"></td>
		<td>N/A</td>
		<td>N/A</td>
		<td><input type="text"></td>
	</tr>
	<tr>
		<td>Bootstrap</td>
		<td>.btn.btn-sm</td>
		<td><a class="btn btn-default btn-sm" role=button href="#">Link</a></td>
		<td><button class="btn btn-default btn-sm" type="submit">Button</button></td>
		<td><input class="btn btn-default btn-sm" type="button" value="Input"></td>
		<td><input class="btn btn-default btn-sm" type="submit" value="Submit"></td>
		<td>
			<div class="btn-group">
				<button data-toggle="dropdown" data-filter="whatToGet" class="btn btn-default btn-sm dropdown-toggle">Drop Down <span class="caret"></span></button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td>
			<div class="btn-group">
				<button class="btn btn-default btn-sm">Drop Down</button>
				<button type="button" class="btn btn-default btn-sm dropdown-toggle" data-toggle="dropdown">
					<span class="caret"></span>
				</button>
				<ul class="dropdown-menu">
					<li data-value="1" data-selected-item="true" ><a role=button href="#">Option 1</a></li>
					<li data-value="2"><a role=button href="#">Option 2</a></li>
					<li data-value="3"><a role=button href="#">Option 3</a></li>
				</ul>
			</div>
		</td>
		<td><input type="text" class="form-control input-sm"></td>
	</tr>
</table>

<h3>JQueryUI Sizes</h3>
<table class="reporttable">
	<tr>
		<th>CSS System</th>
		<th>Button Class</th>
		<th>Link</th>
		<th>Button</th>
		<th>Input</th>
		<th>Submit</th>
		<th>Compare</th>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button.ui-btn-large</td>
		<td><a class="ui-button ui-btn-large" role=button href="#">Link</a></td>
		<td><button class="ui-button ui-btn-large" type="submit">Button</button></td>
		<td><input class="ui-button ui-btn-large" type="button" value="Input"></td>
		<td><input class="ui-button ui-btn-large" type="submit" value="Submit"></td>
		<td><input type="text" class="form-control input-lg"></td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button</td>
		<td><a class="ui-button" role=button href="#">Link</a></td>
		<td><button class="ui-button" type="submit">Button</button></td>
		<td><input class="ui-button" type="button" value="Input"></td>
		<td><input class="ui-button" type="submit" value="Submit"></td>
		<td><input type="text" class="form-control"></td>
	</tr>
	<tr>
		<td>None</td>
		<td>[unclassed]</td>
		<td><a class="" role=button href="#">Link</a></td>
		<td><button type="submit">Button</button></td>
		<td><input type="button" value="Input"></td>
		<td><input type="submit" value="Submit"></td>
		<td><input type="text"></td>
	</tr>
	<tr>
		<td>JQueryUI</td>
		<td>.ui-button.ui-btn-small</td>
		<td><a class="ui-button ui-btn-small" role=button href="#">Link</a></td>
		<td><button class="ui-button ui-btn-small" type="submit">Button</button></td>
		<td><input class="ui-button ui-btn-small" type="button" value="Input"></td>
		<td><input class="ui-button ui-btn-small" type="submit" value="Submit"></td>
		<td><input type="text" class="form-control input-sm"></td>
	</tr>
</table>
