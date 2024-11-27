# REQUISITOS NECESSÁRIOS

Ter os sequintes aplicativos instalados no computador

- **Docker** 
- **VSCode** 

# DEVCONTAINER

- PHP 8.3
- MYSQL 9
- PHP MyAdmin
- XDEBUG
- COMPOSER

# ACESSOS

## Apache PHP

http://localhost:81/src/teste.php

## PHP MyAdmin

http://localhost:8086

- usuario: root
- password: 123456
- database: projeto

> Você pode utilizar o banco de dados **projeto** ou criar um novo

# VSCODE

```
{
  "workbench.colorTheme": "Min Dark",
  "workbench.iconTheme": "symbols",
  "vsicons.dontShowNewVersionMessage": true,
  "editor.mouseWheelZoom": true,
  "explorer.compactFolders": false,
  "editor.rulers": [
    80,
    120
  ],
  "editor.fontFamily": "JetBrains Mono",
  "editor.fontSize": 14,
  "workbench.startupEditor": "newUntitledFile",
  "editor.renderLineHighlight": "gutter",
  "editor.fontLigatures": true,
  "workbench.editor.labelFormat": "short",
  "breadcrumbs.enabled": false,
  "editor.minimap.enabled": false,
  
  "php.suggest.basic": false, 

  "[php]": {
    "editor.formatOnSave": true,
    "editor.defaultFormatter": "bmewburn.vscode-intelephense-client",
  }

}
// sudo apt install fonts-jetbrains-mono
// sudo apt install fonts-firacode
```
