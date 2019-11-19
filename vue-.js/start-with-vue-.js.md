# Start with Vue .js

## What is Vue.js

* front-end framework
* Create js driven web application
* Runs in the browser
* lean \(16 KB\)
* High run-time performance

Example:

```javascript
new Vue({
el: "#app", //Represent the element that we want to control in html
	data: {
		bobby: {
			name: "bobby",
			age: 25,
		},
		john:{
			name: "john",
			age: 22,
		}
	},
	methods : {
		greet : funtion(time){
			return 'Good' + time + ' ' + this.bobby.name; 
			// With Vue, all data in data attribute will be passed 
			//to the top Vue variable and can be refered even they 
			//are not in same level. For example, in js, we need to 
			//write as this.data.name and here, we can simply write this.name
		}
	}
})
<p>{{greet(Afternoon)}}</p> //Good afternoon will be displayed
```

