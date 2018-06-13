# create-component-lib

Create a library of React components that can be published to npm.

**Notes:**
- Uses `create-react-app` under the hood.
- Inspired from [this blog post](https://hackernoon.com/creating-a-library-of-react-components-using-create-react-app-without-ejecting-d182df690c6b).
- Currenlty tested only on Linux and Mac. 
- It's really just a [shell script](./create-component-lib). Contributions welcome!

## Usage

To create a new project, run the command:

```
npx create-component-lib my-project
```

This sets up the project inside `my-project`.

Place everything you want to publish to npm inside `src/lib`. Outside `src/lib` (but inside `src/`), you can create example web pages to test or demonstrate the usage of your components.

To start the development server (with entry point `src/index.js`), run

```
npm start
```

To transpile `src/lib` and create a build in the `dist` folder, run:

```
npm run build
```

You can then publish it to npm using:

```
npm publish
```

Note that only `README.md` and the `dist` folders are published to npm.

To learn more, see [this blog post](https://hackernoon.com/creating-a-library-of-react-components-using-create-react-app-without-ejecting-d182df690c6b) or this [sample libary](https://github.com/aakashns/simple-component-library).
