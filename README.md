# vue1

vue practice

## What is Vue?

### MVVM, specifically view model is where Vue lies in and through dom listeners and data bindings, the dom understands any inputs from the users and delivers to plain javascript. Also, updating the data from data bindings from plain javascript objects.

## what is difference betwen global and local component?

### global component is done by Vue.component() from outside whereas the local component can be implemented within vue instance with components options. Generally, build local components a lot for spa but global components can be useful when creating some higher level component.

## the relationship between component and instance?

### instance can be created and the local components within that instance can only be used in that specific component. Therefore, whenever you want to share some components, put that in global component instead of putting it on every instance you create.

## Difference between computed and methods?

### Computed options has its functions cached and stores the result of the functions in cache unless the dependent input of the function changes whereas methods always run whenever there re-render occurs.

## Difference between watch and computed?

### Those two bascially behave the same except for their programming paradigms. Watch is imperative programming which means commands need to be there to reflect actions on data changes whereas computed is declarative programming. More than often times, watch is imperative and repetitive so prefer to use computed, also with the benefit of caching.
