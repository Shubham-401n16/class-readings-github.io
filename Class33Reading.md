class-readings-33-github.io

Reference - 
https://mobx.js.org/refguide/observable-decorator.html

https://mobx.js.org/getting-started.html

Using mobx and mobx-react packages

Decorator that can be used on ES7- or TypeScript class properties to make them observable. 
The @observable can be used on instance fields and property getters. This offers fine-grained control on which parts of your object become observable.

import { observable, computed } from "mobx"

class OrderLine {
    @observable price = 0
    @observable amount = 1

    @computed get total() {
        return this.price * this.amount
    }
}

@computed
If you have decorators enabled you can use the @computed decorator on any getter of a class property to declaratively create computed properties.

import { observable, computed } from "mobx"

class OrderLine {
    @observable price = 0
    @observable amount = 1

    constructor(price) {
        this.price = price
    }

    @computed get total() {
        return this.price * this.amount
    }
}

Use the @observable decorator or observable(object or array) functions to make objects trackable for MobX.
The @computed decorator can be used to create functions that can automatically derive their value from the state.
Use autorun to automatically run functions that depend on some observable state. This is useful for logging, making network requests, etc.
Use the @observer decorator from the mobx-react package to make your React components truly reactive. 
They will update automatically and efficiently. Even when used in large complex applications with large amounts of data.
