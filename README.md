# react-learning-examples
Transitioning Vanilla HTML/JS to React

## What is the Gist of Frontend JS ?
It's pretty simple. Backend Server provides browser (client) with HTML, CSS and JS files. Browser builts the HTML Dom. Applies the CSS if present. Runs the JS script if present. And we see something.
Server provided JS files can do a bunch of stuffs. 
```
But we generally use the to update the `DOM`. Example : 
Example : document.getElementByID('body').style.background = "red"
```
React is library (just a bunch of of JS functions ) that wants us to write UI in a certain way (like a Design pattern). Folks say this particular way of designing UI helps us tame complexity better than
what we are doing above.

Challenge 3 shown here is a goldmine : `https://react.dev/learn/reacting-to-input-with-state`.

## The Design of React ? 
React wants us to be explicit about `variables` that changes in a component ( like characters `currently` typed in the textfield of website ). Then it provides us `method` that can be triggered to update those variables. We usually call these `setter methods` inside event handlers, when something changes. Invoking setter methods in turn causes react to
re-run logic in that Component/Function. Meaning, UI now displays Component having the updated state variables.
```
const [firstName, setFirstName] = useState("");
function handleFirstInputChange(e) {
    setFirstName(e.target.value);
  }
```

In HTML, we would require something like : 
```
function updateCombinedName() {
  console.log("Updating combined name...");
  const firstName = first_ta.value;
  first_name_sp.innerText = firstName;
};
```


