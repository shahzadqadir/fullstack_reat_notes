```sh
# Create first project
create-react-app demo   # might need root access
# install npm router
npm install react-router --save
# start react app, this will start a default app on port 3000
sudo npm start
```

### Create first custom web page

```shell
# remove existing app and styles
rm App.js App.css
```

1. Add custom file(s) for our project

```shell
# within src directory, add following file
touch Application.js
```

2. Add following to Application.js 

```javascript
import { Component } from "react";


class Application extends Component {
  render() {
    let name = "Shahzad";
    return (
      <div>
        <h1>Hello {name}</h1>
        <p>I hope you make sense to me this time round.</p>
      </div>
    )
  }
}

export default Application
```

3. Update index.js with new file details

```javascript
import Application from './Application';

root.render(
  <React.StrictMode>
    <Application />
  </React.StrictMode>
);

```

4. Run react application

```shell
sudo npm start
```
