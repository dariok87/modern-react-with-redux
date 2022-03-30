Udemy
Modern React with Redux
Practicing List Building
In your React career, you'll build a tremendous number of lists, so let's get some practice right away!

Goal

Given a list of users, print out each user's name inside of an li element

Example

Here's the final structure of HTML that you're trying to create:

<ul>
  <li>Leanne Graham</li>
  <li>Ervin Howell</li>
  <li>Clementine Bauch</li>
  <li>Patricia Lebsack</li>
</ul>
Hints

You'll need to map over the array of users. You can do this in the render method, or define a helper method

When you build the list, don't forget to provide a key prop to each individual item.  You can use the id of a user for this

```javascript
import React from 'react';

const users = [
  { id: 1, name: 'Leanne Graham' },
  { id: 2, name: 'Ervin Howell' },
  { id: 3, name: 'Clementine Bauch' },
  { id: 4, name: 'Patricia Lebsack' }
];


export default class App extends React.Component {
  render() {
    const listUsers = users.map(({id, name}) => {
      return <li key={id}>{name}</li>;
    });
    return (
        <ul>
          {listUsers}
        </ul>
    );
  }
}
```


