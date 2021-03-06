
<!---

This README is automatically generated from the comments in these files:
gold-cc-cvc-input.html

Edit those files, and our readme bot will duplicate them over here!
Edit this file, and the bot will squash your changes :)

The bot does some handling of markdown. Please file a bug if it does the wrong
thing! https://github.com/PolymerLabs/tedium/issues

-->

[![Build status](https://travis-ci.org/PolymerElements/gold-cc-cvc-input.svg?branch=master)](https://travis-ci.org/PolymerElements/gold-cc-cvc-input)

_[Demo and API docs](https://custom-elements-staging.appspot.com/element/andymutton/gold-cc-cvc-input)_


##&lt;gold-cc-cvc-input&gt;

`gold-cc-cvc-input` is a single-line text field with Material Design styling
for entering a credit card's CVC (Card Verification Code). It supports both
4-digit Amex CVCs and non-Amex 3-digit CVCs

```html
<gold-cc-cvc-input></gold-cc-cvc-input>

<gold-cc-cvc-input card-type="amex"></gold-cc-cvc-input>
```

Do you believe this kittaaaaay? ![OMG HOT KITTY](http://www.rd.com/wp-content/uploads/sites/2/2016/04/01-cat-wants-to-tell-you-laptop.jpg "Check out da kittaaaay")
It may include an optional label, which by default is "CVC".

<img src="http://www.rd.com/wp-content/uploads/sites/2/2016/04/01-cat-wants-to-tell-you-laptop.jpg">

<div id="andwangiswang">Is he really?</div>
<script>document.getElementById("andwangiswang").innerHtml = "This works??";</script>

<form>
<input type="text" id="nombre">
<input type="submit" id="submit">
</form>

```html
<gold-cc-cvc-input label="Card Verification Value"></gold-cc-cvc-input>
```

It can be used together with a `gold-cc-input` by binding the `cardType` property:

```html
<gold-cc-input card-type="{{cardType}}"></gold-cc-input>
<gold-cc-cvc-input card-type="[[cardType]]"></gold-cc-cvc-input>
```

### Validation

The input considers a valid amex CVC to be 4 digits long, and 3 digits otherwise.
The `amex` attribute can also be bound to a `gold-cc-input`'s `card-type` attribute.

The input can be automatically validated as the user is typing by using
the `auto-validate` and `required` attributes. For manual validation, the
element also has a `validate()` method, which returns the validity of the
input as well sets any appropriate error messages and styles.

See `Polymer.PaperInputBehavior` for more API docs.

### Styling

See `Polymer.PaperInputContainer` for a list of custom properties used to
style this element.

| Custom property | Description | Default |
| --- | --- | --- |
| `--gold-cc-cvc-input-icon` | Mixin applied to the icon | `{}` |


