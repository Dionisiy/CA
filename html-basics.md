# Redux FAQ

## Table of Contents

* **General** - [When should I use Redux?](#general-when-to-use)  - [Can Redux only be used with React?](#general-only-react)  - [Do I need to have a particular build tool to use Redux?](#general-build-tools) - **Reducers** - [How do I share state between two reducers? Do I have to use combineReducers?](#reducers-share-state)  - [Do I have to use the switch statement to handle actions?](#reducers-use-switch) - **Organizing State** - [Do I have to put all my state into Redux? Should I ever use React's setState\(\)?](#organizing-state-only-redux-state)  - [Can I put functions, promises, or other non-serializable items in my store state?](#organizing-state-non-serializable)  - [How do I organize nested or duplicate data in my state?](#organizing-state-nested-data) - **Store Setup** - [Can or should I create multiple stores? Can I import my store directly, and use it in components myself?](#store-setup-multiple-stores)  - \[Is it OK to have more than one middleware chain in my store enhancer? What is the difference between next and dispatch in a middleware function?\]\(


