---
layout: default
jsLib: jquery
---

### confirm ###
{% highlight javascript %}
$("#confirmMsgBox").on("click", function () {
	$.cnqr.messagebox.confirm({
		message: "Lorem ipsum dolor sit amet, consectetur adipiscing elit."
	});
});
{% endhighlight %}

### success ###
{% highlight javascript %}
$("#successMsgBox").on("click", function () {
	$.cnqr.messagebox.success({
		message: "Lorem ipsum dolor sit amet, consectetur adipiscing elit."
	});
});
{% endhighlight %}

### info ###
{% highlight javascript %}
$("#infoMsgBox").on("click", function () {
	$.cnqr.messagebox.info({
		message: "Lorem ipsum dolor sit amet, consectetur adipiscing elit."
	});
});
{% endhighlight %}

### warning ###
{% highlight javascript %}
$("#warningMsgBox").on("click", function () {
	$.cnqr.messagebox.warning({
		message: "Lorem ipsum dolor sit amet, consectetur adipiscing elit."
	});
});
{% endhighlight %}

### error ###
{% highlight javascript %}
$("#errorMsgBox").on("click", function () {
	$.cnqr.messagebox.error({
		message: "Lorem ipsum dolor sit amet, consectetur adipiscing elit."
	});
});
{% endhighlight %}
