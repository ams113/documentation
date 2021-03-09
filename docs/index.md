# Steps Testing React 17
Documentation and libraries to carry out a test environment in our React project

## Dependencies React 17
Installation npm or yarn packages

* `npm install --save-dev @wojtekmaj/enzyme-adapter-react-17` OR ` yarn add --dev @wojtekmaj/enzyme-adapter-react-17` - enzyme-adapter-react-17
* `npm install --save-dev enzyme-to-json` OR `yarn add --dev enzyme-to-json` - enzyme-to-json
* `npm install "@testing-library/react-hooks" --save-dev` OR `yarn add --dev @testing-library/react-hooks` - react-hooks-testing-library


## Documentation
* **Jest** - JavaScript Testing Framework, It's de runner. **Site:**  [jestjs.io](https://jestjs.io/).
* **Enzyme** - JavaScript Testing utility that makes it easier to test your Components. **Site:**  [enzymejs.github](https://enzymejs.github.io/enzyme/).
* **enzyme-adapter-react-17** - Provisional adapter react 17 to works enzyme. **Site:** [adapter](https://github.com/wojtekmaj/enzyme-adapter-react-17).
* **enzyme-to-json** - Convert Enzyme wrappers to a format compatible with Jest snapshot testing. **Site:** [adapter](https://github.com/adriantoine/enzyme-to-json).
* **React Hooks Testing Library** - Simple and complete React hooks testing utilities that encourage good testing practices.. **Site:** [react-hooks-testing-library.com](https://react-hooks-testing-library.com/).


## Project layout
    ...                     # Other proyect folder and other files.         
    src/                    # Components and props
        components/     
        hooks/          
        test/               # Folder test files
        setupTests.js       # Initializing Test Environment
        ...                 # Other foldesrs and other files.


## Configuration
Example configuration test environment in *setupTests.js*

```
import Enzyme from 'enzyme';
import Adapter from '@wojtekmaj/enzyme-adapter-react-17';

Enzyme.configure({ adapter: new Adapter() });
import {createSerializer} from 'enzyme-to-json';
 
expect.addSnapshotSerializer(createSerializer({mode: 'deep'}));

```

## Commands

* `yarn test` - Run suite test

# React Hooks
Documentation and libraries to carry out a test environment in our React project

