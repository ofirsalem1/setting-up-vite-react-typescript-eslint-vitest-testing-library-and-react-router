# setting-up-vite-react-typescript-eslint-vitest-testing-library-and-react-router

course URL - https://www.youtube.com/watch?app=desktop&v=cchqeWY0Nak

1. npm create vite@latest
2. npm i -D eslint
3. npx eslint --init
4. npx install-peerdeps --dev eslint-config-airbnb.
5. change the "extends" in the .eslintrc.cjs to -> extends: ['airbnb', 'airbnb/hooks', 'plugin:react/recommended', 'plugin:@typescript-eslint/recommended'],
6. npm i -D eslint-config-airbnb-typescript.
7. Add to the "extends" in the .eslintrc.cjs -> 'airbnb-typescript'
8. change the "parserOptions" in the .eslintrc.cjs to -> parserOptions: {
   ecmaVersion: 'latest',
   sourceType: 'module',
   project: './tsconfig.json',
   },
9. change the "include" in the tsconfig.json to -> "include": [".eslintrc.cjs", "src"],
10. npm i -D prettier eslint-config-prettier eslint-plugin-prettier
11. create .prettierrc.cjs file and write inside -> module.exports = {
    trailingComma: 'es5',
    tabWidth: 2,
    semi: true,
    singleQuote: true,
    };
12. change the "plugins" in the .eslintrc.cjs to -> plugins: ['react', '@typescript-eslint', 'prettier'],
13. Add to the end of the "extends" array in the .eslintrc.cjs -> 'plugin:prettier/recommended',
