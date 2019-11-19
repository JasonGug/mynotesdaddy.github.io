# Data Binding

In Vue .js, we are using `v-bind` to bind the data to html attribute.

```javascript
data:{
	name : 'Test',
	job : 'Developer',
	website : 'www.google.com',
	websiteTag : '<a href="www.google.com">The website</a>'
}

<a v-bind:href="website">The website</a> //The data in data attribute from app.js will be binded to the href. 
<value v-bind:id = "name"><value> //id of value will be [Test]
<p v-html="websiteTag"></p>
```

