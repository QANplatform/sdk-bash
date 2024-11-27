# QAN Bash SDK

This repository is guaranteed up-to-date with the upstream QAN API definitions, and leverages OpenAPI technology to stay consistent.

Versioning is based on SEMVER, meaning:

- Stable releases guarantee backwards compatibility for the same major versions.
- Minor releases will not contain breaking changes.
- Patch releases only focus on fixing issues.

## Documentation for API Endpoints

All URIs are relative to *https://rpc-testnet.qanplatform.com*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*QANApi* | [**qanBlockNumber**](docs/QANApi.md#qanblocknumber) | **GET** /blockNumber/ | 
*QANApi* | [**qanCall**](docs/QANApi.md#qancall) | **POST** /call/ | 
*QANApi* | [**qanChainId**](docs/QANApi.md#qanchainid) | **GET** /chainId/ | 
*QANApi* | [**qanEstimateGas**](docs/QANApi.md#qanestimategas) | **POST** /estimateGas/ | 
*QANApi* | [**qanFeeHistory**](docs/QANApi.md#qanfeehistory) | **POST** /feeHistory/ | 
*QANApi* | [**qanGasPrice**](docs/QANApi.md#qangasprice) | **GET** /gasPrice/ | 
*QANApi* | [**qanGetBalance**](docs/QANApi.md#qangetbalance) | **GET** /getBalance/{Address}/ | 
*QANApi* | [**qanGetBlockByHash**](docs/QANApi.md#qangetblockbyhash) | **GET** /getBlockByHash/{Hash}/{TransactionDetailFlag}/ | 
*QANApi* | [**qanGetBlockByNumber**](docs/QANApi.md#qangetblockbynumber) | **GET** /getBlockByNumber/{BlockNumber}/{TransactionDetailFlag}/ | 
*QANApi* | [**qanGetBlockReceipts**](docs/QANApi.md#qangetblockreceipts) | **GET** /getBlockReceipts/{BlockNumber}/ | 
*QANApi* | [**qanGetBlockTransactionCountByHash**](docs/QANApi.md#qangetblocktransactioncountbyhash) | **GET** /getBlockTransactionCountByHash/{Hash}/ | 
*QANApi* | [**qanGetBlockTransactionCountByNumber**](docs/QANApi.md#qangetblocktransactioncountbynumber) | **GET** /getBlockTransactionCountByNumber/{BlockNumber}/ | 
*QANApi* | [**qanGetCode**](docs/QANApi.md#qangetcode) | **GET** /getCode/{Address}/ | 
*QANApi* | [**qanGetFilterChanges**](docs/QANApi.md#qangetfilterchanges) | **GET** /getFilterChanges/{FilterId}/ | 
*QANApi* | [**qanGetFilterLogs**](docs/QANApi.md#qangetfilterlogs) | **GET** /getFilterLogs/{Id}/ | 
*QANApi* | [**qanGetLogs**](docs/QANApi.md#qangetlogs) | **POST** /getLogs/ | 
*QANApi* | [**qanGetProof**](docs/QANApi.md#qangetproof) | **POST** /getProof/ | 
*QANApi* | [**qanGetStorageAt**](docs/QANApi.md#qangetstorageat) | **POST** /getStorageAt/ | 
*QANApi* | [**qanGetTransactionByBlockHashAndIndex**](docs/QANApi.md#qangettransactionbyblockhashandindex) | **GET** /getTransactionByBlockHashAndIndex/{blockHash}/{index}/ | 
*QANApi* | [**qanGetTransactionByBlockNumberAndIndex**](docs/QANApi.md#qangettransactionbyblocknumberandindex) | **GET** /getTransactionByBlockNumberAndIndex/{blockNumber}/{index}/ | 
*QANApi* | [**qanGetTransactionByHash**](docs/QANApi.md#qangettransactionbyhash) | **GET** /getTransactionByHash/{hash}/ | 
*QANApi* | [**qanGetTransactionCount**](docs/QANApi.md#qangettransactioncount) | **GET** /getTransactionCount/{Address}/{BlockNumber}/ | 
*QANApi* | [**qanGetTransactionReceipt**](docs/QANApi.md#qangettransactionreceipt) | **GET** /getTransactionReceipt/{Hash}/ | 
*QANApi* | [**qanMaxPriorityFeePerGas**](docs/QANApi.md#qanmaxpriorityfeepergas) | **GET** /maxPriorityFeePerGas/ | 
*QANApi* | [**qanNewBlockFilter**](docs/QANApi.md#qannewblockfilter) | **GET** /newBlockFilter/ | 
*QANApi* | [**qanNewFilter**](docs/QANApi.md#qannewfilter) | **POST** /newFilter/ | 
*QANApi* | [**qanNewPendingTransactionFilter**](docs/QANApi.md#qannewpendingtransactionfilter) | **GET** /newPendingTransactionFilter/ | 
*QANApi* | [**qanSendRawTransaction**](docs/QANApi.md#qansendrawtransaction) | **POST** /sendRawTransaction/ | 
*QANApi* | [**qanSyncing**](docs/QANApi.md#qansyncing) | **GET** /syncing/ | 
*QANApi* | [**qanUninstallFilter**](docs/QANApi.md#qanuninstallfilter) | **GET** /uninstallFilter/{FilterId}/ | 
*QANApi* | [**qanXlinkValid**](docs/QANApi.md#qanxlinkvalid) | **GET** /xlinkValid/{Address}/ | 


## Documentation For Models

 - [ErrorDetail](docs/ErrorDetail.md)
 - [ErrorModel](docs/ErrorModel.md)
 - [EstimateGasObject](docs/EstimateGasObject.md)
 - [FilterObject](docs/FilterObject.md)
 - [InputCall](docs/InputCall.md)
 - [InputEstimateGas](docs/InputEstimateGas.md)
 - [InputFeeHistory](docs/InputFeeHistory.md)
 - [InputGetLogs](docs/InputGetLogs.md)
 - [InputGetProof](docs/InputGetProof.md)
 - [InputGetStorageAt](docs/InputGetStorageAt.md)
 - [InputNewFilter](docs/InputNewFilter.md)
 - [InputSendRawTransaction](docs/InputSendRawTransaction.md)
 - [OutputBlockNumber](docs/OutputBlockNumber.md)
 - [OutputCall](docs/OutputCall.md)
 - [OutputChainId](docs/OutputChainId.md)
 - [OutputEstimateGas](docs/OutputEstimateGas.md)
 - [OutputFeeHistory](docs/OutputFeeHistory.md)
 - [OutputGasPrice](docs/OutputGasPrice.md)
 - [OutputGetBalance](docs/OutputGetBalance.md)
 - [OutputGetBlockByHash](docs/OutputGetBlockByHash.md)
 - [OutputGetBlockByNumber](docs/OutputGetBlockByNumber.md)
 - [OutputGetBlockReceipts](docs/OutputGetBlockReceipts.md)
 - [OutputGetBlockTransactionCountByHash](docs/OutputGetBlockTransactionCountByHash.md)
 - [OutputGetBlockTransactionCountByNumber](docs/OutputGetBlockTransactionCountByNumber.md)
 - [OutputGetCode](docs/OutputGetCode.md)
 - [OutputGetFilterChanges](docs/OutputGetFilterChanges.md)
 - [OutputGetFilterLogs](docs/OutputGetFilterLogs.md)
 - [OutputGetLogs](docs/OutputGetLogs.md)
 - [OutputGetProof](docs/OutputGetProof.md)
 - [OutputGetStorageAt](docs/OutputGetStorageAt.md)
 - [OutputGetTransactionByBlockHashAndIndex](docs/OutputGetTransactionByBlockHashAndIndex.md)
 - [OutputGetTransactionByBlockNumberAndIndex](docs/OutputGetTransactionByBlockNumberAndIndex.md)
 - [OutputGetTransactionByHash](docs/OutputGetTransactionByHash.md)
 - [OutputGetTransactionCount](docs/OutputGetTransactionCount.md)
 - [OutputGetTransactionReceipt](docs/OutputGetTransactionReceipt.md)
 - [OutputMaxPriorityFeePerGas](docs/OutputMaxPriorityFeePerGas.md)
 - [OutputNewBlockFilter](docs/OutputNewBlockFilter.md)
 - [OutputNewFilter](docs/OutputNewFilter.md)
 - [OutputNewPendingTransactionFilter](docs/OutputNewPendingTransactionFilter.md)
 - [OutputSendRawTransaction](docs/OutputSendRawTransaction.md)
 - [OutputSyncing](docs/OutputSyncing.md)
 - [OutputUninstallFilter](docs/OutputUninstallFilter.md)
 - [OutputXlinkValid](docs/OutputXlinkValid.md)
 - [ParamsTransaction](docs/ParamsTransaction.md)
 - [ResponseBlock](docs/ResponseBlock.md)
 - [ResponseLog](docs/ResponseLog.md)
 - [ResponseStorageEntry](docs/ResponseStorageEntry.md)
 - [ResponseTransaction](docs/ResponseTransaction.md)
 - [ResponseTransactionReceipt](docs/ResponseTransactionReceipt.md)
 - [ResponseWithdrawals](docs/ResponseWithdrawals.md)
 - [SyncStatus](docs/SyncStatus.md)

## Acknowledgements

We would like to thank Smartbear and OpenAPITools tech for making building declarative APIs possible.
A huge benefit for the whole industry!
