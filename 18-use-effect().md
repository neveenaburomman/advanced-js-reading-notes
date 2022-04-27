##  useEffect

## What does useEffect do?

By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed
(we’ll refer to it as our “effect”), and call it later after performing the DOM updates. In this effect, we set the document title, but we could also perform 
data fetching or call some other imperative API.


## Why is useEffect called inside a component? 

Placing useEffect inside the component lets us access the count state variable (or any props) right from the effect. We don’t need a special API to
read it — it’s already in the function scope. Hooks embrace JavaScript closures and avoid introducing React-specific APIs where JavaScript already provides a solution.


## Does useEffect run after every render?

Yes! By default, it runs both after the first render and after every update. Instead of thinking in terms of “mounting” and “updating”,
you might find it easier to think that effects happen “after render”. React guarantees the DOM has been updated by the time it runs the effects.


![image](https://user-images.githubusercontent.com/90922969/165599562-66cc3ede-843d-4b9e-a124-9ae707640a95.png)

We declare the count state variable, and then we tell React we need to use an effect. We pass a function to the useEffect Hook. This function we pass is our effect.
Inside our effect, we set the document title using the document.title browser API. We can read the latest count inside the effect because it’s in the scope of our 
function. 

When React renders our component, it will remember the effect we used, and then run our effect after updating the DOM. This happens for every render, including the
first one.


 useEffect is going to be different on every render. This is intentional. In fact, this is what lets us read the count value from inside the effect without
 worrying about it getting stale. Every time we re-render, we schedule a different effect, replacing the previous one. 
 In a way, this makes the effects behave more like a part of the render result — each effect “belongs” to a particular render

