# react-native-controlled-keyboard
A fully controllable keyboard with many listeners and callbacks

## Install

`npm install react-native-controlled-keyboard`

## integrate it in your appear

```
import ControlledKeyboard from 'react-native-controlled-keyboard'

...

render() {
  return (
    <ControlledKeyboard ... />
  );
}
```

## Props tab

| props name         | props type             | desc                                              |
|--------------------|------------------------|---------------------------------------------------|
| onKeyPressed       | `(text: String) => {}` | each time a key as been pressed                   |
| onShow             | `() => {}`             | each time the keyboard appear                     |
| onHide             | `() => {}`             | each time the keyboard disappear                  |
| onSubmit           | `() => {}`             | when return key is pressed                        |
| keyboardType       | `String`               | look for `TextInput.propTypes.keyboardType`       |
| keyboardAppearance | `String`               | look for `TextInput.propTypes.keyboardAppearance` |
| returnKeyType      | `String`               | look for `TextInput.propTypes.returnKeyType`      |

## method tab

| method      | return  | desc                                        |
|-------------|---------|---------------------------------------------|
| show()      | Boolean | show the keyboard, return `false` if failed |
| hide()      | Boolean | hide the keyboard, return `false` if failed |
| isVisible() | Boolean | return `true` if keyboard is on the screen  |
