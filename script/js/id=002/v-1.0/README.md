# Copy Button
## v-1.0

#### Codepen [Click Here](https://codepen.io/Samson-kiran-02/pen/PoKLVVP).

### Html
```html
<script src="https://samsonkiran02.github.io/p/script/js/id=002/v-1.0/copybutton.js"></script>

<input type="text" value="SK - copy_id-001" id="copy_id-001">
<span class="copybutton" data-clipboard-action="copy" data-clipboard-target="#copy_id-001">Copy</span>

<input type="text" value="SK - copy_id-002" id="copy_id-002">
<span class="copybutton" data-clipboard-action="copy" data-clipboard-target="#copy_id-002">Copy</span>

<script>
$(function () {
	var intv = setInterval(function () {
		$(".copybutton").html('Copy');
	}, 2000);
	$("body").on('click', ".copybutton", function () {
		$(".copybutton").html('Copy');
		$(this).html('Copied');
		clearInterval(intv);
	});
});
var clipboard = new ClipboardJS('.copybutton');
clipboard.on('success', function (e) {
	//console.log(e);
});
clipboard.on('error', function (e) {
	//console.log(e);
});
</script>
```
