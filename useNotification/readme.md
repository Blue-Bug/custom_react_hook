# @custom_react_hook/use-notification

React Hook to use Notification.  
This function need to allow browser's `Notification Permission`.

## Installation

#### yarn

`yarn add @custom_react_hook/use-notification`

#### npm

`npm i @custom_react_hook/use-notification`

## Usage

```js
import React from "react";
import useNotification from "@custom_react_hook/use-notification";
function App() {
  const triggerNotif = useNotification("Notification TEST", {
    body: "Notification content"
  });
  return <button onClick={triggerNotif}>Make a Notification</button>;
}
```

### Arguments

| Argument | Type   | Description                                | Required |
| -------- | ------ | ------------------------------------------ | -------- |
| title    | string | The title of Notification | yes      |
| opts | JSON | Notification's options https://developer.mozilla.org/ko/docs/Web/API/notification| yes|

### Return

| Return value | Type   | Description                                                                                                                     |
| ------------ | ------ | ------------------------------------------------------------------------------------------------------------------------------- |
| Function    | Function | A Function can make a notification|