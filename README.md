# vue1

vue practice

## What is Vue?

### MVVM, specifically view model is where Vue lies in and through dom listeners and data bindings, the dom understands any inputs from the users and delivers to plain javascript. Also, updating the data from data bindings from plain javascript objects.

## what is difference betwen global and local component?

### global component is done by Vue.component() from outside whereas the local component can be implemented within vue instance with components options. Generally, build local components a lot for spa but global components can be useful when creating some higher level component.

## the relationship between component and instance?

### instance can be created and the local components within that instance can only be used in that specific component. Therefore, whenever you want to share some components, put that in global component instead of putting it on every instance you create.
