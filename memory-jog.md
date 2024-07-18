link to source filder:

/c/Users/glads/Downloads/COMPONENTS-RENDER-OTHER-COMPONENTSReturningAnotherComponent/return-another-component

link to AI:

https://chatgpt.com/c/14426d70-9262-425d-95e0-ff40af8c4e99


### COMPONENTS RENDER OTHER COMPONENTS

**Returning Another Component**

As we’ve seen before, each React component is responsible for one piece of the interface. As the application grows in complexity, components need to be able to interact with each other to support the features needed.

So far, we’ve explored components that return JSX elements, such as:

```
function PurchaseButton() {
  return <button onClick={()=>{alert("Purchase Complete")}}>Purchase</button>
}

```
In this example, the React component is not interacting with other components. However, you can have components interact with each other by passing information or even returning other components.

```
function PurchaseButton() {
  return <button onClick={()=>{alert("Purchase Complete")}}>Purchase</button>
}

function ItemBox() {
  return (
    <div>
      <h1>50% Sale</h1>
      <h2>Item: Small Shirt</h2>
      <PurchaseButton />
    </div>
  );
}

```
In the above example, ItemBox returns an instance of PurchaseButton. This is an example of how a component can reference other components!

### Instructions
View Profile.js and observe how the Picture component is referenced inside of the Profile component. Picture is responsible for a piece of Profile.

Together, we exported only the Profile component to be rendered.
