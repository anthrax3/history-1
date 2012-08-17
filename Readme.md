
# History

  Keep track of and cycle through history, for example chat messages.

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

### History#back()

  Cycle backwards through history, returning a value added by `.add()`.
  When the end of history is reached `undefined` is returned. 

### History#back()

  Cycle forwards through history, returning a value added by `.add()`.
  When the end of history is reached `undefined` is returned. 

### History#max(n)

  The maximum number of entries defaulting to `1000`.

### History#reset()

  Reset the index to the latest value.

## License

  MIT