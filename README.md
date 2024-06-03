
<h1 style="margin: 0" align="center">oono stories npm package</h1>
<p align="center">A React component for oono js library (this library is used in oono-dashboard project to display the oono widget component)</p>
<p>It just rendering a widget with a specific ring and brand and creates an iframe that shows stories for a specific oono account or brand </p>



## Install

- create an organization on npmjs.com
- create an npm package under the organization (eg: oono/oono-js)

```bash
npm install --save @oono/oono-js (current name is @wecansync/oono-js)
```

## Usage

```jsx
import React, { Component } from 'react';

import oonoStories from 'oono-js';

const App = () => {
	const conf = {
            "containerId": "oono-widget",
            "host": "oono.ai",
            "widgetId": "eb59c125-2a0f-47e5-a8e1-510e5b43d1a9",
            "tenantId": "680560390",
            "scheme": "https://"
        };
useEffect(() => {
new oonoStories(conf);
}, []);
	return (
		<div id="oono-widget">
    <div>
	);
};
```

## Test

```
git clone <package-path>
cd <package-dir>
cd example
open index.html
```

