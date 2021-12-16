# Vue.js Components Basics

This lab corresponds to the section **Component Basics** of the VueSchool course 
[Vue.js Components Fundamentals](https://vueschool.io/courses/vuejs-components-fundamentals)

This repository contains only the example codes for 

1. The **click counter** (video *[Introduction to Components](https://vueschool.io/lessons/introduction-to-components)*) and 
2. **plan-picker** 
   
examples used inside the initial section of the tutorial **Component Basics**.

## Folder click-counter: Click Counter Task 


Watch the videos 

1. *[Introduction to Components](https://vueschool.io/lessons/introduction-to-components)* 
2. [Component's Template](https://vueschool.io/lessons/components-template) 2:20


And write your code inside the empty files `index.html` and `app.js`.

Files [click-counter/solution.html](click-counter/solution.html) and [click-counter/solution-app.js](click-counter/solution-app.js) contain the final solution. 

See the solution working at <https://crguezl.github.io/vuejs-components-basics-plan-picker-component/click-counter/solution.html>


```
├── app.js
├── index.html
├── solution-app.js
└── solution.html
```

### Check List

- [ ] Set the initial HTML and load Vue from the CDN
- [ ] Inside the app create the Vue app attached to the corresponding div element 
- [ ] Create a component `click-counter` using `Vue.component`
  - [ ] Add the ´data` function that returns the object with the data. 
  - [ ] Set the `count`
  - [ ] Set the template 
- [ ] Add in the `app` div of the HTML the component just created
- [ ] Insert new instances of the component in the HTML
- [ ] Move the template from the `app.js` to the HTML using  a `script` tag
- [ ] Add a second element, a paragraph `the count is` to the `click-counter` component 
- [ ] Wrap the two elements in a `<div>`

Use as many [emmet expressions](https://docs.emmet.io/cheat-sheet/) as you can to speed up the edition

## Folder plan-picker: Plan Picker Task

Watch the videos 

* [Reusable Components with Props](https://vueschool.io/lessons/reusable-components-with-props) 6:46
* [Nested Components](https://vueschool.io/lessons/nested-components) 1:50
* Global vs Local Components 3:11
* [Communication Between Components with Custom Events](https://vueschool.io/lessons/communication-between-components) 7:24

Leave your solution inside the files `index.html` and `app.js`.

```
├── coffee.jpg
├── index.html
├── logo.png
├── solution-app.js
├── solution.html
└── style.css
```

Files [plan-picker/solution.html](plan-picker/solution.html) and [plan-picker/solution-app.js](plan-picker/solution-app.js) contain the final solution. 

See the solution working at <https://crguezl.github.io/vuejs-components-basics-plan-picker-component/plan-picker/solution.html>

### Check List 

- [ ] Use a minimum number of emmet expressions to generate complete the initial `index.html` to have it as at the beginning of the video [Reusable Components with Props](https://vueschool.io/lessons/reusable-components-with-props). The structure to replicate three or four times has to follow this pattern:
  
  ```html
        <div class="plans">
            <div class="plan">
                <div class="description">
                    <span class="title">
                    The Single
                    </span>
                </div>
            </div>
            ...  more like the one above
        </div>
  ```
  - [ ] Here is a [solution](plan-picker/solution.emmet)
- [ ] Create the `plan` component that encapsulates the template above
- [ ] Add it the `prop` with the `name` and update the HTML accordingly for all the repetitions
- [ ] Add to the Vue app data the `plans` array of Strings with the names of the plans
- [ ] Substitute the repetitions of the `<plan>` component  inside  the HTML for a `v-for`  loop
- [ ] Specify that the `prop` `name` has to be of type `String` and is `required`
- [ ] Nested Components Video: Create a componen <plan-picker>  to encapsulate the `.plans` div


## Skills Covered

After this lab, you'll be familiar with:

- The idea behind components and how Vue.js components work
- Component's template, and couple of ways to define your template
- Communication between components with props and custom events
- What is the difference between global and local component registration
