# Issue: vue-hot-reload-api mixins

## Description
### Version
* vue-hot-reload-api 2.2.0

### Steps to reproduce
Try comment/uncomment:

```javascript
// src/mixins/my-mixin.vue#L20-22
foo(){
  console.log('bar')
}
```

### What is expected ?
I expect that `HelloWorld` component will have his `data.internalData` set to `'Some stuff'`.

### What is actually happening?
When a [Mixin](https://vuejs.org/v2/guide/mixins.html) is updated the Component that use it lost his initial `data`.

## Setup
`yarn install`

## Serve
`yarn serve`
