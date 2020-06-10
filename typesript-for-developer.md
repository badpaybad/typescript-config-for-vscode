https://www.typescriptlang.org/docs/handbook/react-&-webpack.html

# Create directory and sample file

                proj/
                ├─ dist/
                └─ src/
                |   └─ components/
                |   ├─ index.ts
                └─ index.html
                ├─ webpack.config.js //auto create after run command
                ├─ tsconfig.json //auto create after run command
                ├─ package.json //auto create after run command
                ├─ 
                ├─ 
                ├─ 

# Run cmds:

                npm init -y

                tsc --init

                npm install --save-dev webpack webpack-cli

                npm install --save-dev typescript ts-loader source-map-loader

## package.json
                ...
                "scripts": {
                    "test": "echo \"Error: no test specified\" && exit 1",
                    "build":"webpack webpack.config.js"   
                },   
                ...
# index.ts
alert('Hello world');

# index.html
<script src="./dist/main.js"></script>

# auto build on save install extentsion terminal-command-keys

https://medium.com/swlh/how-to-assign-terminal-commands-onto-keybindings-in-vs-code-streamlining-your-debugging-process-a42a027c38d3

Ctrl + Shift + P open file
keybindings.json

                [
                    {
                        "key": "ctrl+s",
                        "command": "-workbench.action.files.save"
                    },
                    {
                        "key": "ctrl+s",
                        "command": "terminalCommandKeys.run",
                        "args": {
                            "cmd":"npm run build"
                        }
                    }
                ]
