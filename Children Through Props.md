Take a look at the code below. The App is showing two separate groups of elements. Notice how there is one element that is giving both these groups the nice grey background - it is the <div className="ui placeholder segment"></div> .

Your goal:

Create a new reusable component called Segment that takes some child elements and shows them inside of a div with classNames of ui placeholder segment.

Refactor the App to use this new Segment component

```javascript
<script type="text/babel" data-presets="env,react">
    const App = () => {
        const Segment = (props) => {
  return (
      <div className="content">{props.children}</div>
  );
};
        return (
            <div className="ui placeholder segment">
                <Segment>
                    <div className="ui icon header">
                        <i className="pdf file outline icon"></i>
                        No documents are listed for this customer.
                    </div>
                    <div className="ui primary button">Add Document</div>
                    <h4 className="ui header">For Your Information</h4>
                    <p>
                        Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo.
                    </p>
                </ Segment>
            </div>
        );
    }




    // Renders the App component into a div with id 'root'
    ReactDOM.render(<App />, document.querySelector('#root'));
</script>


<!--The App component above will be rendered into this-->
<div id="root"></div>
```
