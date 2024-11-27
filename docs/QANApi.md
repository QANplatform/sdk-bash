# QANApi

All URIs are relative to **

Method | HTTP request | Description
------------- | ------------- | -------------
[**qanBlockNumber**](QANApi.md#qanBlockNumber) | **GET** /blockNumber/ | Returns the latest block number of the blockchain.
[**qanCall**](QANApi.md#qanCall) | **POST** /call/ | Executes a new message call immediately without creating a transaction on the block chain.
[**qanChainId**](QANApi.md#qanChainId) | **GET** /chainId/ | Returns the current network/chain ID, used to sign replay-protected transaction introduced in EIP-155.
[**qanEstimateGas**](QANApi.md#qanEstimateGas) | **POST** /estimateGas/ | Returns an estimation of gas for a given transaction.
[**qanFeeHistory**](QANApi.md#qanFeeHistory) | **POST** /feeHistory/ | Returns the collection of historical gas information.
[**qanGasPrice**](QANApi.md#qanGasPrice) | **GET** /gasPrice/ | Returns the current gas price on the network in wei.
[**qanGetBalance**](QANApi.md#qanGetBalance) | **GET** /getBalance/{Address}/ | Returns the balance of the account of given address.
[**qanGetBlockByHash**](QANApi.md#qanGetBlockByHash) | **GET** /getBlockByHash/{Hash}/{TransactionDetailFlag}/ | Returns information of the block matching the given block hash.
[**qanGetBlockByNumber**](QANApi.md#qanGetBlockByNumber) | **GET** /getBlockByNumber/{BlockNumber}/{TransactionDetailFlag}/ | Returns information of the block matching the given block number.
[**qanGetBlockReceipts**](QANApi.md#qanGetBlockReceipts) | **GET** /getBlockReceipts/{BlockNumber}/ | Returns all transaction receipts for a given block.
[**qanGetBlockTransactionCountByHash**](QANApi.md#qanGetBlockTransactionCountByHash) | **GET** /getBlockTransactionCountByHash/{Hash}/ | Returns the number of transactions for the block matching the given block hash.
[**qanGetBlockTransactionCountByNumber**](QANApi.md#qanGetBlockTransactionCountByNumber) | **GET** /getBlockTransactionCountByNumber/{BlockNumber}/ | Returns the number of transactions for the block matching the given block number.
[**qanGetCode**](QANApi.md#qanGetCode) | **GET** /getCode/{Address}/ | Returns the compiled bytecode of a smart contract.
[**qanGetFilterChanges**](QANApi.md#qanGetFilterChanges) | **GET** /getFilterChanges/{FilterId}/ | Polling method for a filter, which returns an array of events that have occurred since the last poll.
[**qanGetFilterLogs**](QANApi.md#qanGetFilterLogs) | **GET** /getFilterLogs/{Id}/ | Returns an array of all logs matching filter with given id.
[**qanGetLogs**](QANApi.md#qanGetLogs) | **POST** /getLogs/ | Returns an array of all logs matching a given filter object.
[**qanGetProof**](QANApi.md#qanGetProof) | **POST** /getProof/ | Returns the account and storage values of the specified account including the Merkle-proof.
[**qanGetStorageAt**](QANApi.md#qanGetStorageAt) | **POST** /getStorageAt/ | Returns the value from a storage position at a given address.
[**qanGetTransactionByBlockHashAndIndex**](QANApi.md#qanGetTransactionByBlockHashAndIndex) | **GET** /getTransactionByBlockHashAndIndex/{blockHash}/{index}/ | Returns information about a transaction given a blockhash and transaction index position.
[**qanGetTransactionByBlockNumberAndIndex**](QANApi.md#qanGetTransactionByBlockNumberAndIndex) | **GET** /getTransactionByBlockNumberAndIndex/{blockNumber}/{index}/ | Returns information about a transaction given a block number and transaction index position.
[**qanGetTransactionByHash**](QANApi.md#qanGetTransactionByHash) | **GET** /getTransactionByHash/{hash}/ | Returns the information about a transaction from a transaction hash.
[**qanGetTransactionCount**](QANApi.md#qanGetTransactionCount) | **GET** /getTransactionCount/{Address}/{BlockNumber}/ | Returns the number of transactions sent from an address.
[**qanGetTransactionReceipt**](QANApi.md#qanGetTransactionReceipt) | **GET** /getTransactionReceipt/{Hash}/ | Returns the receipt of a transaction by transaction hash.
[**qanMaxPriorityFeePerGas**](QANApi.md#qanMaxPriorityFeePerGas) | **GET** /maxPriorityFeePerGas/ | Get the priority fee needed to be included in a block.
[**qanNewBlockFilter**](QANApi.md#qanNewBlockFilter) | **GET** /newBlockFilter/ | Creates a filter in the node, to notify when a new block arrives.
[**qanNewFilter**](QANApi.md#qanNewFilter) | **POST** /newFilter/ | Creates a filter object, based on filter options, to notify when the state changes (logs).
[**qanNewPendingTransactionFilter**](QANApi.md#qanNewPendingTransactionFilter) | **GET** /newPendingTransactionFilter/ | Creates a filter in the node to notify when new pending transactions arrive.
[**qanSendRawTransaction**](QANApi.md#qanSendRawTransaction) | **POST** /sendRawTransaction/ | Creates new message call transaction or a contract creation for signed transactions.
[**qanSyncing**](QANApi.md#qanSyncing) | **GET** /syncing/ | Returns an object with the sync status of the node if the node is out-of-sync and is syncing. Returns null when the node is already in sync.
[**qanUninstallFilter**](QANApi.md#qanUninstallFilter) | **GET** /uninstallFilter/{FilterId}/ | Uninstalls a filter with the given filter id.
[**qanXlinkValid**](QANApi.md#qanXlinkValid) | **GET** /xlinkValid/{Address}/ | Returns the xlink validity time of the account of given address.



## qanBlockNumber

Returns the latest block number of the blockchain.

### Example

```bash
 qanBlockNumber
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**OutputBlockNumber**](OutputBlockNumber.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanCall

Executes a new message call immediately without creating a transaction on the block chain.

### Example

```bash
 qanCall
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inputCall** | [**InputCall**](InputCall.md) |  |

### Return type

[**OutputCall**](OutputCall.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanChainId

Returns the current network/chain ID, used to sign replay-protected transaction introduced in EIP-155.

### Example

```bash
 qanChainId
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**OutputChainId**](OutputChainId.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanEstimateGas

Returns an estimation of gas for a given transaction.

### Example

```bash
 qanEstimateGas
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inputEstimateGas** | [**InputEstimateGas**](InputEstimateGas.md) |  |

### Return type

[**OutputEstimateGas**](OutputEstimateGas.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanFeeHistory

Returns the collection of historical gas information.

### Example

```bash
 qanFeeHistory
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inputFeeHistory** | [**InputFeeHistory**](InputFeeHistory.md) |  |

### Return type

[**OutputFeeHistory**](OutputFeeHistory.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanGasPrice

Returns the current gas price on the network in wei.

### Example

```bash
 qanGasPrice
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**OutputGasPrice**](OutputGasPrice.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanGetBalance

Returns the balance of the account of given address.

### Example

```bash
 qanGetBalance Address=value  BlockNumber=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **address** | **string** | A 20 bytes long hexadecimal value representing an address | [default to null]
 **blockNumber** | **string** | The block number in hexadecimal or decimal format or the string latest, earliest, pending | [optional] [default to latest]

### Return type

[**OutputGetBalance**](OutputGetBalance.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanGetBlockByHash

Returns information of the block matching the given block hash.

### Example

```bash
 qanGetBlockByHash Hash=value TransactionDetailFlag=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **hash** | **string** | The hash (32 bytes) of the block | [default to null]
 **transactionDetailFlag** | **boolean** | The method returns the full transaction objects when this value is true otherwise, it returns only the hashes of the transactions | [default to false]

### Return type

[**OutputGetBlockByHash**](OutputGetBlockByHash.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanGetBlockByNumber

Returns information of the block matching the given block number.

### Example

```bash
 qanGetBlockByNumber BlockNumber=value TransactionDetailFlag=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **blockNumber** | **string** | The block number in hexadecimal or decimal format or the string latest, earliest, pending | [default to latest]
 **transactionDetailFlag** | **boolean** | The method returns the full transaction objects when this value is true otherwise, it returns only the hashes of the transactions | [default to false]

### Return type

[**OutputGetBlockByNumber**](OutputGetBlockByNumber.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanGetBlockReceipts

Returns all transaction receipts for a given block.

### Example

```bash
 qanGetBlockReceipts BlockNumber=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **blockNumber** | **string** | The block number in hexadecimal or decimal format or the string latest, earliest, pending | [default to latest]

### Return type

[**OutputGetBlockReceipts**](OutputGetBlockReceipts.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanGetBlockTransactionCountByHash

Returns the number of transactions for the block matching the given block hash.

### Example

```bash
 qanGetBlockTransactionCountByHash Hash=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **hash** | **string** | The hash of the block | [default to null]

### Return type

[**OutputGetBlockTransactionCountByHash**](OutputGetBlockTransactionCountByHash.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanGetBlockTransactionCountByNumber

Returns the number of transactions for the block matching the given block number.

### Example

```bash
 qanGetBlockTransactionCountByNumber BlockNumber=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **blockNumber** | **string** | The block number in hexadecimal or decimal format or the string latest, earliest, pending | [default to null]

### Return type

[**OutputGetBlockTransactionCountByNumber**](OutputGetBlockTransactionCountByNumber.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanGetCode

Returns the compiled bytecode of a smart contract.

### Example

```bash
 qanGetCode Address=value  BlockNumber=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **address** | **string** | The address of the smart contract from which the bytecode will be obtained | [default to null]
 **blockNumber** | **string** | The block number in hexadecimal or decimal format or the string latest, earliest, pending | [optional] [default to latest]

### Return type

[**OutputGetCode**](OutputGetCode.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanGetFilterChanges

Polling method for a filter, which returns an array of events that have occurred since the last poll.

### Example

```bash
 qanGetFilterChanges FilterId=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filterId** | **string** | The filter id that is returned from getFilterChangesnewFilter, getFilterChangesnewBlockFilter or getFilterChangesnewPendingTransactionFilter | [default to null]

### Return type

[**OutputGetFilterChanges**](OutputGetFilterChanges.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanGetFilterLogs

Returns an array of all logs matching filter with given id.

### Example

```bash
 qanGetFilterLogs Id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string** | The filter ID | [default to null]

### Return type

[**OutputGetFilterLogs**](OutputGetFilterLogs.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanGetLogs

Returns an array of all logs matching a given filter object.

### Example

```bash
 qanGetLogs
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inputGetLogs** | [**InputGetLogs**](InputGetLogs.md) |  |

### Return type

[**OutputGetLogs**](OutputGetLogs.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanGetProof

Returns the account and storage values of the specified account including the Merkle-proof.

### Example

```bash
 qanGetProof
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inputGetProof** | [**InputGetProof**](InputGetProof.md) |  |

### Return type

[**OutputGetProof**](OutputGetProof.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanGetStorageAt

Returns the value from a storage position at a given address.

### Example

```bash
 qanGetStorageAt
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inputGetStorageAt** | [**InputGetStorageAt**](InputGetStorageAt.md) |  |

### Return type

[**OutputGetStorageAt**](OutputGetStorageAt.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanGetTransactionByBlockHashAndIndex

Returns information about a transaction given a blockhash and transaction index position.

### Example

```bash
 qanGetTransactionByBlockHashAndIndex blockHash=value index=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **blockHash** | **string** |  | [default to null]
 **index** | **string** | An integer of the transaction index position | [default to null]

### Return type

[**OutputGetTransactionByBlockHashAndIndex**](OutputGetTransactionByBlockHashAndIndex.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanGetTransactionByBlockNumberAndIndex

Returns information about a transaction given a block number and transaction index position.

### Example

```bash
 qanGetTransactionByBlockNumberAndIndex blockNumber=value index=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **blockNumber** | **string** | The block number in hexadecimal or decimal format or the string latest, earliest, pending | [default to null]
 **index** | **string** | An integer of the transaction index position | [default to null]

### Return type

[**OutputGetTransactionByBlockNumberAndIndex**](OutputGetTransactionByBlockNumberAndIndex.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanGetTransactionByHash

Returns the information about a transaction from a transaction hash.

### Example

```bash
 qanGetTransactionByHash hash=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **hash** | **string** | The hash of a transaction | [default to null]

### Return type

[**OutputGetTransactionByHash**](OutputGetTransactionByHash.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanGetTransactionCount

Returns the number of transactions sent from an address.

### Example

```bash
 qanGetTransactionCount Address=value BlockNumber=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **address** | **string** | The address from which the transaction count to be checked | [default to null]
 **blockNumber** | **string** | The block number in hexadecimal or decimal format or the string latest, earliest, pending | [default to null]

### Return type

[**OutputGetTransactionCount**](OutputGetTransactionCount.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanGetTransactionReceipt

Returns the receipt of a transaction by transaction hash.

### Example

```bash
 qanGetTransactionReceipt Hash=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **hash** | **string** | The hash of a transaction | [default to null]

### Return type

[**OutputGetTransactionReceipt**](OutputGetTransactionReceipt.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanMaxPriorityFeePerGas

Get the priority fee needed to be included in a block.

### Example

```bash
 qanMaxPriorityFeePerGas
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**OutputMaxPriorityFeePerGas**](OutputMaxPriorityFeePerGas.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanNewBlockFilter

Creates a filter in the node, to notify when a new block arrives.

### Example

```bash
 qanNewBlockFilter
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**OutputNewBlockFilter**](OutputNewBlockFilter.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanNewFilter

Creates a filter object, based on filter options, to notify when the state changes (logs).

### Example

```bash
 qanNewFilter
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inputNewFilter** | [**InputNewFilter**](InputNewFilter.md) |  |

### Return type

[**OutputNewFilter**](OutputNewFilter.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanNewPendingTransactionFilter

Creates a filter in the node to notify when new pending transactions arrive.

### Example

```bash
 qanNewPendingTransactionFilter
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**OutputNewPendingTransactionFilter**](OutputNewPendingTransactionFilter.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanSendRawTransaction

Creates new message call transaction or a contract creation for signed transactions.

### Example

```bash
 qanSendRawTransaction
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inputSendRawTransaction** | [**InputSendRawTransaction**](InputSendRawTransaction.md) |  |

### Return type

[**OutputSendRawTransaction**](OutputSendRawTransaction.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanSyncing

Returns an object with the sync status of the node if the node is out-of-sync and is syncing. Returns null when the node is already in sync.

### Example

```bash
 qanSyncing
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**OutputSyncing**](OutputSyncing.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanUninstallFilter

Uninstalls a filter with the given filter id.

### Example

```bash
 qanUninstallFilter FilterId=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filterId** | **string** | The filter ID that needs to be uninstalled. It should always be called when watch is no longer needed. Additionally, Filters timeout when they aren't requested with getFilterChanges for a period of time | [default to null]

### Return type

[**OutputUninstallFilter**](OutputUninstallFilter.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## qanXlinkValid

Returns the xlink validity time of the account of given address.

### Example

```bash
 qanXlinkValid Address=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **address** | **string** |  | [default to null]

### Return type

[**OutputXlinkValid**](OutputXlinkValid.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

