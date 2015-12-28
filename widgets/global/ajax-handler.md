---
layout: reference
title: Global - Ajax Handler
---

We have added few options to the $.ajax method to facilitate showing the processing messages, forms validation and error handling.

<h3>Options</h3>
							
		<div id="ajaxhandler-processmsg" class="cnqr-option cnqr-outer">
		<div class="cnqr-option-header col-md-12">
			<div class="col-md-5 cnqr-option-name"><strong>processMsg</strong></div>
			<div class="col-md-4 cnqr-option-default"><strong>Default: </strong>false</div>
			<div class="col-md-3 cnqr-option-type"><span class="pull-right"><strong>Type: </strong>Boolean Or String</span></div>
		</div>
		<div class="cnqr-inner col-md-12">
			<div class="cnqr-option-content">
				<p>Show processing open message on Ajax start, and close it on Ajax Complete.</p>
				<ul>
					<li>
						<span> <strong>Boolean</strong>: If set to true, the shown processing open message on Ajax start is equivalent to $.cnqr.processing.open().The close method $.cnqr.processing.close(), is called on Ajax Complete.</span>
						<div><div class="syntaxhighlighter  js" id="highlighter_187182"><table cellspacing="0" cellpadding="0" border="0"><tbody><tr><td class="gutter"><div class="line number1 index0 alt2">1</div><div class="line number2 index1 alt1">2</div><div class="line number3 index2 alt2">3</div><div class="line number4 index3 alt1">4</div><div class="line number5 index4 alt2">5</div><div class="line number6 index5 alt1">6</div><div class="line number7 index6 alt2">7</div></td><td class="code"><div class="container"><div class="line number1 index0 alt2"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</code>&nbsp;</div><div class="line number2 index1 alt1"><code class="js plain">$.ajax({</code></div><div class="line number3 index2 alt2"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;</code><code class="js plain">...,</code></div><div class="line number4 index3 alt1"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;</code><code class="js plain">processMsg: </code><code class="js keyword">true</code><code class="js plain">,</code></div><div class="line number5 index4 alt2"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;</code><code class="js plain">...,</code></div><div class="line number6 index5 alt1"><code class="js plain">});</code></div><div class="line number7 index6 alt2"><code class="js spaces">&nbsp;&nbsp;&nbsp;</code>&nbsp;</div></div></td></tr></tbody></table></div></div>
					</li>
					<li>
						<span> <strong>String</strong>: A custom string to show in the processing box.</span>
						<div><div class="syntaxhighlighter  js" id="highlighter_324841"><table cellspacing="0" cellpadding="0" border="0"><tbody><tr><td class="gutter"><div class="line number1 index0 alt2">1</div><div class="line number2 index1 alt1">2</div><div class="line number3 index2 alt2">3</div><div class="line number4 index3 alt1">4</div><div class="line number5 index4 alt2">5</div><div class="line number6 index5 alt1">6</div><div class="line number7 index6 alt2">7</div></td><td class="code"><div class="container"><div class="line number1 index0 alt2"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</code>&nbsp;</div><div class="line number2 index1 alt1"><code class="js plain">$.ajax({</code></div><div class="line number3 index2 alt2"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;</code><code class="js plain">...,</code></div><div class="line number4 index3 alt1"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;</code><code class="js plain">processMsg: </code><code class="js string">"My custom processing message"</code><code class="js plain">,</code></div><div class="line number5 index4 alt2"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;</code><code class="js plain">...,</code></div><div class="line number6 index5 alt1"><code class="js plain">});</code></div><div class="line number7 index6 alt2"><code class="js spaces">&nbsp;&nbsp;&nbsp;</code>&nbsp;</div></div></td></tr></tbody></table></div></div>
					</li>
					
				</ul>
			</div>
		</div>
	</div>


		<div id="ajaxhandler-errormsg" class="cnqr-option cnqr-outer">
		<div class="cnqr-option-header col-md-12">
			<div class="col-md-5 cnqr-option-name"><strong>errorMsg</strong></div>
			<div class="col-md-4 cnqr-option-default"><strong>Default: </strong>true</div>
			<div class="col-md-3 cnqr-option-type"><span class="pull-right"><strong>Type: </strong>Boolean Or String</span></div>
		</div>
		<div class="cnqr-inner col-md-12">
			<div class="cnqr-option-content">
				<p>Show a generic error message when the ajax call fails.</p>
				<ul>
					<li>
						<span> <strong>Boolean</strong>: If set to true, the shown error is a generic error. This is equivalent to $.cnqr.messegebox.error();</span>
						<div><div class="syntaxhighlighter  js" id="highlighter_119225"><table cellspacing="0" cellpadding="0" border="0"><tbody><tr><td class="gutter"><div class="line number1 index0 alt2">1</div><div class="line number2 index1 alt1">2</div><div class="line number3 index2 alt2">3</div><div class="line number4 index3 alt1">4</div><div class="line number5 index4 alt2">5</div><div class="line number6 index5 alt1">6</div><div class="line number7 index6 alt2">7</div></td><td class="code"><div class="container"><div class="line number1 index0 alt2"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</code>&nbsp;</div><div class="line number2 index1 alt1"><code class="js plain">$.ajax({</code></div><div class="line number3 index2 alt2"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;</code><code class="js plain">...,</code></div><div class="line number4 index3 alt1"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;</code><code class="js plain">errorMsg: </code><code class="js keyword">true</code><code class="js plain">,</code></div><div class="line number5 index4 alt2"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;</code><code class="js plain">...,</code></div><div class="line number6 index5 alt1"><code class="js plain">});</code></div><div class="line number7 index6 alt2"><code class="js spaces">&nbsp;&nbsp;&nbsp;</code>&nbsp;</div></div></td></tr></tbody></table></div></div>
					</li>
					<li>
						<span> <strong>String</strong>: A custom string to show in the error message box.</span>
						<div><div class="syntaxhighlighter  js" id="highlighter_738994"><table cellspacing="0" cellpadding="0" border="0"><tbody><tr><td class="gutter"><div class="line number1 index0 alt2">1</div><div class="line number2 index1 alt1">2</div><div class="line number3 index2 alt2">3</div><div class="line number4 index3 alt1">4</div><div class="line number5 index4 alt2">5</div><div class="line number6 index5 alt1">6</div><div class="line number7 index6 alt2">7</div></td><td class="code"><div class="container"><div class="line number1 index0 alt2"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</code>&nbsp;</div><div class="line number2 index1 alt1"><code class="js plain">$.ajax({</code></div><div class="line number3 index2 alt2"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;</code><code class="js plain">...,</code></div><div class="line number4 index3 alt1"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;</code><code class="js plain">errorMsg: </code><code class="js string">"My custom error message"</code><code class="js plain">,</code></div><div class="line number5 index4 alt2"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;</code><code class="js plain">...,</code></div><div class="line number6 index5 alt1"><code class="js plain">});</code></div><div class="line number7 index6 alt2"><code class="js spaces">&nbsp;&nbsp;&nbsp;</code>&nbsp;</div></div></td></tr></tbody></table></div></div>
					</li>
					
				</ul>
			</div>
		</div>
	</div>


		<div id="ajaxhandler-validate" class="cnqr-option cnqr-outer">
		<div class="cnqr-option-header col-md-12">
			<div class="col-md-5 cnqr-option-name"><strong>validate</strong></div>
			<div class="col-md-4 cnqr-option-default"><strong>Default: </strong>true</div>
			<div class="col-md-3 cnqr-option-type"><span class="pull-right"><strong>Type: </strong>Boolean</span></div>
		</div>
		<div class="cnqr-inner col-md-12">
			<div class="cnqr-option-content">
				<p>Attach Validation to any forms that the Ajax response might have.</p>
					<div><div class="syntaxhighlighter  js" id="highlighter_551009"><table cellspacing="0" cellpadding="0" border="0"><tbody><tr><td class="gutter"><div class="line number1 index0 alt2">1</div><div class="line number2 index1 alt1">2</div><div class="line number3 index2 alt2">3</div><div class="line number4 index3 alt1">4</div><div class="line number5 index4 alt2">5</div><div class="line number6 index5 alt1">6</div><div class="line number7 index6 alt2">7</div><div class="line number8 index7 alt1">8</div></td><td class="code"><div class="container"><div class="line number1 index0 alt2"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;</code>&nbsp;</div><div class="line number2 index1 alt1"><code class="js comments">//After</code></div><div class="line number3 index2 alt2"><code class="js plain">$.ajax({</code></div><div class="line number4 index3 alt1"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;</code><code class="js plain">...,</code></div><div class="line number5 index4 alt2"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;</code><code class="js plain">validate: </code><code class="js keyword">true</code><code class="js plain">,</code></div><div class="line number6 index5 alt1"><code class="js spaces">&nbsp;&nbsp;&nbsp;&nbsp;</code><code class="js plain">...,</code></div><div class="line number7 index6 alt2"><code class="js plain">});</code></div></div></td></tr></tbody></table></div></div>
			</div>
		</div>
	</div>
