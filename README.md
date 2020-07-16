# jquery.beauty.nestedfield V1.0.1

A simple jquery plugin, that allow get or set properties by name, nested properties inclusive.

## How to use 
Setting a value
```js
$.setField(object,'propNameOrPath',newValue)
```
Getting a value
```js
$.getField(object,'propNameOrPath')
```
## Example

```js
var person : {
  names: 'Adan Escobar',
  lastName: 'Escobar',
  address:{}
}
// setting new values
$.setField(person,'names','Adan Patricio')
$.setField(person,'lastName','Escobar Lagos')

// setting non exists values
$.setField(person,'address.street','Miraflores')
$.setField(person,'address.number','130')

console.log(person)

```
