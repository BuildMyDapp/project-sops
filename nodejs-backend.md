# Build My Dapp node.js backend File Structure

## File Structure

(file names under app folder other than index.ts are written as an example)

📦backend
┣ 📂app
┃ ┣ 📂auth
┃ ┃ ┗ 📜index.ts
┃ ┣ 📂controller
┃ ┃ ┣ 📂adminController
┃ ┃ ┃ ┣ 📜updatePassword.ts
┃ ┃ ┃ ┗ 📜updateUsername.ts
┃ ┃ ┗ 📂nftController
┃ ┃ ┃ ┗ 📜createNft.ts
┃ ┣ 📂db
┃ ┃ ┗ 📜index.ts
┃ ┣ 📂model
┃ ┃ ┣ 📜adminModel.ts
┃ ┃ ┗ 📜nftModel.ts
┃ ┣ 📂routes
┃ ┃ ┗ 📜router.ts
┃ ┣ 📂schema
┃ ┃ ┣ 📜adminSchema.ts
┃ ┃ ┗ 📜nftSchema.ts
┃ ┗ 📂validators
┃ ┃ ┣ 📜customValidator.ts
┃ ┃ ┗ 📜tokenValidator.ts
┣ 📜.gitignore
┣ 📜environment.ts
┣ 📜index.ts
┣ 📜package-lock.json
┣ 📜package.json
┗ 📜tsconfig.json

## Folders purpose:

### Auth

For login authentication

### Schemas

For mongo schemas

### Models

For writing database methods like find(), create(), update() etc using mongo model

### Routes

Create api routes here

### Controllers

Middle man between router and model, here we can destructure ctx object and send necessary data to model function or write some other logic need to be processed before querying database

### Validator

Here create validator files to write field validation functions

## Naming Conventions:

File and folder name should be in small letters
variable names in camel case
Function names in camel case
Classes/mongoose model names start with capital letter
