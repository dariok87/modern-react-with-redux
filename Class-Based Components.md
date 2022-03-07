Udemy
Modern React with Redux
Class-Based Components
See the code below, which creates a component called UserForm .  Right now the UserForm is a functional component.

Your goal:

Refactor the UserForm to be a class-based component.  It should return the exact same JSX.

Remember that class-based components must:

Be a Javascript class

Extend React.Component

Implement a render method that returns some JSX


```javascript
<script type="text/babel" data-presets="env,react">
    const UserForm = () => {
        return (
            <form>
                <label>Enter a username:</label>
                <input />
            </form>
        );
    }


    // Renders the App component into a div with id 'root'
    ReactDOM.render(<UserForm />, document.querySelector('#root'));
</script>






<!--The App component above will be rendered into this-->
<div id="root"></div>


<!--No need to change anything after this line!-->
<!--No need to change anything after this line!-->
<script src="https://cdnjs.cloudflare.com/ajax/libs/babel-polyfill/7.0.0/polyfill.min.js"></script>
<script crossorigin src="https://unpkg.com/@babel/standalone@7.0.0/babel.min.js"></script>
<script crossorigin src="https://unpkg.com/@babel/preset-env-standalone@7.0.0/babel-preset-env.min.js"></script>
<script src="https://unpkg.com/react@16/umd/react.production.min.js"></script>
<script src="https://unpkg.com/react-dom@16/umd/react-dom.production.min.js"></script>
<script src="https://unpkg.com/redux@4.0.1/dist/redux.js"></scr
```

