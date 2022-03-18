# 🚀 Quick Start

📄 Clone or fork `vestingVault-dapp`:

```sh
git clone https://github.com/menezesphill/vestingVault-dapp.git
```

💿 Install all dependencies:

```sh
cd vestingVault-dapp
yarn install
```

🚴‍♂️ Run your App:

```sh
yarn run serve
```

A static server will start and be served at http://localhost:9011

🚚 Building the project for distribution:

```sh
yarn run build
```

# 🧰 Making changes to the dApp

We use [Browserify](https://browserify.org/) to require('modules') on our browser. So, in order to modify this dApp you need to:

💿 Install Browserify:

```sh
npm install -g browserify
```

Any time you edit [contract.js](https://github.com/menezesphill/vestingVault-dapp/blob/master/src/contract.js), it is necessary to bundle the new edited file with all your dependencies by using:

```sh
browserify contract.js -o bundle.js
```

And reload the dApp by using `Ctrl` + `Shift` + `R` to see the changes reflect at http://localhost:9011
