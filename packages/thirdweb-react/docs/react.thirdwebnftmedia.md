<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thirdweb-dev/react](./react.md) &gt; [ThirdwebNftMedia](./react.thirdwebnftmedia.md)

## ThirdwebNftMedia variable

> This API is provided as a preview for developers and may change based on feedback that we receive. Do not use this API in a production environment.
> 

<b>Signature:</b>

```typescript
ThirdwebNftMedia: React.ForwardRefExoticComponent<ThirdwebNftMediaProps & React.RefAttributes<HTMLMediaElement>>
```

## Example


```jsx
import { ThirdwebNftMedia, useNFTCollection, useNFT } from "@thirdweb-dev/react";
export default function NFTCollectionRender() {
  const contract = useNFTCollection(<your-contract-address>);
  const { data: nft, isLoading } = useNFT(contract, 0);

  return (
    <div>
      {!isLoading && nft ? (
        <ThirdwebNftMedia metadata={nft.metadata} />
      ) : (
        <p>Loading...</p>
      )}
    </div>
  );
}
```
Use this to get the primary sales recipient of your 
