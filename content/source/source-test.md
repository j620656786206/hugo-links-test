+++
date = "2016-07-12T11:57:15+02:00"
draft = false
title = "Testing sourceRelativeLinksEval links"

+++

## Links

These links are pairwise identical except for the file extension. The
table after each link shows when it works in the cases tested for.

### Absolute paths in links

- [Markdown file (/targets/test.md)](/targets/test.md)

<div style="float: left;">
<b>Hugo 0.16</b><br />
<table>
<tr><td></td><th>BaseURL w/ prefix</th><th>BaseURL w/o prefix</th></tr>
<tr><th>RelativeURLs=true</th><td style="color:red;">Broken</td><td style="color:green;">Works</td></tr>
<tr><th>RelativeURLs=false</th><td style="color:green;">Works</td><td style="color:green;">Works</td></tr>
</table>
</div>
<div style="float: left; margin-left: 1em;">
<b>With patch (#2277):</b><br />
<table>
<tr><td></td><th>BaseURL w/ prefix</th><th>BaseURL w/o prefix</th></tr>
<tr><th>RelativeURLs=true</th><td style="color:green;">Works</td><td style="color:green;">Works</td></tr>
<tr><th>RelativeURLs=false</th><td style="color:red;">Broken</td><td style="color:green;">Works</td></tr>
</table>
</div>
<div style="clear: both;">&nbsp;</div>


- [Image file (/targets/test.png)](/targets/test.png)

<div style="float: left;">
<b>Hugo 0.16</b><br />
<table>
<tr><td></td><th>BaseURL w/ prefix</th><th>BaseURL w/o prefix</th></tr>
<tr><th>RelativeURLs=true</th><td style="color:green;">Works</td><td style="color:green;">Works</td></tr>
<tr><th>RelativeURLs=false</th><td style="color:red;">Broken</td><td style="color:green;">Works</td></tr>
</table>
</div>
<div style="float: left; margin-left: 1em;">
<b>With patch (#2277):</b><br />
<table>
<tr><td></td><th>BaseURL w/ prefix</th><th>BaseURL w/o prefix</th></tr>
<tr><th>RelativeURLs=true</th><td style="color:green;">Works</td><td style="color:green;">Works</td></tr>
<tr><th>RelativeURLs=false</th><td style="color:red;">Broken</td><td style="color:green;">Works</td></tr>
</table>
</div>
<div style="clear: both;">&nbsp;</div>


### Relative paths in links

- [Markdown file (../targets/test.md)](../targets/test.md)

<div style="float: left;">
<b>Hugo 0.16</b><br />
<table>
<tr><td></td><th>BaseURL w/ prefix</th><th>BaseURL w/o prefix</th></tr>
<tr><th>RelativeURLs=true</th><td style="color:red;">Broken</td><td style="color:green;">Works</td></tr>
<tr><th>RelativeURLs=false</th><td style="color:green;">Works</td><td style="color:green;">Works</td></tr>
</table>
</div>
<div style="float: left; margin-left: 1em;">
<b>With patch (#2277):</b><br />
<table>
<tr><td></td><th>BaseURL w/ prefix</th><th>BaseURL w/o prefix</th></tr>
<tr><th>RelativeURLs=true</th><td style="color:green;">Works</td><td style="color:green;">Works</td></tr>
<tr><th>RelativeURLs=false</th><td style="color:red;">Broken</td><td style="color:green;">Works</td></tr>
</table>
</div>
<div style="clear: both;">&nbsp;</div>

- [Image file (../targets/test.png)](../targets/test.png)

<div style="float: left;">
<b>Hugo 0.16</b><br />
<table>
<tr><td></td><th>BaseURL w/ prefix</th><th>BaseURL w/o prefix</th></tr>
<tr><th>RelativeURLs=true</th><td style="color:red;">Broken</td><td style="color:red;">Broken</td></tr>
<tr><th>RelativeURLs=false</th><td style="color:red;">Broken</td><td style="color:red;">Broken</td></tr>
</table>
</div>
<div style="float: left; margin-left: 1em;">
<b>With patch (#2277):</b><br />
<table>
<tr><td></td><th>BaseURL w/ prefix</th><th>BaseURL w/o prefix</th></tr>
<tr><th>RelativeURLs=true</th><td style="color:red;">Broken</td><td style="color:red;">Broken</td></tr>
<tr><th>RelativeURLs=false</th><td style="color:red;">Broken</td><td style="color:red;">Broken</td></tr>
</table>
</div>
<div style="clear: both;">&nbsp;</div>

## Images

Same as above, but for image embed links.

### Absolute path

![Test image (absolute path)](/targets/test.png)

<div style="float: left;">
<b>Hugo 0.16</b><br />
<table>
<tr><td></td><th>BaseURL w/ prefix</th><th>BaseURL w/o prefix</th></tr>
<tr><th>RelativeURLs=true</th><td style="color:green;">Works</td><td style="color:green;">Works</td></tr>
<tr><th>RelativeURLs=false</th><td style="color:red;">Broken</td><td style="color:green;">Works</td></tr>
</table>
</div>
<div style="float: left; margin-left: 1em;">
<b>With patch (#2277):</b><br />
<table>
<tr><td></td><th>BaseURL w/ prefix</th><th>BaseURL w/o prefix</th></tr>
<tr><th>RelativeURLs=true</th><td style="color:green;">Works</td><td style="color:green;">Works</td></tr>
<tr><th>RelativeURLs=false</th><td style="color:red;">Broken</td><td style="color:green;">Works</td></tr>
</table>
</div>
<div style="clear: both;">&nbsp;</div>

### Relative path

![Test image (relative path)](../targets/test.png)

<div style="float: left;">
<b>Hugo 0.16</b><br />
<table>
<tr><td></td><th>BaseURL w/ prefix</th><th>BaseURL w/o prefix</th></tr>
<tr><th>RelativeURLs=true</th><td style="color:green;">Works</td><td style="color:green;">Works</td></tr>
<tr><th>RelativeURLs=false</th><td style="color:red;">Broken</td><td style="color:green;">Works</td></tr>
</table>
</div>
<div style="float: left; margin-left: 1em;">
<b>With patch (#2277):</b><br />
<table>
<tr><td></td><th>BaseURL w/ prefix</th><th>BaseURL w/o prefix</th></tr>
<tr><th>RelativeURLs=true</th><td style="color:green;">Works</td><td style="color:green;">Works</td></tr>
<tr><th>RelativeURLs=false</th><td style="color:red;">Broken</td><td style="color:green;">Works</td></tr>
</table>
</div>
<div style="clear: both;">&nbsp;</div>
