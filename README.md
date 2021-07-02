# tweed


====


## Requirement

- firebase
- React.js

### Dashboard Template
- [Material Dashboard React](https://github.com/creativetimofficial/material-dashboard-react)
- [CHARTIST.js](https://gionkunz.github.io/chartist-js/index.html)

## Usage

- 開発環境の起動

```
make
```

- 開発環境に入る

```
make enter
```


- 開発環境を止める


```
make stop
```

- ローカルのデータを使ってfirebase emulatorsを起動

```
firebase emulators:start --import=<data-path> --export-on-exit
```

### dashboard

- reactの起動
```
cd dashboard
npm run start
```

## Deploy

### Firebase login

- Dockerからログインする際は`--no-localhost`オプションを利用する

```
firebase login --no-localhost
```

### dashboard deploy

- build
```
npm run build
```

- deploy

```
firebase deploy --only hosting
```

### functions deploy

```
firebase deploy --only functions:<function name>
```

