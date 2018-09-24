# A Simple Accordion Menu in Vue JS

- [ ] Work in Process

## Dependencies

- Vue Js, installed via Content Delivery Network
```  
    <script src="https://cdn.jsdelivr.net/npm/vue@2.5.13/dist/vue.js"></script>
```

## Project setup

- Open index.html

## Misc Notes

- Templating and data binding

#### Methods and directives

- Use v-for to loop through an array of objects
- Use v-show to show/hide details for each object in the list
```
<ul>
    <li v-for="media in mediaList" v-on:click="toggleDetails(media)">
      <h3>{{media.title}}</h3> 
      <div v-show="media.showDetail">
        <p>{{media.description}}</p>
        <p class="byline">By: {{media.contributor}}</p>
      </div>
    </li>
</ul>
 ```
 
 - v-if
 - v-else
 - [v-show vs v-if](https://vuejs.org/v2/guide/conditional.html#v-if-vs-v-show), use v-show if the element will toggle frequently. v-show uses css and is faster.  Use v-if if the condition does not change a lot.
 
 
#### Event Handling
 
- Use the event object in Vue to filter a list of items by type. 
```
//In Vue instance
filterList = function(event) {...}

//In Vue template 
<select v-on:change="filterList">
```
- "When an event happens, the browser creates an event object, puts details into it and passes it as an argument to the handler. [[JavaScript.info]](https://javascript.info/introduction-browser-events#event-object)
- [X] Create a dynamic select menu that populates the selections from our data. If a selection type is added to our data, the option will be added to our selection menu automatically.




#### Simple animation
 

## Sources

- [Treehouse Vue.js Basics Course](https://teamtreehouse.com/library/vuejs-basics)
- [VueJS.org: v-show vs v-if](https://vuejs.org/v2/guide/conditional.html#v-if-vs-v-show)
- [Javascript.info: Event Object[(https://javascript.info/introduction-browser-events#event-object)
