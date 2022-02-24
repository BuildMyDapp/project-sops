# Build My Dapp React frontend File Structure

## File Structure

(file names under app folder other than index.ts are written as an example)

📦frontend
┣ 📂public
┣ 📂src
┃ ┣ 📂assets
┃ ┣ 📂components
┃ ┃ ┣ 📂common
┃ ┃ ┣ 📜footer.tsx
┃ ┃ ┗ 📜navbar.tsx
┃ ┣ 📂helpers
┃ ┃ ┗ 📜index.ts
┃ ┣ 📂interfaces
┃ ┃ ┗ 📜types.ts
┃ ┣ 📂pages
┃ ┃ ┣ 📂aboutUs
┃ ┃ ┗ 📂login
┃ ┣ 📂services
┃ ┃ ┗ 📜networkService.ts
┃ ┣ 📂store
┃ ┃ ┣ 📂redux
┃ ┃ ┃ ┣ 📂slices
┃ ┃ ┃ ┃ ┗ 📂nftSlices
┃ ┃ ┃ ┃ ┃ ┗ 📜createNftSlice.ts
┃ ┃ ┃ ┗ 📜parentReducer.ts
┃ ┃ ┣ 📂saga
┃ ┃ ┃ ┣ 📜nftSaga.ts
┃ ┃ ┃ ┗ 📜rootSaga.ts
┃ ┃ ┗ 📜store.ts
┃ ┣ 📜app.tsx
┃ ┗ 📜index.ts
┣ 📜pacakge-lock.json
┣ 📜package.json
┗ 📜tsconfig.json

## Folders purpose:

### Assets

The folder will contain all the images and if videos inside their suitable directory

### Components

The folder will contain all the components.

#### \_common

The folder will contain components which are used more than once. Like a button. If a button with the same properties is used multiple times then we will create that component inside this directory.

### Helpers

The folder will contain functions which are being used multiple times or it can also contain a file with which you are unsure of what to do. Cause sometimes working we create a function which we will need later so we can create it inside helper directory as it will help us later.

### Interfaces

This folder is specifically for typescript. It will contain types which are being use more than one time. For example if we are passing props to a single component then we will create those types inside that component file not here. But if the same props are being passed to multiple components multiple times than we create those types inside this directory.

### Pages:

The directory will contain an index.tsx file where all the pages will be imported and then exported so that it gets easy for developers to import all the pages from one file.

### Redux:

web3Connect: The directory have a web3ConnectSlice.ts file where we will have our web3Connect logic
We will have different folders for different types of logics. If there was authentication then we would have created an Authentication folder and inside authSlice.ts file which would have our authentication logic.  
The parentReducer.ts will be our reducer file
The store.ts file will be our store

### Services

This folder will contain those files which belong to some kind of service. For example if we are using firebase service then this folder would have a firebase.ts file.

## Naming Conventions:

1.React component folder will have camelCase naming convention
