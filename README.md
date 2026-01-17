# react-learning-examples
Transitioning Vanilla HTML/JS to React

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


