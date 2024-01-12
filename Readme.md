
## Pet store API test 
Check CRUD process in http://localhost:8080/api/v3/pet via API

## Requerimients

 - Make sure you have Node.js installed on your machine. You can download it from https://nodejs.org/.
 - Make sure you have docker installed  on your machine. You can get it from https://docs.docker.com/get-docker/

## Installation

- Clone this repository to your local machine:

```
git clone https://github.com/rommelayala/wefox.git
```

- Navigate to the project directory:

```
cd wefox
```

- Install the necessary dependencies using the following command:

```
npm install
```

# Important 
YOU NEED EXECUTE "pet store API" LOCALLY BEFORE EXECUTE ALL TESTS 

1.- Go to swagger-petstore-master folder

2.- Execute (this command Will Pull docker) 
```
docker pull swaggerapi/petstore3:unstable
```
3.- Execute (this command Will run container)
```
docker run  --name swaggerapi-petstore3 -d -p 8080:8080 swaggerapi/petstore3:unstable
````

## Running Tests
- To run the tests, use the following command:

```
npx cypress run --spec "cypress/e2e/features/petstore.feature"
```

This command will execute the tests defined in the petstore.feature file located in the cypress/e2e/features/ folder.

## Customizing Tests
If you want to add or modify tests, you can do so by editing the feature files in the cypress/e2e/features/ folder. Ensure you follow the Cucumber format when writing your scenarios.

## Development Environment
```
Cypress: ^10.11.0
Cucumber Preprocessor: ^19.1.0
ESBuild Preprocessor: ^2.2.0
Make sure to have these dependencie
```
