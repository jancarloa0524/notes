# Firestore

Here, I write as much as I can about Firebase documentation sepcifically for Firestore, which I can reference later on. Reference firestore-example in vscode in order to better understand the following. 

First things first, understand that Firebase is *modular*, so you import only the functions you need for your project. 

``` javascript
import { getFirestore, etc } from 'firebase/firestore'
```

The rest of the functions you can import will be shown.

`getFirestore()` is used to initialize the Firestore database. You can do this by creating a reference to the function, after it grabs 