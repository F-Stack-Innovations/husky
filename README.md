# Learn to used husky

(source)[https://github.com/typicode/husky]

## install

```sh
git init
npm init -y

npx husky-init && npm install
```

## Créer une commande

```sh
npx husky add .husky/commit-msg 'echo pouet'
```

Contenu du fichier

```sh
#!/usr/bin/env sh
. "$(dirname -- "$0")/_/husky.sh"

echo pouet
```

si on relance à nouveau la même commande, nous obtiendrons ce fichier

```sh
#!/usr/bin/env sh
. "$(dirname -- "$0")/\_/husky.sh"

echo pouet
echo pouet2
```
