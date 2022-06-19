# SQL Editor as a part of Atlan Assignment

EdiQL fulfils all the requirements that were mentioned by team Atlan.

You can run different queries on the table and view data of each table. The queries are : ALTER TABLE, ANALYZE, CREATE VIEW, DROP TABLE

Task : Create a SQL editor view where your users can query easily on a table using SQL, and see the results.

## Production Build

https://rajshree-sql-editor.netlify.app/

## Requirements

- yarn

## Libraries Used

- [React](https://reactjs.org/)
- [Material-UI](https://material-ui.com/)
- [React-Ace](https://github.com/securingsincity/react-ace)

## How to run:

1. [Download](https://github.com/sagarchoudhary96/react-sql-editor/archive/refs/heads/master.zip) or [Clone](https://github.com/sagarchoudhary96/react-sql-editor.git) the Repository.
2. Run `yarn install` to install the project dependencies.

3. Run `yarn start` to run the app in development mode.

4. App can be seen at: `http://localhost:3000/`

## Page Load Time

Page Load TIme has been calculated by using the [Lighthouse Tool](https://developers.google.com/web/tools/lighthouse).

<img width="1440" alt="ss of performance.png" src="https://user-images.githubusercontent.com/56116708/132289454-da310ada-4325-43e6-93a6-db99486623f8.png">

### Steps taken to Optimize

1. There was render blocking javascript for google font causing delay, used method mentioned [here](https://pagespeedchecklist.com/asynchronous-google-fonts) to overcome the problem.

2. Import for `react-ace` editor was long tasks running during page load, Converted it to Lasy loaded component using `React.lazy()` for code-splitting and delaying it's loading.

3. Only importing used Module in a component from library rather than importing whole library.

## create-react-app

This project was bootstrapped with [Create React App](https://github.com/facebookincubator/create-react-app). You can find more information on how to perform common tasks [here](https://github.com/facebook/create-react-app/blob/master/packages/cra-template/template/README.md).
