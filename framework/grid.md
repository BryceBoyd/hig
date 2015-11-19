---
layout: reference
title: grid
requireCss: /static/less/cnqr-view/docs.less
---

## Grid  (Available In All Themes - Must Be Enabled On Page) ##

### Bootstrap Grid ###

Grid systems are used for creating page layouts through a series of rows and columns that house your content. Here's how the Bootstrap grid system works:

* Use rows to create horizontal groups of columns.
* Predefined grid classes like .row and .col-xs-4 are available for quickly making grid layouts.
* Columns create gutters (gaps between column content) via padding.
* Grid columns are created by specifying the number of twelve available columns you wish to span. For example, three equal columns would use three .col-xs-4.

For most pages in concur, you would will use the layouthelper, which uses Layout.cshtml. This template will render the header, footer and a wrapping container (with class .container) for your content

All that is left for you to define on your page is a set of grid column containers.

Because each of our columns live inside a "container" element, they will take on different widths depending on overall viewport widths.

### Concur Grid ###

Bootstrap grids are designed to simplify layout, but are not enabled on non gateway themed pages (like Bluesky) by default.
	
To Enable Bootstrap on a classic asp page:

* Set page = new PageTemplate
* page.UseBootstrapLayout = true
* (see demo.asp for an example)

To Enable Bootstrap on a MVC .NET page:

* var layout = LayoutHelper.Current;
* layout.UseBootstrapLayout = true;
* (see CompanyAdmin/CompanyLocation/index.cshtml for an example)

<table>
	<tr>
		<th>Theme</th>
		<th>Gateway</th>
		<th>Bluesky (with boostrap)</th>
		<th>Bluesky (without boostrap)</th>
	</tr>
	<tr>
		<th>Grid Framework</th>
		<td>Bootstrap</td>
		<td>Bootstrap (content area only)</td>
		<td>N/A</td>
	</tr>
	<tr>
		<th>Simplified Page Layout</th>
		<td>
			<table border="1">
				<tr>
					<td><strong>"Header"</strong><br/>.cnqr-app-header<br/>(a Boostrap grid aware container)</td>
				</tr>
				<tr>
					<td style="background-color:mediumturquoise"><strong>"Content"</strong><br/>.cnqr-app-content<br/>(a Bootstrap row container)</td>
				</tr>
				<tr>
					<td><strong>"Footer"</strong><br/>.cnqr-app-footer<br/>(a Boostrap grid aware container)</td>
				</tr>
			</table>
		</td>
		<td>
			<table border="1">
				<tr>
					<td><strong>"Header"</strong><br/>(multiple containers)<br/>&nbsp;</td>
				</tr>
				<tr>
					<td style="background-color:mediumturquoise"><strong>"Content"</strong><br/>.cnqr-app-content<br/>(a Bootstrap row container)</td>
				</tr>
				<tr>
					<td><strong>"Footer"</strong><br/>N/A<br/>&nbsp;</td>
				</tr>
			</table>
		</td>
		<td>
			<table border="1">
				<tr>
					<td><strong>"Header"</strong><br/>(multiple containers)<br/>&nbsp;</td>
				</tr>
				<tr>
					<td><strong>"Content"</strong><br/>(multiple containers)<br/>&nbsp;</td>
				</tr>
				<tr>
					<td><strong>"Footer"</strong><br/>N/A<br/>&nbsp;</td>
				</tr>
			</table>
		</td>
	</tr>
</table>


### Layout ###

Using bootstrap or not, most pages are set up so that the content area has 2 main containers

* **#sidebar1** a optional container typically seen on the left side
* **#featured** a required container

When using bootstrap (UseBootstrapLayout), the 2 main content areas appear inside .cnqr-app-content

<table border="1">
	<tr>
		<td style="background-color:mediumturquoise">.cnqr-app-content<br/>(a Bootstrap row container)
		<table border="1" style="background-color:white">
			<tr>
				<td><strong>#Sidebar1 (optional)</strong><br/>(bootstrap column classes)<br/>(a Bootstrap column container)</td>
				<td><strong>#Featured</strong><br/>(bootstrap column classes)<br/>(a Bootstrap column container)</td>
			</tr>
		</table>
		</td>
	</tr>
</table>

When using bootstrap (UseBootstrapLayout) there are a couple of predefined enums that can be used to define the relationship between the width of the sidebar and the width of the featured area

* **leftColumnSize: Small** Smaller sidebar1 width (% based on viewport size)
* **leftColumnSize: Medium** Larger sidebar1 width (% based on viewport size)
* **leftColumnSize: Large** Set the sidebar1 width and the feature with to be equal.

### Layout Options ###

#### Concur grid control ####

These classes need to applied to the body tag. Unless they they directly conflict (cnqr-grid-sidebar-fixed-wide/cnqr-grid-sidebar-fixed-narrow), multiple classes can be used together.

* **.cnqr-grid-wide** to shut off responsive design and make the content fill the whole viewport. Note that these pages will generate a scrollbar if width drops below 1200px
* **.cnqr-grid-centered** this class has no effect in gateway, but in bluesky it centers the content. See demo.asp in bluesky for an example
* **.cnqr-grid-sidebar-fixed-wide** this fixes the width of the sidebar1 column to 330px in Gateway. This is currently only used on home.asp, a gateway only page.
* **.cnqr-grid-sidebar-fixed-narrow** this fixes the width of the sidebar1 column to 184px in gateway, 180px in bluesky (to match the existing width seen on non usebootstrap page). (see CompanyAdmin/CompanyLocation/index.cshtml for an example)

#### Concur column control ####

These classes need to be applied to a col-xx-xx container

* **.cnqr-col-no-gutter** remove column padding, both sides.
* **.cnqr-col-no-gutter-right** remove column padding, right side.
* **.cnqr-col-no-gutter-left** remove column padding, right side.

#### Responsive Design ####

Out of the box, Bootstrap provides 4 *breakpoints* - (Large, medium, small, extra small) that scales the grid system used to layout the page depending on viewport sizes. Read more here: http://getbootstrap.com/css/#grid 

By default for all of Concur CTE we have disabled the bottom 2 breakpoints (small and extra small), leaving only the large amd medium breakpoints.

To enable fully responsive (all 4 Bootstrap breakpoints) for a page in:

* **classic asp:** page.UseBootstrapFullyResponsive = true
* **MVC .NET**  layout.UseBootstrapFullyResponsive = true

Separately, you will want to set up any reporttables with the modifier class "reporttable-nomoretables".
