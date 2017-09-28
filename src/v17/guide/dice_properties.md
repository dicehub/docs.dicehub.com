---
title: diceProperties
type: guide
order: 16
---

### Properties

<p style="text-align: center">
  <img style="width:700px" src="/images/diceProperties.png" alt="wvc, dice">
</p>

#### Example

Define a button in QML:
```JS
ValueField {
  target: app
  property: "quantity"
}
```

The target `app` connects the interface to your application.
In your main application file you can then define the property in the following way:

```python
@diceProperty('QVariant', name='quantity')
def quantity(self):
  return self.__config.get('quantity', 1e-6)
```

This way you interface shows the value from the configuration variable/file. Next step is to make sure that you can also change the value by defining a `setter`:

```python
@quantity.setter
def quantity(self, value):
  if self.quantity != value:
    self.__config['quantity'] = value
    self.__config.write()
```
If the value is different than what was in the `self.__config['quantity']` variable it will change and written into the configuration file.
