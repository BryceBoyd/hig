## Less Syntax ##

Adapted from http://lesscss.org/ 

### Variables ###

Variables allow you to specify widely used values in a single place, and then re-use them throughout the style sheet, making global changes as easy as changing one line of code.
<table class="reporttable">
	<tr>
		<th>LESS</th>
		<th>Compiled CSS</th>
	</tr>
	<tr>
		<td>
			<code><pre>
<span class="variable">@@color</span>: <span class="color">#4D926F</span>;

<span class="id">#header</span> {
<span class="attribute">color</span>: <span class="variable">@@color</span>;
}

<span class="element">h2</span> {
<span class="attribute">color</span>: <span class="variable">@@color</span>;
}
</pre></code>
		</td>
		<td>
			<code><pre>
<span class="id">#header</span> {
<span class="attribute">color</span>: <span class="color">#4D926F</span>;
}

<span class="element">h2</span> {
<span class="attribute">color</span>: <span class="color">#4D926F</span>;
}
			</pre></code>
		</td>
	</tr>
</table>

### Mixins ###

Mixins allow you to embed all the properties of a class into another class by simply including the class name as one of its properties. It’s just like variables, but for whole classes. Mixins can also behave like functions, and take arguments, as seen in the example below.

<table class="reporttable">
  <tr>
	<th>LESS</th>
	<th>Compiled CSS</th>
  </tr>
  <tbody><tr><td>
  <code><pre>
<span class="class">.rounded-corners</span> (<span class="variable">@@radius</span>: <span class="number">5px</span>) {
  <span class="attribute">-webkit-border-radius</span>: <span class="variable">@@radius</span>;
  <span class="attribute">-moz-border-radius</span>: <span class="variable">@@radius</span>;
  <span class="attribute">-ms-border-radius</span>: <span class="variable">@@radius</span>;
  <span class="attribute">-o-border-radius</span>: <span class="variable">@@radius</span>;
  <span class="attribute">border-radius</span>: <span class="variable">@@radius</span>;
}

<span class="id">#header</span> {
  <span class="mixin">.rounded-corners</span>;
}

<span class="id">#footer</span> {
  <span class="mixin">.rounded-corners</span>(<span class="number">10px</span>);
}</pre></code></td>

<td>
  <code><pre>
<span class="id">#header</span> {
  <span class="attribute">-webkit-border-radius</span>: <span class="number">5px</span>;
  <span class="attribute">-moz-border-radius</span>: <span class="number">5px</span>;
  <span class="attribute">-ms-border-radius</span>: <span class="number">5px</span>;
  <span class="attribute">-o-border-radius</span>: <span class="number">5px</span>;
  <span class="attribute">border-radius</span>: <span class="number">5px</span>;
}

<span class="id">#footer</span> {
  <span class="attribute">-webkit-border-radius</span>: <span class="number">10px</span>;
  <span class="attribute">-moz-border-radius</span>: <span class="number">10px</span>;
  <span class="attribute">-ms-border-radius</span>: <span class="number">10px</span>;
  <span class="attribute">-o-border-radius</span>: <span class="number">10px</span>;
  <span class="attribute">border-radius</span>: <span class="number">10px</span>;
}</pre></code>
  </td></tr>
</tbody></table>

### Nested Rules ###

Rather than constructing long selector names to specify inheritance, in Less you can simply nest selectors inside other selectors. This makes inheritance clear and style sheets shorter.

<table class="reporttable">
  <tr>
	<th>LESS</th>
	<th>Compileed CSS</th>
  </tr>
  <tbody><tr><td>
  <code><pre>
<span class="id">#header</span> {
  <span class="element">h1</span> {
    <span class="attribute">font-size</span>: <span class="number">26px</span>;
    <span class="attribute">font-weight</span>: bold;
  }

  <span class="element">p</span> { <span class="attribute">font-size</span>: <span class="number">12px</span>;
    <span class="element">a</span> { <span class="attribute">text-decoration</span>: none;
      &amp;<span class="class">:hover</span> { <span class="attribute">border-width</span>: <span class="number">1px</span> }
    }
  }
}
</pre></code></td>
<td>
  <code><pre>
<span class="id">#header</span> <span class="element">h1</span> {
  <span class="attribute">font-size</span>: <span class="number">26px</span>;
  <span class="attribute">font-weight</span>: bold;
}

<span class="id">#header</span> <span class="element">p</span> {
  <span class="attribute">font-size</span>: <span class="number">12px</span>;
}

<span class="id">#header</span> <span class="element">p</span> <span class="element">a</span> {
  <span class="attribute">text-decoration</span>: none;
}

<span class="id">#header</span> <span class="element">p</span> <span class="element">a</span><span class="class">:hover</span> {
  <span class="attribute">border-width</span>: <span class="number">1px</span>;
}
</pre></code>
  </td></tr>
</tbody></table>

### @@import in LESS ###