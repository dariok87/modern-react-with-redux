Udemy
Modern React with Redux
Updating Components with State
Note: this is a tough problem, if you have trouble with it then check out the solutions!

The Clock class below is trying to implement a clock display that updates every second.  Right now, a beginner engineer tried putting the component together, but they're finding that they can't get the time to update!

Your goal:

Update the Clock class so that it properly updates once per second

Hints:

You definitely need to use 'state'.  Make sure you initialize the 'state' object.

Remember that you can get your component to update by calling setState

Remember that you only update state by calling setState

```javascript
<script type="text/babel" data-presets="env,react">
    class Clock extends React.Component {
        state = { time: new Date().toLocaleTimeString() }

        componentDidMount() {
            setInterval(() => {
                this.setState({ time: new Date().toLocaleTimeString() }) 
            }, 1000)
        }
        
        render() {
            return (
                <div className="time">
                    The time is: {this.state.time}
                </div>
            );
        }
    }
```







