# Instalación de CommitLint

npm i -D @commitlint/{cli,config-conventional}

# Crea un archivo commitlint.config.js en la raiz del proyecto con el siguiente contenido:

module.exports = {extends: ['@commitlint/config-conventional']}

# Instalación de Husky

npm i -D husky

# Añadir husky hook

npx husky install

# Añadir hook de commit-msg

npx husky add .husky/commit-msg 'npx --no-install commitlint --edit $1'
