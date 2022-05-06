<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thirdweb-dev/react](./react.md) &gt; [useEditions](./react.useeditions.md)

## useEditions() function

> This API is provided as a preview for developers and may change based on feedback that we receive. Do not use this API in a production environment.
> 

Use this to get a list of NFT tokens of your ERC1155 contract.

<b>Signature:</b>

```typescript
export declare function useEditions(contract: RequiredParam<Erc1155>, queryParams?: QueryAllParams): import("react-query").UseQueryResult<{
    metadata: {
        [x: string]: import("@thirdweb-dev/sdk").Json;
        name?: string | undefined;
        description?: string | undefined;
        image?: string | undefined;
        external_url?: string | undefined;
        animation_url?: string | undefined;
        uri: string;
        id: import("@ethersproject/bignumber").BigNumber;
    };
    supply: import("@ethersproject/bignumber").BigNumber;
}[], unknown>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  contract | [RequiredParam](./react.requiredparam.md)<!-- -->&lt;Erc1155&gt; | an instace of a contract that extends the ERC1155 spec (edition, edition drop, custom contract that follows the ERC1155 spec) |
|  queryParams | QueryAllParams | <i>(Optional)</i> query params to pass to the query for the sake of pagination |

<b>Returns:</b>

import("react-query").UseQueryResult&lt;{ metadata: { \[x: string\]: import("@thirdweb-dev/sdk").Json; name?: string \| undefined; description?: string \| undefined; image?: string \| undefined; external\_url?: string \| undefined; animation\_url?: string \| undefined; uri: string; id: import("@ethersproject/bignumber").BigNumber; }; supply: import("@ethersproject/bignumber").BigNumber; }\[\], unknown&gt;

a response object that includes an array of NFTs

## Example


```javascript
const { data: editions, isLoading, error } = useEditions(<YourERC1155Instance>, { start: 0, count: 100 });
```
