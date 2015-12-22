---
layout: reference
title: message box
---


## Types ##

<table class="reporttable">
	<tr>
		<th>confirm</th>
		<th>success</th>
		<th>info   </th>
		<th>warning</th>
		<th>error  </th>
	</tr>
	<tr>
		<td><input id="confirmMsgBox" type="button" value="Confirm" class="btn btn-default cnqr-muted"></td>
		<td><input id="successMsgBox" type="button" value="Success" class="btn btn-success"></td>
		<td><input id="infoMsgBox" type="button" value="Info" class="btn btn-info"></td>
		<td><input id="warningMsgBox" type="button" value="Warning" class="btn btn-warning"></td>
		<td><input id="errorMsgBox" type="button" value="Error" class="btn btn-danger"></td>
	</tr>
</table>

##Implmentation

### JQuery
<iframe src="messagebox-jquery.html" frameBorder="0"></iframe>

### PrototypeJS
<iframe src="messagebox-prototypejs.html" frameBorder="0"></iframe> 

### ExtJS
<iframe src="messagebox-extjs.html" frameBorder="0"></iframe>

<script>
	$.cnqr.ready(function () {
		$("#confirmMsgBox").on("click", function () {
			$.cnqr.messagebox.confirm({
				message: "Lorem ipsum dolor sit amet, consectetur adipiscing elit."
			});
		});

		$("#successMsgBox").on("click", function () {
			$.cnqr.messagebox.success({
				message: "Nullam sagittis tincidunt malesuada."
			});
		});

		$("#infoMsgBox").on("click", function () {
			$.cnqr.messagebox.info({
				message: "Phasellus tristique tristique blandit. Nullam pellentesque porttitor orci. Nunc eros turpis, ultrices ut consequat in, rhoncus vitae metus. Pellentesque sit amet rutrum augue, a placerat odio. Mauris blandit pharetra sapien, id placerat orci tempus eget. Aliquam interdum neque a metus molestie, ut rhoncus justo hendrerit. In aliquam porttitor mauris at luctus. In ullamcorper tristique hendrerit. "
			});
		});

		$("#warningMsgBox").on("click", function () {
			$.cnqr.messagebox.warning({
				message: "Nunc lobortis, nisi eget rhoncus pellentesque, eros mauris gravida nisi, a aliquet dolor odio quis nisi. Donec sed lectus eu diam malesuada placerat eget non ipsum. Ut auctor nisi ac nibh convallis dignissim. "
			});
		});

		$("#errorMsgBox").on("click", function () {
			$.cnqr.messagebox.error({
				message: "Aliquam vestibulum risus porta arcu egestas rhoncus. Nulla vehicula, elit eget porta ultricies,"
			});
		});
	});
</script>
