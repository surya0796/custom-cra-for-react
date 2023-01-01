Steps to setup React with TS using webpack
1. Create .gitignore file and folders named build and src. Aldo create index.html file and div id="root" element inside body tag.
2. Enter "npm init --y" inside terminal, which creates package.json file.
3. Add build and node_modules name inside .gitignore file 
4. Install react and react-dom using "npm add react react-dom".
5. Now install "npm add -D typescript @types/react @types/react-dom" dev dependencies.
6. Create tsconfig.json file and add "{
                                    "compilerOptions": {
                                        "target": "ES5" /* Specify ECMAScript target version: 'ES3' (default), 'ES5', 'ES2015', 'ES2016', 'ES2017', 'ES2018', 'ES2019', 'ES2020', or 'ESNEXT'. */,
                                        "module": "ESNext" /* Specify module code generation: 'none', 'commonjs', 'amd', 'system', 'umd', 'es2015', 'es2020', or 'ESNext'. */,
                                        "moduleResolution": "node" /* Specify module resolution strategy: 'node' (Node.js) or 'classic' (TypeScript pre-1.6). */ /* Type declaration files to be included in compilation. */,
                                        "lib": [
                                        "DOM",
                                        "ESNext"
                                        ] /* Specify library files to be included in the compilation. */,
                                        "jsx": "react-jsx" /* Specify JSX code generation: 'preserve', 'react-native', 'react' or 'react-jsx'. */,
                                        "noEmit": true /* Do not emit outputs. */,
                                        "isolatedModules": true /* Transpile each file as a separate module (similar to 'ts.transpileModule'). */,
                                        "esModuleInterop": true /* Enables emit interoperability between CommonJS and ES Modules via creation of namespace objects for all imports. Implies 'allowSyntheticDefaultImports'. */,
                                        "strict": true /* Enable all strict type-checking options. */,
                                        "skipLibCheck": true /* Skip type checking of declaration files. */,
                                        "forceConsistentCasingInFileNames": true /* Disallow inconsistently-cased references to the same file. */,
                                        "resolveJsonModule": true
                                        // "allowJs": true /* Allow javascript files to be compiled. Useful when migrating JS to TS */,
                                        // "checkJs": true /* Report errors in .js files. Works in tandem with allowJs. */,
                                    },
                                    "include": ["src/**/*"]
                                    }" inside that file.
7. Create App.tsx and index.tsx inside src folder and write an entry component inside App.tsx and inject that function inside index.html using ReactDOM method.
8. Install babel and its dev dependencies using "npm add -D @babel/core @babel/preset-env @babel/preset-react @babel/preset-typescript"