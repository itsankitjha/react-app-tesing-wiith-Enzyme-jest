## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.


-------------------------------------------------------------------------

1. Installation
Let’s start by installing all the necessary libraries. Open the application and console using yarn or npm to install Jest, Enzyme, and some additional plugins.

If you created your app with create-react-app you don’t have to install Jest, it’s already there.

### yarn add enzyme enzyme-adapter-react-16 react-test-renderer
yarn add enzyme-to-json
If you don’t have Jest in your project yet you can install it with the following command:

### yarn add jest
When it’s ready, we can open the application code and start setting up the testing environment.

2. Setting test file
Please open the setupTest.js file, where we will need to configure the adapter to use Enzyme in the Jest environment properly.

import { configure } from "enzyme";
import Adapter from "enzyme-adapter-react-16";
configure({ adapter: new Adapter() });
When that’s ready and saved, the next step will be to think about test cases.
