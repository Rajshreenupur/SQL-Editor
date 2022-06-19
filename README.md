# SQL Editor as a part of Atlan Assignment

EdiQL fulfils all the requirements that were mentioned by team Atlan.

You can run different queries on the table and view data of each table. The queries are : ALTER TABLE, ANALYZE, CREATE VIEW, DROP TABLE

Task : Create a SQL editor view where your users can query easily on a table using SQL, and see the results.

## Production Build

https://rajshree-sql-editor.netlify.app/

## Data

I have coverted the csv files provided by team Atlan to JSON format and thus loaded it anytime a query is demanding the data to be retrieved from the file.

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

<img width="1440" alt="ss of performance.png" src="https://github.com/Rajshreenupur/SQL-Editor/blob/master/images/ss%20of%20performance.png">

<img width="1440" alt="ss of performance1.png" src="https://github.com/Rajshreenupur/SQL-Editor/blob/master/images/ss%20of%20performance1.png">

### Steps taken to Optimize

1. There was render blocking javascript for google font causing delay, used method mentioned [here](https://pagespeedchecklist.com/asynchronous-google-fonts) to overcome the problem.

2. Import for `react-ace` editor was long tasks running during page load, Converted it to Lasy loaded component using `React.lazy()` for code-splitting and delaying it's loading.

3. Only importing used Module in a component from library rather than importing whole library.

## create-react-app

This project was bootstrapped with [Create React App](https://github.com/facebookincubator/create-react-app). You can find more information on how to perform common tasks [here](https://github.com/facebook/create-react-app/blob/master/packages/cra-template/template/README.md).

## Screenshots

<img width="1439" alt="s1.png" src="https://user-images.githubusercontent.com/56116708/132289773-32250d77-3203-4d7b-b4a6-751672a45957.png">

<img width="1439" alt="s2.png" src="https://user-images.githubusercontent.com/56116708/132289814-0c3f2601-dc23-43d8-9518-e41beaa05ba2.png">

<img width="1440" alt="s3.png" src="https://user-images.githubusercontent.com/56116708/132289888-05f87a54-f461-4df8-8912-e9e58d70b462.png">

<img width="1427" alt="s4.png" src="https://user-images.githubusercontent.com/56116708/132290058-f599c2f4-577e-4efa-b516-4f7814c82413.png">

<img width="1440" alt="s5.png" src="https://user-images.githubusercontent.com/56116708/132290096-71c22dc1-b534-4ee8-b312-db5ab2a9f4af.png">
