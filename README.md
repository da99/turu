# turu
It let's you fly around the DOM. (In other words, you won't need it. But, I do.)

# NOTE:

It's not ready yet.

# Example:

```javascript
<script src="../path/to/turu.js"></script>

var on = Turu.on;

on('load', ['news', 'good'], {hasClass: 'append'}, function (data) {
  return someValueForFurtherProcessing;
});

on('load', ['news', 'bad'], function (data) {
  return undefined;       // ... to stop processing
});

var is_empty_string = function (data) {
  if (!_.isString(data))
    return undefined;     // ... to skip this;
  return _.isEmpty(data); // A boolean value has to be returned.
};

on(['news', 'bad'], is_empty_string, function (data) {
    // ...do your data processing
});

```

# Useless Facts:
Named after a [Jonny Quest episode](http://jqdb.wikia.com/wiki/Turu_the_Terrible)
because you can travel pretty far if you rode on a pteranodon.