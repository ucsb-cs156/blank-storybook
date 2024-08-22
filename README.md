# blank-storybook
A blank storybook, in CS156 house style (in frontend directory)

This repo contains a minimal React frontend in CS156 house style:
* Frontend is in a directory called `frontend`, and was created using:
  
  ```
  npx create-react-app frontend
  ```
* Then we added storybook using 
  ```
  npx storybook@latest init
  ```

We then made minimal changes to set up the repo for access to Chromatics online tools for Storybook, 
including CI/CD support using Github Actions.

* <https://www.chromatic.com/docs/github-actions/>

In addition to following those instructions, we also:

* Added a `.env` file at top level to the `.gitignore`
* Set up the `chromatic` command in `package.json` to use the environment variable `CHROMATIC_PROJECT_TOKEN` for the `npm run chromatic` command.

Using the `npm run chromatic` command, we obtained this published storybook:
* <https://66c68be66b674682376d8e52-yigcpwfsvt.chromatic.com/>