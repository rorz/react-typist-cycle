# React Typist Cycle
A React Component for 'cycling' through [React-Typist](https://github.com/jstejada/react-typist) elements.

## Install
```shell
npm install react-typist-cycle
```
## Example Usage
![example of the element in use](https://raw.githubusercontent.com/rorz/react-typist-cycle/master/demo.gif)

```jsx
<TypistCycle
  content={[
    'First typist *line*', 
    'Second line', 
    'Third line :)'
  ]}
  numberOfCycles={-1} // loop indefinitely
  segmentDelay={0.8} // stop for 0.8s at end line
  className="my-class"
/>
```
## Options
### Inherited
React Typist Cycle inherits all of [React Typist's props](https://github.com/jstejada/react-typist/blob/master/README.md#options), with the exception of `onTypingDone` (this is reserved for cycling).

### New
React Typist Cycle comes with the following props...

#### content (**REQUIRED**)

An array of string objects representing each Typist element to display.


#### numberOfCycles
*Default:* `1`


How many times to cycle through the values.
A **negative value** will cause the component to cycle through its content infinitely.
NOTE: At the end of the specified cycle amount, the component will load the first line again and remain there.


#### segmentDelay
*Default:* `0.44`

The delay at the end of each line, in seconds.

## Licence
MIT

