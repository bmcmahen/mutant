
# mutant

  a simple api for the MutationObserver

## Installation

  Install with [component(1)](http://component.io):

    $ component install bmcmahen/mutant

## API

```javascript
var editable = document.getElementById('editable');
var mutant = require('mutant')(editable, 'p');

mutant.on('added', function(el){
  console.log('added', el);
});

mutant.on('removed', function(el){
  console.log('removed', el);
});

mutant.disconnect();
```

## License

  MIT
