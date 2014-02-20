*This repository is a mirror of the [component](http://component.io) module [yields/within](http://github.com/yields/within). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/yields-within`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# within

  `Date(now + 1e3) // => "in a second"`

## Installation

  Install with [component(1)](http://component.io):

    $ component install yields/within

## API

### within(date)

  Convert the given `Date` to a human readable string.

## Examples

```js
within(new Date - 6e4); // => ""
within(new Date); // => "just now"
within(+new Date + 1e3); // =>  "in a second"
within(+new Date + 1e3 * 5); // => "in 5 seconds"
within(+new Date + 6e4); // => "in a minute"
within(+new Date + 6e4 * 5); // => "in 5 minutes"
within(+new Date + 6e4 * 60); // => "in an hour"
within(+new Date + 6e4 * 120); // => "in 2 hours"
within(+new Date + 8.64e+7); // => "in a day"
within(+new Date + 8.64e+7 * 2); // => "in 2 days"
within(+new Date + 8.64e+7 * 7); // => "in a week"
within(+new Date + 2.63e+9); // => "in a month"
within(+new Date + 2.63e+9 * 2); // => "in 2 months"
within(+new Date + 2.63e+9 * 12); // => "in a year"
within(+new Date + 3.156e+10 * 9); // => "in 9 years"
within(+new Date + 3.156e+10 * 10); // => "in a decade"
```

## License

  MIT
