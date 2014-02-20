*This repository is a mirror of the [component](http://component.io) module [component/history](http://github.com/component/history). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/component-history`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# History

  Keep track of and cycle through capped history (chat messages, REPL command-lines etc).

## Installation

```
$ component install component/history
```

## API

### History(vals)

  Initialize with an array of `vals`.
  
### History#add(val)

  Add a value, for example a chat message or REPL command line.
  This method resets the history index, meaning the next call
  to `.back()` will be this latest value.

### History#prev()

  Cycle backwards through history, returning a value added by `.add()`.

### History#next()

  Cycle forwards through history, returning a value added by `.add()`.

### History#max(n)

  The maximum number of entries defaulting to `1000`.

### History#reset()

  Reset the index to the latest value.

## License

  MIT