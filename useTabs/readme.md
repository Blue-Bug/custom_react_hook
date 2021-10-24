# @custom_react_hook/use-tabs

React Hook to change your tab.

## Installation

#### yarn

`yarn add @custom_react_hook/use-tabs`

#### npm

`npm i @custom_react_hook/use-tabs`

## Usage

```js
import React from "react";
import useTabs from "@custom_react_hook/use-tabs";
function App() {
  const myTabs = ["apple","banana","pear"];
  const { currentItem, changeItem } = useTabs(myTabs);
  return (
    { myTabs.map((content,index) => (
      <button onClick={() => changeItem(index)}>
        { content }
      </button>
    ))}
    <div>{ currentItem }</div>
  );
}
```

### Arguments

| Argument | Type   | Description                                | Required |
| -------- | ------ | ------------------------------------------ | -------- |
| allTabs    | Array | an Array containing allTabs | yes      |
| initialTab | Number | initial tab's index (default = 0)                      | no      |