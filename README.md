# A Simple Accordion Menu in Vue JS



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
 
#### Event Handling
 
 - v-show vs v-if, use v-show if the element will toggle frequently. v-show uses css and is faster
    Use v-if if the condition does not change a lot.

#### Simple animation
 

## Sources

- [Treehouse Vue.js Basics Course](https://teamtreehouse.com/library/vuejs-basics)