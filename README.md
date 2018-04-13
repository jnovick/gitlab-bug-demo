This project is meant to demonstrate the issue here: https://github.com/jdalrymple/node-gitlab-api/issues/66

Steps to reproduce this project:
1. Create a project via create-react-app.
    ``` bash
      npx create-react-app test
    ```
1. Install `node-gitlab-api` or `gitlab` npm module
    ``` bash
      npm install --save gitlab
    ```
1. Import `gitlab` anywhere in the project
1. Now you can see that `npm start` works but `npm build` doesn't.
    ``` bash
      npm build # Doesn't work
      npm start # Works
    ```

These aren't the exact steps I used. I actual had already globally installed `create-react-app` via yarn and I performed steps 3 and 4 with yarn as well, but these steps will produce the same result.