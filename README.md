# Free Time

## Mastering Javascipt Functional Programming

### Chapter 2:Thinking Functionally - A First Example

#### Doing something only once
```
const once = fn => {
	let done = false;
	return (...args) => {
		if (!done) {
			done = true;
			fn(...args);
		}
	};
};
```
