- Download and install node.js\
  node.js reference link: https://nodejs.org/en/download/

- Download and install npm or yarn, you need to install npm to download yarn\
  yarn reference link: https://classic.yarnpkg.com/lang/en/docs/install/#windows-stable \
  npm reference link: https://docs.npmjs.com/downloading-and-installing-node-js-and-npm

- Install the dependency packages\
  in the project folder navigate to directory using

```
cd .\contract_for_front_end\ui_sol_deneme2\ui_sol_deneme\sol_ui
```

install the dependencies using "npm install" or "yarn install"\
install next if needed using "npm install next" or "yarn install next"\
Clone the repo from: https://github.com/Cem-Kaya/SU_Govern

- To run the front-end:\
  in the project folder change the directory using

```
cd .\contract_for_front_end\ui_sol_deneme2\ui_sol_deneme\sol_ui
```

run the front end using "npm run dev" or "yarn dev"

- Deploying Contracts on TestNet:\
  Remix IDE was used for this.\
  Contracts are compiled in this order:

  1. token.sol
  2. creator.sol
  3. newDAO1.sol
  4. newFactory1.sol.

  Contracts are deployed in this order:

  1. creator.sol
  2. newFactory1.sol

  While deploying newFactory1.sol use the address of creator.sol.

- Connecting to Front End:\
  The files that needs modification are found in the directory below.

```
cd .\contract_for_front_end\ui_sol_deneme2\ui_sol_deneme\sol_ui\pages
```

In dao.js and index.js, the address of daoFactory should be typed in the statement where the daoFactoryContract is defined. In dao.js, line 114, and in index.js, line 180.\

**In addition to this, in order to get YK privileges, the first admin of the Top DAO needs to withdraw 1 YK token from TOP DAO. This can be done through the frontend. This is a one time case during creation. The first contract needs to be deployed using Remix IDE.**
