<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thirdweb-dev/react](./react.md) &gt; [useCoinbaseWallet](./react.usecoinbasewallet.md)

## useCoinbaseWallet() function

Convienience hook for connecting to a wallet via Coinbase Wallet

<b>Signature:</b>

```typescript
export declare function useCoinbaseWallet(): () => Promise<{
    data?: import("wagmi-core").ConnectorData<any> | undefined;
    error?: Error | undefined;
}>;
```
<b>Returns:</b>

() =&gt; Promise&lt;{ data?: import("wagmi-core").ConnectorData&lt;any&gt; \| undefined; error?: Error \| undefined; }&gt;

a function that will prompt the user to connect their wallet via Coinbase Wallet
