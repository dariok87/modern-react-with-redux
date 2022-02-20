# Test Your Knowledge: Props

Check out the code below.  Right now it contains two components: the App and the Message .  The code works, but notice that the Message component has a hard-coded header of Changes in Service and hard-coded message of We just updated... .

As it stands, the Message component can't be reused to show any other message!

Your goal:

Refactor the Message component so that it receives its props from the parent component (the App).

The Message should receive a prop of header and text

The Message should show the header prop inside of the div with className header and the text prop inside of the paragraph tag.

```javascript
<script type="text/babel" data-presets="env,react">
    const App = () => {
        return (
            <div>
                <Message header='Changes in Service' text='We just updated our privacy policy here to better service our customers' />
            </div>
        );
    }
    
    const Message = (props) => {
        return (
            <div className="ui message">
                <div className="header">{props.header}</div>
                <p>{props.text}</p>
            </div>
        );
    }
    

    // Renders the App component into a div with id 'root'
    ReactDOM.render(<App />, document.querySelector('#root'));
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
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/semantic-ui/2.4.1/semantic.min.css" />
```

