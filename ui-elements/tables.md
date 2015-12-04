---
layout: reference
title: tables
---

## Tables (Available in all themes)##

###.reporttable ###

Concur's workhorse data tables
<div class="row">
	<div class="col-xs-12 col-md-11 col-md-offset-1">
		<h4>.reporttable</h4>
		<p>This is the default table style we use thoughout Concur for tabular data</p>

		<table class="reporttable">
			<thead>
				<tr>
					<th>Heading1</th>
					<th class="asc"><a href="javascript:void(0)">Heading2</a></th>
					<th><a href="javascript:void(0)">Heading3</a></th>
					<th><a href="javascript:void(0)">Heading4</th>
					<th>Heading5</th>
				</tr>
			</thead>
			<tbody>
				<tr>
					<th class="tablerow">table heading inline row </th>
					<td>Content2</td>
					<td><a href="javascript:void(0)">Content3</a></td>
					<td>Content4</td>
					<td>Content5</td>
				</tr>
				<tr>
					<th class="tablerow">table heading inline row </th>
					<td>Content2</td>
					<td><a href="javascript:void(0)">Content3</a></td>
					<td>Content4</td>
					<td>Content5</td>
				</tr>
				<tr>
					<th class="tablerow">table heading inline row </th>
					<td>Content2</td>
					<td><a href="javascript:void(0)">Content3</a></td>
					<td>Content4</td>
					<td>Content5</td>
				</tr>
				<tr>
					<th class="tablerow">table heading inline row </th>
					<td>Content2</td>
					<td>Content3</td>
					<td>Content4</td>
					<td>
						<table>
							<tbody><tr>
								       <th>Unaffected Heading one</th>
								       <th>Unaffected Heading two</th>
							       </tr>
								<tr>
									<td>Unaffected content one</td>
									<td>Unaffected content two</td>
								</tr>
							</tbody></table>

					</td>
				</tr>
			</tbody>
		</table>
	</div>
</div>

### .reporttable's options ###

Tools to alter the appearance of .reporttable. Can be used in combination.

<div class="row">
	<div class="col-xs-12 col-md-11 col-md-offset-1">
		<h4>.reporttable .reporttable-airy</h4>
		<p>Makes .reporttable more finger friendly</p>
		<table class="reporttable reporttable-airy">
			<thead>
				<tr>
					<th>Heading1</th>
					<th><a href="javascript:void(0)">Heading3</a></th>
					<th><a href="javascript:void(0)">Heading4</a></th>
					<th><a href="javascript:void(0)">Heading5 <img border="0" align="absmiddle" alt="Sorted ascending" src="/images/SortUp.gif"></a></th>
					<th>Heading6</th>
				</tr>
			</thead>
			<tbody>
				<tr>
					<th class="tablerow">table heading inline row </th>
					<td>Content2</td>
					<td><a href="javascript:void(0)">Content3</a></td>
					<td>Content4</td>
					<td>Content5</td>
				</tr>
				<tr>
					<th class="tablerow">table heading inline row </th>
					<td>Content2</td>
					<td><a href="javascript:void(0)">Content3</a></td>
					<td>Content4</td>
					<td>Content5</td>
				</tr>
				<tr>
					<th class="tablerow">Content1</th>
					<td>Content2</td>
					<td>Content3</td>
					<td>Content4</td>
					<td>
						<table>
							<tbody><tr>
									   <th>Unaffected Heading one</th>
									   <th>Unaffected Heading two</th>
								   </tr>
								<tr>
									<td>Unaffected content one</td>
									<td>Unaffected content two</td>
								</tr>
							</tbody></table>
					</td>
				</tr>
			</tbody>
		</table>
	</div>
</div>


<div class="row">
	<div class="col-xs-12 col-md-11 col-md-offset-1">
		<h4>Zebra Striping (2 ways)</h4>
		<div class="row">
			<div class="col-xs-12 col-md-6">
		
				<p>Either adding the class ".alternaterow" to every other &lt;tr&gt;...</p>

				<table class="reporttable">
					<thead>
						<tr>
							<th>Heading1</th>
							<th class="desc"><a href="javascript:void(0)">Heading2</a></th>
							<th><a href="javascript:void(0)">Heading3</a></th>
							<th><a href="javascript:void(0)">Heading4</a></th>
							<th><a href="javascript:void(0)">Heading5</a></th>
						</tr>
					</thead>
					<tbody>
						<tr class="alternaterow">
							<th class="tablerow">table heading inline row </th>
							<td>Content2</td>
							<td>Content3</td>
							<td>Content4</td>
							<td>Content5</td>
						</tr>
						<tr>
							<th class="tablerow">table heading inline row </th>
							<td>Content2</td>
							<td>Content3</td>
							<td>Content4</td>
							<td>Content5</td>
						</tr>
						<tr class="alternaterow">
							<th class="tablerow">table heading inline row </th>
							<td>Content2</td>
							<td>Content3</td>
							<td>Content4</td>
							<td>Content5</td>
						</tr>
						<tr>
							<th class="tablerow">table heading inline row </th>
							<td>Content2</td>
							<td>Content3</td>
							<td>Content4</td>
							<td>
								<table>
									<tbody><tr>
											   <th>Unaffected Heading one</th>
											   <th>Unaffected Heading two</th>
										   </tr>
										<tr>
											<td>Unaffected content one</td>
											<td>Unaffected content two</td>
										</tr>
										<tr>
											<td>Unaffected content one</td>
											<td>Unaffected content two</td>
										</tr>
									</tbody></table>
							</td>
						</tr>
					</tbody>
				</table>
			</div>
			<div class="col-xs-12 col-md-6 cnqr-col-no-gutter-left">
				<p>...Or adding the class ".reporttable-striped" to to the table (N/A for IE8)</p>

				<table class="reporttable reporttable-striped">
					<thead>
					<tr>
						<th>Heading1</th>
						<th class="desc"><a href="javascript:void(0)">Heading2</a></th>
						<th><a href="javascript:void(0)">Heading3</a></th>
						<th><a href="javascript:void(0)">Heading4</a></th>
						<th><a href="javascript:void(0)">Heading5</a></th>
					</tr>
					</thead>
					<tbody>
						<tr>
							<th class="tablerow">table heading inline row </th>
							<td>Content2</td>
							<td>Content3</td>
							<td>Content4</td>
							<td>Content5</td>
						</tr>
						<tr>
							<th class="tablerow">table heading inline row </th>
							<td>Content2</td>
							<td>Content3</td>
							<td>Content4</td>
							<td>Content5</td>
						</tr>
						<tr>
							<th class="tablerow">table heading inline row </th>
							<td>Content2</td>
							<td>Content3</td>
							<td>Content4</td>
							<td>Content5</td>
						</tr>
						<tr>
							<th class="tablerow">table heading inline row </th>
							<td>Content2</td>
							<td>Content3</td>
							<td>Content4</td>
							<td>
								<table>
									<tbody><tr>
										<th>Unaffected Heading one</th>
										<th>Unaffected Heading two</th>
									</tr>
									<tr>
										<td>Unaffected content one</td>
										<td>Unaffected content two</td>
									</tr>
									<tr>
										<td>Unaffected content one</td>
										<td>Unaffected content two</td>
									</tr>
								</tbody></table>
							</td>
						</tr>
					</tbody>
				</table>
			</div>
		</div>
	</div>
</div>

<div class="row">
	<div class="col-xs-12 col-md-11 col-md-offset-1">
		<h4>Row States</h4>
		<p>add state classes .success, .warning, .danger or .info to table row, or table cell</p>
		<table class="reporttable">
			<thead>
				<tr>
					<th>Heading1</th>
					<th><a href="javascript:void(0)">Heading3</a></th>
					<th><a href="javascript:void(0)">Heading4</a></th>
					<th><a href="javascript:void(0)">Heading5 <img border="0" align="absmiddle" alt="Sorted ascending" src="/images/SortUp.gif"></a></th>
					<th>Heading6</th>
				</tr>
			</thead>
			<tbody>
				<tr class="active">
					<th class="tablerow">Active Row</th>
					<td>Content2</td>
					<td><a href="javascript:void(0)">Content3</a></td>
					<td>Content4</td>
					<td>Content5</td>
				</tr>
				<tr>
					<th class="tablerow">table heading inline row</th>
					<td class="active">Active Cell</td>
					<td><a href="javascript:void(0)">Content3</a></td>
					<td>Content4</td>
					<td>Content5</td>
				</tr>
				
				<tr class="success">
					<th class="tablerow">Success Row</th>
					<td>Content2</td>
					<td><a href="javascript:void(0)">Content3</a></td>
					<td>Content4</td>
					<td>Content5</td>
				</tr>
				<tr>
					<th class="tablerow">table heading inline row</th>
					<td class="success">Success Cell</td>
					<td><a href="javascript:void(0)">Content3</a></td>
					<td>Content4</td>
					<td>Content5</td>
				</tr>
				<tr class="warning">
					<th class="tablerow">Warning Row </th>
					<td >Content2</td>
					<td><a href="javascript:void(0)">Content3</a></td>
					<td>Content4</td>
					<td>Content5</td>
				</tr>
				<tr>
					<th class="tablerow">table heading inline row</th>
					<td class="warning">Warning Cell</td>
					<td><a href="javascript:void(0)">Content3</a></td>
					<td>Content4</td>
					<td>Content5</td>
				</tr>
				<tr class="danger">
					<th class="tablerow">Danger Row </th>
					<td>Content2</td>
					<td><a href="javascript:void(0)">Content3</a></td>
					<td>Content4</td>
					<td>Content5</td>
				</tr>
				<tr>
					<th class="tablerow">table heading inline row</th>
					<td class="danger">Danger Cell</td>
					<td><a href="javascript:void(0)">Content3</a></td>
					<td>Content4</td>
					<td>Content5</td>
				</tr>
				<tr class="info">
					<th class="tablerow">Info Row </th>
					<td>Content2</td>
					<td><a href="javascript:void(0)">Content3</a></td>
					<td>Content4</td>
					<td>Content5</td>
				</tr>
				<tr>
					<th class="tablerow">table heading inline row</th>
					<td class="info">Info Cell</td>
					<td><a href="javascript:void(0)">Content3</a></td>
					<td>Content4</td>
					<td>Content5</td>
				</tr>
			</tbody>
		</table>
	</div>
</div>

<div class="row">
	<div class="col-xs-12 col-md-11 col-md-offset-1">
		<h4>.reporttable .reporttable-nomoretable</h4>
		<p>Makes .reporttable collapsible on a fully responsive page.</p>
		<p>To work well, populate the "data-title" attribute for TD elements</p>
		<table class="reporttable reporttable-nomoretable">
			<thead>
				<tr>
					<th>Heading1</th>
					<th><a href="javascript:void(0)">Heading2</a></th>
					<th><a href="javascript:void(0)">Heading3</a></th>
					<th><a href="javascript:void(0)">Heading4 <img border="0" align="absmiddle" alt="Sorted ascending" src="/images/SortUp.gif"></a></th>
					<th>Heading5</th>
				</tr>
			</thead>
			<tbody>
				<tr>
					<th class="tablerow">table heading inline row </th>
					<td data-title="Heading2">Content2</td>
					<td data-title="Heading3"><a href="javascript:void(0)">Content3</a></td>
					<td data-title="Heading4">Content4</td>
					<td data-title="Heading5">Content5</td>
				</tr>
				<tr>
					<th class="tablerow">table heading inline row </th>
					<td data-title="Heading2">Content2</td>
					<td data-title="Heading3"><a href="javascript:void(0)">Content3</a></td>
					<td data-title="Heading4">Content4</td>
					<td data-title="Heading5">Content5</td>
				</tr>
				<tr>
					<th class="tablerow">Content1</th>
					<td data-title="Heading2">Content2</td>
					<td data-title="Heading3">Content3</td>
					<td data-title="Heading4">Content4</td>
					<td data-title="Heading5">
						<table>
							<tbody><tr>
									   <th>Unaffected Heading one</th>
									   <th>Unaffected Heading two</th>
								   </tr>
								<tr>
									<td>Unaffected content one</td>
									<td>Unaffected content two</td>
								</tr>
							</tbody></table>
					</td>
				</tr>
			</tbody>
		</table>
	</div>
</div>

<div class="row">
	<div class="col-xs-12 col-md-11 col-md-offset-1">
		<h4>.cnqr-last</h4>
		<p>remove bottom margin on .reporttable</p>
		<table class="reporttable cnqr-last">
			<thead>
				<tr>
					<th>Heading1</th>
					<th><a href="javascript:void(0)">Heading3</a></th>
					<th><a href="javascript:void(0)">Heading4</a></th>
					<th><a href="javascript:void(0)">Heading5 <img border="0" align="absmiddle" alt="Sorted ascending" src="/images/SortUp.gif"></a></th>
					<th>Heading6</th>
				</tr>
			</thead>
			<tbody>
				<tr>
					<th class="tablerow">table heading inline row </th>
					<td>Content2</td>
					<td><a href="javascript:void(0)">Content3</a></td>
					<td>Content4</td>
					<td>Content5</td>
				</tr>
				<tr>
					<th class="tablerow">table heading inline row </th>
					<td>Content2</td>
					<td><a href="javascript:void(0)">Content3</a></td>
					<td>Content4</td>
					<td>Content5</td>
				</tr>
				<tr>
					<th class="tablerow">Content1</th>
					<td>Content2</td>
					<td>Content3</td>
					<td>Content4</td>
					<td>
						<table>
							<tbody><tr>
								       <th>Unaffected Heading one</th>
								       <th>Unaffected Heading two</th>
							       </tr>
								<tr>
									<td>Unaffected content one</td>
									<td>Unaffected content two</td>
								</tr>
							</tbody></table>
					</td>
				</tr>
			</tbody>
		</table>
	</div>
</div>

###.presentationtable ###

**Designer:** This table type only meant for developers. Ignore.
**Developer:** Tables should be avoided when laying out non tabular content. 

But when it cannot be avoided, use .presentationtable, a general purpose table. Don't forget to add role="presentation"

Useful for input field layout.
<div class="row">
	<div class="col-xs-12 col-md-11 col-md-offset-1">
		<table role="presentation" class="presentationtable">
			<tbody>
				<tr>
					<td><label for="text1">label one</label></td>
					<td><label for="text2">label two</label></td>
				</tr>
				<tr>
					<td><input type="text" id="text1" value=""></td>
					<td><input type="text" id="text2" value=""></td>
					<td><input type="button" name="btnEdit" value="Edit"></td>
					<td><input type="button" name="btnAdmin" value="Administer"></td>
					<td><input type="button" name="btnBilling" value="Modify"></td>
				</tr>
			</tbody>
		</table>
	</div>
</div>

### .presentationtable's options ###
#### .cnqr-condensed ####

A tight table with no margin or padding

**Designer:** This table type only meant for developers. Ignore.

Useful for positioning where no space between elements is required.
<div class="row">
	<div class="col-xs-12 col-md-11 col-md-offset-1">
		<table class="presentationtable cnqr-condensed" role="presentation">
			<tbody>
				<tr>
					<td><img src="/images/CreditCardVS80.gif" alt=""/></td>
					<td><img src="/images/CreditCardMC80.gif" alt=""/></td>
					<td><img src="/images/CreditCardAE80.gif" alt=""/></td>
				</tr>
			</tbody>
		</table>
	</div>
</div>

#### .presentationtable-center ####

Horizontally center a presentationtable

**Designer:** This table type only meant for developers. Ignore.

Useful for positioning where no space between elements is required.
<div class="row">
	<div class="col-xs-12 col-md-11 col-md-offset-1">
		<table class="presentationtable presentationtable-center" role="presentation">
			<tbody>
				<tr>
					<td><img src="/images/CreditCardVS80.gif" alt=""/></td>
					<td><img src="/images/CreditCardMC80.gif" alt=""/></td>
					<td><img src="/images/CreditCardAE80.gif" alt=""/></td>
				</tr>
			</tbody>
		</table>
	</div>
</div>
