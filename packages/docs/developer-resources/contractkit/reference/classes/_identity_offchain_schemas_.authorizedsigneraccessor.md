# Class: AuthorizedSignerAccessor

## Hierarchy

* **AuthorizedSignerAccessor**

## Index

### Constructors

* [constructor](_identity_offchain_schemas_.authorizedsigneraccessor.md#constructor)

### Properties

* [basePath](_identity_offchain_schemas_.authorizedsigneraccessor.md#basepath)
* [read](_identity_offchain_schemas_.authorizedsigneraccessor.md#read)
* [wrapper](_identity_offchain_schemas_.authorizedsigneraccessor.md#wrapper)

### Methods

* [readAsResult](_identity_offchain_schemas_.authorizedsigneraccessor.md#readasresult)
* [write](_identity_offchain_schemas_.authorizedsigneraccessor.md#write)

## Constructors

###  constructor

\+ **new AuthorizedSignerAccessor**(`wrapper`: [OffchainDataWrapper](_identity_offchain_data_wrapper_.offchaindatawrapper.md)): *[AuthorizedSignerAccessor](_identity_offchain_schemas_.authorizedsigneraccessor.md)*

*Defined in [contractkit/src/identity/offchain/schemas.ts:27](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/identity/offchain/schemas.ts#L27)*

**Parameters:**

Name | Type |
------ | ------ |
`wrapper` | [OffchainDataWrapper](_identity_offchain_data_wrapper_.offchaindatawrapper.md) |

**Returns:** *[AuthorizedSignerAccessor](_identity_offchain_schemas_.authorizedsigneraccessor.md)*

## Properties

###  basePath

• **basePath**: *string* = "/account/authorizedSigners"

*Defined in [contractkit/src/identity/offchain/schemas.ts:27](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/identity/offchain/schemas.ts#L27)*

___

###  read

• **read**: *any* = makeAsyncThrowable(this.readAsResult.bind(this))

*Defined in [contractkit/src/identity/offchain/schemas.ts:39](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/identity/offchain/schemas.ts#L39)*

___

###  wrapper

• **wrapper**: *[OffchainDataWrapper](_identity_offchain_data_wrapper_.offchaindatawrapper.md)*

*Defined in [contractkit/src/identity/offchain/schemas.ts:28](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/identity/offchain/schemas.ts#L28)*

## Methods

###  readAsResult

▸ **readAsResult**(`account`: [Address](../modules/_base_.md#address), `signer`: [Address](../modules/_base_.md#address)): *Promise‹any›*

*Defined in [contractkit/src/identity/offchain/schemas.ts:30](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/identity/offchain/schemas.ts#L30)*

**Parameters:**

Name | Type |
------ | ------ |
`account` | [Address](../modules/_base_.md#address) |
`signer` | [Address](../modules/_base_.md#address) |

**Returns:** *Promise‹any›*

___

###  write

▸ **write**(`signer`: [Address](../modules/_base_.md#address), `proofOfPossession`: string, `filteredDataPaths`: string): *Promise‹void›*

*Defined in [contractkit/src/identity/offchain/schemas.ts:41](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/identity/offchain/schemas.ts#L41)*

**Parameters:**

Name | Type |
------ | ------ |
`signer` | [Address](../modules/_base_.md#address) |
`proofOfPossession` | string |
`filteredDataPaths` | string |

**Returns:** *Promise‹void›*
