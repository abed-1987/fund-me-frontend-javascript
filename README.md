
# Quickstart

1. Clone the repo

```
git clone https://github.com/PatrickAlphaC/html-fund-me-fcc
cd html-fund-me-fcc
```

2. Run the file.

You can usually just double click the file to "run it in the browser". Or you can right click the file in your VSCode and run "open with live server".

Optionally:

If you'd like to run with prettier formatting, or don't have a way to run your file in the browser, run:
```
yarn
yarn http-server
```

And you should see a small button that says "connect".

![Connect](connect.png)

Hit it, and you should see metamask pop up.

# Execute a transaction

If you want to execute a transaction follow this:

Make sure you have the following installed:

1. You'll need to open up a second terminal and run:

```
git clone https://github.com/abed-1987/fund-me-hardhat.git
cd fund-me-hardhat-main
yarn
yarn hardhat node
```

This will deploy a sample contract and start a local hardhat blockchain.

2. Update your `constants.js` with the new contract address.

In your `constants.js` file, update the variable `contractAddress` with the address of the deployed "FundMe" contract. You'll see it near the top of the hardhat output.

3. Connect your [metamask](https://metamask.io/) to your local hardhat blockchain.

In the output of the above command, take one of the private key accounts and [import it into your metamask.]

Additionally, add your localhost with chainid 31337 to your metamask.

4. Reserve the front end with `yarn http-server`, input an amount in the text box, and hit `fund` button after connecting

