<img src=".assets/whistle_dark.svg" width="100px" align="left" style="padding: 10px;" />
 
# Whistle (legacy)

Legacy whistle code in typescript

## CLI

### Installing

```base
$ deno install whistle -A -f https://raw.github.com/whistle-lang/whistle/master/cli/whistle.ts
```

### Usage

```
$ whistle -h
```

### Example

```
$ whistle compile examples/HelloWorld.whi > HelloWorld.js
```

the file `HelloWorld.js` should now look like this:

```js
function Log(text){console.log(text);}(() => {Log("Hello World");})();
```

and running:

```
$ whistle run examples/HelloWorld.whi
```

will produce this output:

```
Hello World
```
