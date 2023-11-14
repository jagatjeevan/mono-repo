## MonoRepo

This repo/project/folder is an attemp to understand monorepo which is being used widely in recent frontend world. This would allow you to:

- Clone a single repo and have all the relevant projects/application of frontend in a single go.
- Easier referring to the libraries in development lifecycle. No need to deploy to test the application.

For more detail understanding on mono-repo follow this [link](https://jagatjeevan.vercel.app/blogs/mono-repo)

## Other good things done here

- [Prettier](https://prettier.io/): Auto-formats your code and have consistency across the project.

### VSCode settings

If you are using VSCode, you might integrate prettier to have a better developer experience by

- Install plugin for [VSCode](https://github.com/prettier/prettier-vscode)
- Create a file in the root folder `.vscode/settings.json` and paste the below code

```
{
  "eslint.options": {
    "configFile": ".eslintrc.json"
  },
  "eslint.validate": ["javascript", "javascriptreact"],
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  },
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.formatOnSave": true
}
```

Note: I am using react in the project, there might be few lines wrt react code, feel free to change as per your codebase.
