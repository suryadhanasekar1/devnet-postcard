# Devnet Postcard

Write a short note, stamp it, and send it as a real transaction on Solana devnet. The app creates a disposable wallet in the browser, uses Solana's Memo program, shows a confirmation receipt and Explorer link, and displays recent postcards in a live mailbox.

## Live transaction proof

[View a confirmed postcard on Solana Explorer](https://explorer.solana.com/tx/2CLqD5C6nsb7CKkj5nDp3cFrqo9zcNTUuW9wPh4ZmFj9cFoZWHDRv7HGWwWPiDaty93RUHJDjtBGm6dY4cGvcXe9?cluster=devnet) — message: “hello solana”, sender label: “surya”.

## Run locally

From this folder, run `python3 -m http.server 5173` and open `http://127.0.0.1:5173` in a browser. Generate a wallet, fund its displayed address with devnet SOL from [Solana Faucet](https://faucet.solana.com/), write a note, and click **Stamp & send**. The receipt links to the confirmed transaction.

The wallet exists only in the current browser tab. Keep the tab open until the send completes. This project uses the already deployed Memo program; it does not include a custom Solana program. Devnet can be reset, so it is not permanent storage.

Built during a Solana workshop using the [brimigs/workshop](https://github.com/brimigs/workshop) development scaffold.
