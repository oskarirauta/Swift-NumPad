# Swift-NumPad
NumPad keyboard for iOS. For both, iPhone and iPad.

# NumPad Framework
Shared framework which provides 2 new public classes:
  - NumPad
  - DoneBar
  
# NumPad class
NumPad class provides a NumPad style keyboard for iOS platforms with some styling properties.
Class can have type set to one of following types:
  - number: Simple digit input
  - decimal: Decimal number input (adds decimal point button)
  - phone: Phone number input ( adds + button and changes appearance of buttons in portrait mode )
  
# NumPad Styling
NumPad can be styled with following attributes:
  - overlayColor ( view background )
  - backgroundColor ( button background )
  - backgroundColorHighlighted ( button background when highlighted )
  - shadowColor ( button shadow color )
  - foregroundColor ( button text color )
  - foregroundColorHighlighted ( button text color when highlighted )
  - font ( button font and +/. button font )
  - phoneFont ( button font when using phone type )
  - phoneCharFont ( when phone type is used, this font is used for letters )
  - backspaceColor ( color of backspace icon )

# DoneBar class
Donebar is a fast UIToolbar initializer with Done button aligned to right.

# Usage
Used with UITextField or UITextView.

```
var tf: UITextField = UITextField(frame: .zero)
...
tf.inputView = NumPad(delegate: tf, type: .number)
tf.inputAccessoryView = DoneBar(delegate: tf)
```

See provided example.

# Screenshots

![Screenshot of decimal keyboard](https://raw.githubusercontent.com/oskarirauta/Swift-NumPad/master/Screenshots/Decimal.png)   ![Screenshot of phone keyboard](https://raw.githubusercontent.com/oskarirauta/Swift-NumPad/master/Screenshots/Phone.png)

![Landscape screenshot](https://raw.githubusercontent.com/oskarirauta/Swift-NumPad/master/Screenshots/Landscape.png)
