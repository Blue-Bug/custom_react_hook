# @custom_react_hook/use-title

React Hook to update your document's title.

## Installation

#### yarn

`yarn add @custom_react_hook/use-title`

#### npm

`npm i @custom_react_hook/use-title`

## Usage

```js
import React from "react";
import useTitle from "@custom_react_hook/use-title";
function App() {
  useTitle("Welcome");
  return <h1>Welcome</h1>;
}
```

### Arguments

| Argument | Type   | Description                                | Required |
| -------- | ------ | ------------------------------------------ | -------- |
| title    | string | The title you want to use on your document | yes      |