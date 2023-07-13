# Instalación de CommitLint

npm i -D @commitlint/{cli,config-conventional}

# Create a .commitlintrc.json file

# Instalación de Husky

npm i -D husky

# Añadir husky hook

npx husky install

# Añadir hook de commit-msg

npx husky add .husky/commit-msg 'npx --no-install commitlint --edit $1'
