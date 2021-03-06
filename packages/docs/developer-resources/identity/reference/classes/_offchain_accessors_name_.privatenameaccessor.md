# Class: PrivateNameAccessor

## Hierarchy

* [PrivateSimpleAccessor](_offchain_accessors_simple_.privatesimpleaccessor.md)‹[NameType](../modules/_offchain_accessors_name_.md#nametype)›

  ↳ **PrivateNameAccessor**

## Implements

* [PrivateAccessor](../interfaces/_offchain_accessors_interfaces_.privateaccessor.md)‹[NameType](../modules/_offchain_accessors_name_.md#nametype)›

## Index

### Constructors

* [constructor](_offchain_accessors_name_.privatenameaccessor.md#constructor)

### Properties

* [dataPath](_offchain_accessors_name_.privatenameaccessor.md#readonly-datapath)
* [read](_offchain_accessors_name_.privatenameaccessor.md#read)
* [type](_offchain_accessors_name_.privatenameaccessor.md#readonly-type)
* [wrapper](_offchain_accessors_name_.privatenameaccessor.md#readonly-wrapper)

### Methods

* [readAsResult](_offchain_accessors_name_.privatenameaccessor.md#readasresult)
* [write](_offchain_accessors_name_.privatenameaccessor.md#write)

## Constructors

###  constructor

\+ **new PrivateNameAccessor**(`wrapper`: [OffchainDataWrapper](_offchain_data_wrapper_.offchaindatawrapper.md)): *[PrivateNameAccessor](_offchain_accessors_name_.privatenameaccessor.md)*

*Overrides [PrivateSimpleAccessor](_offchain_accessors_simple_.privatesimpleaccessor.md).[constructor](_offchain_accessors_simple_.privatesimpleaccessor.md#constructor)*

*Defined in [packages/sdk/identity/src/offchain/accessors/name.ts:17](https://github.com/medhak1/celo-monorepo/blob/master/packages/sdk/identity/src/offchain/accessors/name.ts#L17)*

**Parameters:**

Name | Type |
------ | ------ |
`wrapper` | [OffchainDataWrapper](_offchain_data_wrapper_.offchaindatawrapper.md) |

**Returns:** *[PrivateNameAccessor](_offchain_accessors_name_.privatenameaccessor.md)*

## Properties

### `Readonly` dataPath

• **dataPath**: *string*

*Inherited from [PrivateSimpleAccessor](_offchain_accessors_simple_.privatesimpleaccessor.md).[dataPath](_offchain_accessors_simple_.privatesimpleaccessor.md#readonly-datapath)*

*Defined in [packages/sdk/identity/src/offchain/accessors/simple.ts:72](https://github.com/medhak1/celo-monorepo/blob/master/packages/sdk/identity/src/offchain/accessors/simple.ts#L72)*

___

###  read

• **read**: *function* = makeAsyncThrowable(this.readAsResult.bind(this))

*Implementation of [PrivateAccessor](../interfaces/_offchain_accessors_interfaces_.privateaccessor.md).[read](../interfaces/_offchain_accessors_interfaces_.privateaccessor.md#read)*

*Inherited from [PrivateSimpleAccessor](_offchain_accessors_simple_.privatesimpleaccessor.md).[read](_offchain_accessors_simple_.privatesimpleaccessor.md#read)*

*Defined in [packages/sdk/identity/src/offchain/accessors/simple.ts:93](https://github.com/medhak1/celo-monorepo/blob/master/packages/sdk/identity/src/offchain/accessors/simple.ts#L93)*

#### Type declaration:

▸ (...`args`: TArgs): *Promise‹TResult›*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | TArgs |

___

### `Readonly` type

• **type**: *Type‹[NameType](../modules/_offchain_accessors_name_.md#nametype)›*

*Inherited from [PrivateSimpleAccessor](_offchain_accessors_simple_.privatesimpleaccessor.md).[type](_offchain_accessors_simple_.privatesimpleaccessor.md#readonly-type)*

*Defined in [packages/sdk/identity/src/offchain/accessors/simple.ts:71](https://github.com/medhak1/celo-monorepo/blob/master/packages/sdk/identity/src/offchain/accessors/simple.ts#L71)*

___

### `Readonly` wrapper

• **wrapper**: *[OffchainDataWrapper](_offchain_data_wrapper_.offchaindatawrapper.md)*

*Overrides [PrivateSimpleAccessor](_offchain_accessors_simple_.privatesimpleaccessor.md).[wrapper](_offchain_accessors_simple_.privatesimpleaccessor.md#readonly-wrapper)*

*Defined in [packages/sdk/identity/src/offchain/accessors/name.ts:18](https://github.com/medhak1/celo-monorepo/blob/master/packages/sdk/identity/src/offchain/accessors/name.ts#L18)*

## Methods

###  readAsResult

▸ **readAsResult**(`account`: Address): *Promise‹Result‹[NameType](../modules/_offchain_accessors_name_.md#nametype), [SchemaErrors](../modules/_offchain_accessors_errors_.md#schemaerrors)››*

*Inherited from [PrivateSimpleAccessor](_offchain_accessors_simple_.privatesimpleaccessor.md).[readAsResult](_offchain_accessors_simple_.privatesimpleaccessor.md#readasresult)*

*Defined in [packages/sdk/identity/src/offchain/accessors/simple.ts:83](https://github.com/medhak1/celo-monorepo/blob/master/packages/sdk/identity/src/offchain/accessors/simple.ts#L83)*

**Parameters:**

Name | Type |
------ | ------ |
`account` | Address |

**Returns:** *Promise‹Result‹[NameType](../modules/_offchain_accessors_name_.md#nametype), [SchemaErrors](../modules/_offchain_accessors_errors_.md#schemaerrors)››*

___

###  write

▸ **write**(`data`: [NameType](../modules/_offchain_accessors_name_.md#nametype), `toAddresses`: Address[], `symmetricKey?`: Buffer): *Promise‹void | [InvalidDataError](_offchain_accessors_errors_.invaliddataerror.md)‹› | [OffchainError](_offchain_accessors_errors_.offchainerror.md)‹› | [UnknownCiphertext](_offchain_accessors_errors_.unknownciphertext.md)‹› | [UnavailableKey](_offchain_accessors_errors_.unavailablekey.md)‹› | [InvalidKey](_offchain_accessors_errors_.invalidkey.md)‹››*

*Inherited from [PrivateSimpleAccessor](_offchain_accessors_simple_.privatesimpleaccessor.md).[write](_offchain_accessors_simple_.privatesimpleaccessor.md#write)*

*Defined in [packages/sdk/identity/src/offchain/accessors/simple.ts:75](https://github.com/medhak1/celo-monorepo/blob/master/packages/sdk/identity/src/offchain/accessors/simple.ts#L75)*

**Parameters:**

Name | Type |
------ | ------ |
`data` | [NameType](../modules/_offchain_accessors_name_.md#nametype) |
`toAddresses` | Address[] |
`symmetricKey?` | Buffer |

**Returns:** *Promise‹void | [InvalidDataError](_offchain_accessors_errors_.invaliddataerror.md)‹› | [OffchainError](_offchain_accessors_errors_.offchainerror.md)‹› | [UnknownCiphertext](_offchain_accessors_errors_.unknownciphertext.md)‹› | [UnavailableKey](_offchain_accessors_errors_.unavailablekey.md)‹› | [InvalidKey](_offchain_accessors_errors_.invalidkey.md)‹››*
