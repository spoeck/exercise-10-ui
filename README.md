# exercise-10-ui
## Building WebComponents with Stencil JS
In this exercise, you get started with the new [W3C Standard](https://www.w3.org/TR/components-intro/) WebComponents. You can find a good introduction at [webcomponents.org](https://www.webcomponents.org/introduction):
> Web components are a set of web platform APIs that allow you to create new custom, reusable, encapsulated HTML tags to use in web pages and web apps. Custom components and widgets build on the Web Component standards, will work across modern browsers, and can be used with any JavaScript library or framework that works with HTML.
>
> Web components are based on existing web standards. Features to support web components are currently being added to the HTML and DOM specs, letting web developers easily extend HTML with new elements with encapsulated styling and custom behavior.

You can develope WebComponents in plain HTML, CSS and JS. Although we want to use a library or framework which comes with less overhead, simpler lifecycle management and other benefits. But before our project relates on a runtime dependency the better approach is to compile the component at build time to a WebComponent. And this is how [stencil](https://stenciljs.com/) joins the game. Stencil feels like a library but it's a compiler. The output is a plain WebComponent in HTML, CSS and JS with you can use with every other framework.

### 0. Get familiar with WebComponets stencil (20min)
https://www.webcomponents.org/introduction </br>
https://stenciljs.com/docs



### 1. Setup
1. Install npm if you don't have it already.
[Install NPM](https://www.npmjs.com/get-npm)

2. Clone the stater repository for a stencil component
```
git clone https://github.com/ionic-team/stencil-component-starter.git my-component
cd my-component
git remote rm origin
```

3. Install dependencies and start
```
npm install
npm start
```

### 2. Developing a simple text-based component
Change your component `my-component.tsx`. Change the prop `first` and `last` to a single `name` for example. Add an image tag and use scss or inline styles.
Inline styling:  `<div style={{color: 'red'}}>`

### 3. Compile the component and use it
Compile it to a WebComponent with
```
npm run build
```
Create in a new directory a new folder with an `index.html`. Copy everything of your `dist` folder into the new folder. Import and use your component via the `<script>` tag. Open the index.html with chrome or safari and your component should be displayed.

### 4. Create a new dynamic component
Create a second component and use a `<button>` which changes the color of a text. The component holds the color in it's state. If the state changes it will be re-rendered. More info about the state at https://stenciljs.com/docs/decorators

### 5. Compile the new componentn and use it as well as the first one
Same as 3.

### 6. Be creative: Create a more complex component
You can also find team members and build a small website. If you're a lone wolf you can make your components pretty and get familiar with scss and inline styles.
