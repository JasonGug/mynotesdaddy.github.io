# Events

### Configuration

```javascript
//Code part I
data:{
	name : 'Test',
	job : 'Developer',
	age : 25,
	x: 0,
	y: 0,
	},
methods :{
	reset : function(){
		this.age = 25;
	}, // this will reset the age to 25
	OR
	reset : function(int){
		this.age = int;
	}, // this will reset the age to the parameter int
	//NOTE They can exist together even if the method name is the same
	updateXY : function (event){
		this.x = event.offsetX;
		this.y = event.offsetY;
	}
}
```

* Define the data, methods \(functions\).

### Event I

* v-on:click:event is triggered when left mouse clicking.
* v-on:dbclick:event is triggered when left mouse click twice.

Example:

```markup
<button v-on:click="age++">Add a year</button> 
//age will listen to the event on click (age++)

<button v-on:click="age--">Subtract a year </button> 
//age will listen to the event on click (age--)

<button v-on:click="reset">Reset</button>
 //age will listen to the event on click (reset : function())
 
<button v-on:dblclick="reset(25)">Reset to 25</button>
 //age will listen to the event on double click (reset : function(int))
```

Simple way of writing event: Replace \[v-on:\] to \[@\]:

```markup
<button @click="age++">Add a year</button>
<button @click="age--">Subtract a year </button>
<button @click="reset">Reset</button>
<button @dblclick="reset(25)">Reset to 25</button>
```

### Event II

v-on:mousemove: event is triggered when the mouse is move on the canvas

Example:

```markup
<div id="canvas" v-on:mousemove="updateXY">{{x}},{{y}}</div>
 //When mouse move, X and Y will change based on the cursor axis in the canvas. 
```



