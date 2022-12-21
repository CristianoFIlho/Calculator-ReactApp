# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Deploy

https://calculator-react-app-two.vercel.app/

![Calculator-ReactApp](https://user-images.githubusercontent.com/54041918/175449265-d84595e6-613b-4994-ad55-366ab8f9f5ee.gif)


## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.



### `Dockerfile properts`

```docker
FROM node:14

WORKDIR /app

COPY package.json .
RUN npm install

COPY . .

CMD ["npm", "start"]

```

### `Docker build`

```docker
   docker build -t calculator-app .
```

### `Docker run`

```docker
docker run -p 3000:3000 calculator-app
```