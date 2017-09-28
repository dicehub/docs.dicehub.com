---
title: Advanced Features
type: guide
order: 3
---

### WVC: "Whatever"-View-Controller

<p style="text-align: center">
  <img style="width:700px" src="/images/WVC.png" alt="wvc, dice">
</p>

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

### Slots

<p style="text-align: center">
  <img style="width:700px" src="/images/diceSlots.png" alt="wvc, dice">
</p>

### Synchronize

<p style="text-align: center">
  <img style="width:700px" src="/images/diceSync.png" alt="wvc, dice">
</p>

### User Defined Protocols

<p style="text-align: center">
  <img style="width:700px" src="/images/UD Protocols.png" alt="wvc, dice">
</p>

### Tasks

<p style="text-align: center">
  <img style="width:700px" src="/images/diceTasks.png" alt="wvc, dice">
</p>
