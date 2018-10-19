# repo-downloader

Open your [repos](https://github.com/matthewgarrison?tab=repositories) page, and run this script in the console window.

```
var ul = document.getElementById('user-repositories-list');
var items = ul.getElementsByTagName("li");
for (var i = 0; i < items.length; ++i) {
	var a = items[i].getElementsByTagName("div")[0].getElementsByTagName("h3")[0].getElementsByTagName("a")[0];
	console.log(a.href);
	var link = a.href + "/archive/master.zip";
	console.log(link);
	window.open(link, '_blank');
}
```
