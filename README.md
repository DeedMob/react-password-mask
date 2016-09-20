# react-password-mask

Show/hide the contents of a password field.

## Installation

Install:

```sh
$ npm install react-password-mask
```

## Usage

```js
import PasswordMask from 'react-password-mask';
```

```js
<PasswordMask
  className="form-control"
  id="password"
  name="password"
  placeholder="Enter password"
  value={ui.password}
  onChange={this.handleChange.bind(this)}
  hideOnTimeout={400}
/>
```

    value: PropTypes.any.isRequired,
    className: PropTypes.string,
    id: PropTypes.string,
    name: PropTypes.string,
    placeholder: PropTypes.string,
    onChange: PropTypes.func,
    onShow: PropTypes.func,
    onHide: PropTypes.func,
    onToggle: PropTypes.func,
    hideOnTimeout: PropTypes.number,
    inputStyles: PropTypes.object,
    buttonStyles: PropTypes.object

## Options

| option        | type      | description                                                   |
|---------------|-----------|---------------------------------------------------------------|
| `value`       | any       | The value of the password field.                              |
| `className`   | string    | A space-separated list of HTML `class` attributes.            |
| `id`          | string    | The HTML `id` attribute used for the password field.          |
| `name`        | string    | The HTML `name` attribute used for the password field.        |
| `placeholder` | string    | The HTML `placeholder` attribute used for the password field. |
| `onChange`    | function  | A callback function to be invoked when the `value` of the field changes. Receives an argument containing the current value of the field. |
| `onShow`      | function  | A callback function to be invoked when the `value` of the field is shown. Receives an argument containing the current value of the field. |
| `onHide`      | function  | A callback function to be invoked when the `value` of the field is masked. Receives an argument containing the current value of the field. |
| `onToggle`    | function  | A callback function to be invoked when the `value` of the field is shown or masked. Receives an argument containing the current value of the field. |
| `hideOnTimeout` | number  | The amount of time (in milliseconds) that the password `value` will be shown for after being changed. |
| `inputStyles` | object  | The CSS styles to be applied to the password field.            |
| `buttonStyles`| object  | The CSS styles to be applied to the show/hide button.          |

## License

MIT