> The tic-tac-toe`Board` needs to know the state of each of the 9 square `components`. 
> The best approach to complete is to store the games state in the parent `Board` component instead of in each `Square` component.
> The `Board` component can tell each `Square` what to display by passing a `prop`, just like we did when we passed a `number` to each `Square`.
> To collect data from multiple children, declare the shared state in their parent component instead.
> The parent component can pass the state back down to the children by using `props`; this keeps the child components in sync with each other and with the parent component.
> This is called "lifting state up". We will remove the `constructor` from the `Square` component and set the `state` in the `Board` component instead.