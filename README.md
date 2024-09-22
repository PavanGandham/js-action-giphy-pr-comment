# js-action-giphy-pr-comment

1. run `npm init -y` to create the package.json file.

2. run all these below command to install all the dependencies is package.json file
    `npm i @actions/core@1.10.0`
    `npm i @actions/github@5.1.1`
    `npm i @octokit/rest@20.0.1`
    `npm i giphy-api@2.0.2`

3. run `npm install @vercel/ncc`

4. now use ncc command to package the dependencies to a single file by running below command
    `ncc build index.js -o dist`
    This will create dist directory with index.js file in it. If the ncc dist folder's index.js file doesn't contains all the code dependencies then re check the steps in github official doc and re-run those commands.
