# Sublime HTML - Custom

> Custom Sublime Text 3 HTML syntax definition. 


### Install
Go to your sublime text packages folder and run:

    git clone https://github.com/ionutvmi/sublime-html.git 'HTML'

You can find the packages folder under Preferences -> Browser Packages


---------

List of changes from the default package:

**Added support for underscore/handlebars script templates**

```html
<script type="text/template">
    <!-- html here -->
</script>

<script type="text/html">
    <!-- html here -->
</script>

<script type="text/x-handlebars-template">
    <!-- html here -->
</script>
```

---------

**Added support for lodash templates**

Code between `<%` and `%>` is is scoped as JavaScript code.
```js
<%
for (var i = 0; i < 10; i++) {
    print(i);
}
%>
```
This removes support for embedded ruby.

---------

**Fixed the script tag comment toggle**  

Before
```
// <script src="main.js"></script>
```
After
```
<!-- <script src="main.js"></script> -->
```
## Credits

- http://stackoverflow.com/a/11886848/1579481
- http://wesbos.com/fix-sublime-text-toggle-comment/
