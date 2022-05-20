<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thirdweb-dev/react](./react.md) &gt; [useClaimNFT](./react.useclaimnft.md)

## useClaimNFT() function

> This API is provided as a preview for developers and may change based on feedback that we receive. Do not use this API in a production environment.
> 

Use this to mint a new NFT on your [DropContract](./react.dropcontract.md)

<b>Signature:</b>

```typescript
export declare function useClaimNFT<TContract extends DropContract>(contract: RequiredParam<TContract>): import("react-query").UseMutationResult<ClaimNFTReturnType<TContract>, unknown, ClaimNFTParams<TContract>, unknown>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  contract | [RequiredParam](./react.requiredparam.md)<!-- -->&lt;TContract&gt; | an instace of a [DropContract](./react.dropcontract.md) |

<b>Returns:</b>

import("react-query").UseMutationResult&lt;[ClaimNFTReturnType](./react.claimnftreturntype.md)<!-- -->&lt;TContract&gt;, unknown, [ClaimNFTParams](./react.claimnftparams.md)<!-- -->&lt;TContract&gt;, unknown&gt;

a mutation object that can be used to mint a new NFT token to the connected wallet

## Example


```jsx
const Component = () => {
  const {
    mutate: claimNft,
    isLoading,
    error,
  } = useClaimNFT(DropContract);

  if (error) {
    console.error("failed to mint nft", error);
  }

  return (
    <button
      disabled={isLoading}
      onClick={() => claimNft({to: "0x...", quantity: 1})}
    >
      Mint!
    </button>
  );
};
```
