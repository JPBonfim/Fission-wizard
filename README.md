# Fission Wizard #

The **Fission Wizard** is a tool to help **deploy and destroy multiple [fission]( https://fission.io/) functions simultaneously**.
To use it, run the script in the folder that contains the functions.

For the tool to work, each function must be inside a folder that contains another folder with the deployment files. 
(As in the documentation: https://fission.io/docs/usage/spec/)

**Example:**
```
└── functions
    ├── function-1
    │  ├── main.py
    │  ├── src/
    │  └── specs
    │
    ├── function-2
    │  ├── main.py
    │  └── specs
    │
    ├── function-3
    │  ├── main.py
    │  ├── test.sh
    │  ├── src/
    │  └── specs
```

### Requirements ###

The only requirement is to have the Fission CLI installed.

### Instalation ###

You can just clone the repository and run the script directly in the folder with the fissions:

```shell
bash fission-wizard.sh
```

Or you can add the script to the path, so you can call it from any folder:

```shell
chmod +x fission-wizard
sudo cp fission-wizard /usr/local/bin/
```