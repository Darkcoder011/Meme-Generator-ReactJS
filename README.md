# Meme-Generator-ReactJS 🤪
Creating a **`Meme Generator App`** using `ReactJS`


<!-- ## [Live Preview](https://hmjatt.github.io/Meme-Generator-ReactJS/)

![This is an image]()
![This is an image]() -->

<hr>
<hr>

### About ℹ️

This app generates a *meme* by reaching out to `imgflip API`, getting the 100 most popular *meme images* at that time. One of those *meme images* will be and users can enter the *meme text*. The `meme text` will then be placed over the selected `meme image`, hence creating a `meme` :trollface: and users can also press a `button` to generate a new `meme image`. By creating this project I learned about `Event Listeners in React`, `React State`, `Conditional Rendering in React`, `React Forms`, `React Hooks(useEffect)`, etc. After creating the project, it was deployed to `GitHub Pages` :bird: Feel free to reach me on[Twitter](https://twitter.com/hmjatt/) 🪶

<hr>
<hr>

### Technologies Used 💻

<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="50" height="50"/> </a> &emsp; <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="50" height="50"/> </a> &emsp; <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="50" height="50"/> </a> &emsp; <a href="https://www.w3schools.com/js/js_es6.asp" target="_blank" rel="noreferrer"> <img src="https://camo.githubusercontent.com/792f7fce1ff8bfac6d0524a21b69161cdc6080a3c4e39979f21d5f8489d6fdd3/68747470733a2f2f692e626c6f67732e65732f3534356366382f6573362d6c6f676f2f6f726967696e616c2e706e67" alt="ES6" width="50" height="50"/> </a> &emsp; <a href="https://reactjs.org/" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/a/a7/React-icon.svg" alt="reactJS" width="50" height="50"/> </a> &emsp; <a href="https://www.figma.com/" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/a/ad/Figma-1-logo.png" alt="figma" width="70" height="50"/> </a>

<hr>
<hr>

## Includes the following features/components ⚙️

    - ReactJS
    - create-react-app
    - Figma Design Template
	- imgflip API
	- Event Listeners in React
	- React State
	- React Forms
	- Conditional Rendering in React
	- React Hooks(useEffect)
    - github-pages

<hr>
<hr>

## Usage 🤓

```
cd meme-generator

```

```
npm install

```

```
npm start

```
<hr>
<hr>

## Steps I followed to complete this project 🪜


### 1. Initialize Project 🎍
- [x] Initialize the project using `npx create-react-app meme-generator` which will create a 
complete **React App** pre-configured and pre-installed with all the dependencies.

- [x] Import **`Karla`** font from google fonts and apply it to the **`App`** component.

<hr>

### 2. Organize components 🗄️
- [x] Create a `components` folder inside the `src` directory.

- [x] Create **custom components** inside the `components` folder.

- [x] Create an `images` folder inside the `src` directory and add images/logos inside it. 

- [x] Create a `styles` folder inside the `src` directory and add `.css` files inside it.

<hr>

### 3. Clean directory🧹
- [x] Delete **unnecessary** files and code from the directory.

<hr>

### 4. Header Component 🧩
- [x] Create a **`Header`** component and basic JSX elements for it.

- [x] Add appropriate `className`s to elements in the `Header` component.

- [x] Add `troll-face.png` image to the **`Header`** component.

- [x] Import **`Header`** component inside `App` component.

- [x] Style **`Header`** and **`App`** component.

<hr>

### 5. Meme Component 🧩
- [x] Create a **`Meme`** component and basic JSX elements for it.

- [x] Add appropriate `className`s to elements in the `Meme` component.

- [x] Import **`Meme`** component inside **`App`** component.

- [x] Add basic style to **`Meme`** component.

<hr>

### 6. Footer Component 🧩
- [x] Create **`Footer`** component and basic JSX elements for it.

- [x] Import **`Footer`** component inside `App` component.

- [x] Style **`Footer`** component.

<hr>

### 7. Get Random Meme 🪄
- [x] Change `<form>` to `<div>` inside the **`Meme`** component as we don't need to submit our *form* instead just get a `meme image`.

- [x] Create a `memesData.js` inside the `data` folder which is an *object of 100 most popular meme images* returned after making an *API request* to `imgflip API`.

- [x] Import `memesData.js` as `memesData` *object* inside the **`Meme`** component.

- [x] Select a *random meme image's* `url` property, `console.log(url)` using `onClick={getRandomImage}` *react mouse event property* when `Get a new meme image 🖼️` *button* is clicked.

- [x] `console.log(url)` for now as our `UI` won't update if we insert the `url` *variable* inside the **`Meme`** component. Because this has everything to do with the way *react* deals with updating the `UI` using *variables*. `⚠️ Spoiler Alert!!!: React doesn't just insert every variable that is declared inside our component`.

<hr>

### 8. Add Images to the Meme Generator 🖼️
- [x] Save the *random meme URL* in *state* and *import the react* `{ useState }` *hook*.

- [x] Create a new *state* called `memeImage` with an empty string as default.

- [x] When the `getMemeImage` function is called, update the `memeImage` *state* to be the *random image URL*

- [x] Below the `div.form`, add an `<img />` element and set the src to the new `memeImage` state we created.

- [x] Style newly created `<img />` element.

<hr>

### 9. Refactor State 🔃
- [x] Update our *state* to save the meme-related data as an object called `meme`. It should have the following *3 properties*: `topText, bottomText, randomImage`.

- [x] The *2 text states* can default to empty strings for now, and `randomImage` should default to `"http://i.imgflip.com/1bij.jpg"`

- [x] Next, create a *new state variable* called `allMemeImages` which will default to `memesData`, which we imported at the top of `Meme.js`

- [x] Lastly, update the `getMemeImage` function and the markup to reflect our newly reformed state object and array in the correct way

<hr>

### 10. Add Text to Image 📝
- [x] Update `topText` element to have a `value={meme.topText}`, `name="topText"` and an `onChange={handleChange}` event handler which will run `{handleChange}` *function* on each key press. On each key press our state changes and *React* re-renders our component and is in charge of maintaining the state. 

- [x] Update `bottomText` element to have a `value={meme.bottomText}`, `name="bottomText"` and an `onChange={handleChange}` event handler which will run `{handleChange}` *function* on each key press. On each key press our state changes and *React* re-renders our component and is in charge of maintaining the state. 

- [x] Create a `handleChange` *function*, use *Destructuring assignment(ES6)* to return a new object i.e., -> `const [name, value] = event.target`. While keeping the old *object(state)* intact create a new *object(state)* by using the spread operator `...prevState`.

- [x]  Override the specific property `[name]: value` using *previous state* and *arrow functions*. Making use of *Computed Properties(ES6)* allows us to turn a *dynamic string(Something Stored in a Variable)* and use it as the property name for our *Object*.

- [ ] Create a `div` with `className=meme` containing `meme-image` and two `<h2>` elements, which will used to show text on top of our `meme-image`.

- [ ] Update our `<h2>` elements by using *values* stored in `{meme.topText}, {meme.bottomText}` *keys* inside our *meme Object*.

- [ ] Style `className=meme` `div` container and `<h2>` elements in it.

<hr>

### 10. Make App Responsive 🎨

<!-- - [x] Add _flexbox_ style to `.cards-list` *div* and other *necessary styles*.
- [x] Add a *media query* for `max-width: 600px`.
- [x] App is responsive upto this point. :smiley: -->

<!-- ### 9. Pass object as props(Option #1) 📟

- [ ] Pass entire object when we _.map_ over _array of objects_ in **`App`** component using _item_ as _key_ and _array of objects_ as its _value_.
- [ ] Access the object that is passed as prop in **`Card`** component, where _item_ is _key_ and _array of objects_ are its _values_.

### 10. Spread object as props(Option #2) 📼

- [x] We can make use of `{...item}` [Spread in Object Literals](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax#spread_in_object_literals), which takes properties of our _object_ and create a separate prop for each _key_ in _object_. _Value_ of _props_ can be accessed using `props.key` syntax, where _key_ is an actual _key_ in `data.js`. This is an alternate to instead of creating our own _prop_ called _item_ to which we pass our entire _object_.**`Spread object as props(Option #2) 📼`** is used in this project. -->

### 11. Prepare for Deployment 🪢

<!-- - [x] Create total of 7 unique **`Card`** components(*journal entries*) inside **`.cards-list`** by updating `data.js`.
- [x] Delete **unnecessary** files from directory and format code with `Prettier`.
- [x] Test for _Responsiveness_ and make changes if need be ✅.
- [x] Add links to `Live Preview` and _screenshots_ ✅. -->

### 12. Deploy 📤

- [x] Use Official Documentation([link](https://create-react-app.dev/docs/deployment/#github-pages)) to push the project to **GitHub Pages** 🎆🎆🎆

<hr>
<hr>

## Future Changes ♾️

- [ ] Only show `meme images` that are compatible with app design(*2 text fields - top & bottom*).
- [ ] Update the form based upon the retrieved `meme image`.


<hr>
<hr>

## Links to content that helped me with this project 🔗

1. The Odin Project

    - [React Introduction](https://www.theodinproject.com/lessons/node-path-javascript-react-introduction)
    - [React State & Props](https://www.theodinproject.com/lessons/node-path-javascript-state-and-props)
	- [Handle Inputs And Render Lists](https://www.theodinproject.com/lessons/node-path-javascript-handle-inputs-and-render-lists)


2. Figma Design

    - [Meme Generator](https://www.figma.com/file/MoLwFPHNHJVrzdFurxHzNV/Meme-Generator?node-id=0%3A1)

3. Scrimba

    - [Learn React](https://scrimba.com/learn/learnreact)

4. React Official Documentation

	- [Mouse Events in React](https://reactjs.org/docs/events.html#mouse-events)
    - [State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)
    - [Handling Events](https://reactjs.org/docs/handling-events.html)
    - [Conditional Rendering](https://reactjs.org/docs/conditional-rendering.html)
    - [Lists and Keys](https://reactjs.org/docs/lists-and-keys.html)
    - [Forms](https://reactjs.org/docs/forms.html)
	- [Using the State Hook](https://reactjs.org/docs/hooks-state.html)
	- [Using the Effect Hook](https://reactjs.org/docs/hooks-effect.html)


<hr>
<hr>

#### Quote ✒️

    “People think computers will keep them from making mistakes. They're wrong. With computers you make mistakes faster.”
    — Adam Osborne

> 🦝👻😶‍🌫️