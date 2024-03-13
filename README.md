# sf-crypto-demo
## Project Objective: Integrate an API call within a Salesforce flow.

### Data Model:

- **Crypto Wallets**: Custom objects representing user wallets.

- **Coins**: Custom objects representing cryptocurrency holdings. Coins must be linked to a Crypto Wallet (Master-Detail relationship).

- **Coin Price Table**: A single custom object holding a list of available coins with details like symbol and price.

### Functionality:

- A flow updates Coin information using an API call. This update applies to all entries in the Coin Price Table.
- Existing Coins in user wallets are then synchronized with the updated Coin Price Table. This eliminates redundant API calls for the same coin data.

### Assumptions:

- There is only one Coin Price Table in the Salesforce instance.

# Salesforce Objects
1. Person Account
2. Crypto Wallet (Custom)
3. Coin (Custom)
4. Coin Price Table (Custom)

# Salesforce Flows In Use
