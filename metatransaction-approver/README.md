# MetaCredits MetaTx Approver Service

This service can be used as a template for Dapp Developers who have been funded through the MetaCredits smart contracts to approve and forward on metatransactions from their users (typically via their Dapp) on to a relayer.

The initial service was created to run on a serverless AWS lambda instance but it can be adapted in many ways. To run the service locally, first setup a `secret.env` file with a `SIGNER_PRIV_KEY` and input the private key you wish to use as the approver.

```
SIGNER_PRIV_KEY=38a0f921a9ec060639ec8395eb618487962284274ad9ace6d5b60facdb72e108
```

After this file is in place, run `npm run local` to start a signing service on your machine at PORT 3010