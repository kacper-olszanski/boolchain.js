[boolchain](README.md) / Exports

# boolchain

## Table of contents

### Functions

- [and](modules.md#and)
- [andAsync](modules.md#andasync)
- [nand](modules.md#nand)
- [nandAsync](modules.md#nandasync)
- [not](modules.md#not)
- [notAsync](modules.md#notasync)
- [or](modules.md#or)
- [orAsync](modules.md#orasync)
- [xor](modules.md#xor)
- [xorAsync](modules.md#xorasync)

## Functions

### and

▸ **and**\<`T`\>(`...funcs`): `T`

Combines multiple functions or boolean values into a single function that returns true
if all functions return true or all boolean values are true.

#### Type parameters

| Name | Type                             | Description                               |
| :--- | :------------------------------- | :---------------------------------------- |
| `T`  | extends `BoolchainType`\<`any`\> | The type of the functions being combined. |

#### Parameters

| Name       | Type                                 | Description                                 |
| :--------- | :----------------------------------- | :------------------------------------------ |
| `...funcs` | [`unknown`, `unknown`, ...unknown[]] | The functions or boolean values to combine. |

#### Returns

`T`

- A function that returns true if all functions return true or all boolean values are true.

#### Defined in

[core/and.ts:12](https://github.com/kacper-olszanski/boolchain.js/blob/cca7c726b6dd3d7319c5387e40412e9999db9188/lib/core/and.ts#L12)

---

### andAsync

▸ **andAsync**\<`T`\>(`...funcs`): `T`

Combines multiple asynchronous functions or boolean values into a single asynchronous function.
The resulting function returns `true` if all functions return `true` or all boolean values are `true`,
otherwise it returns `false`.

#### Type parameters

| Name | Type                                | Description                             |
| :--- | :---------------------------------- | :-------------------------------------- |
| `T`  | extends `BoolchainAsyncType`\<`T`\> | The type of the asynchronous functions. |

#### Parameters

| Name       | Type                                 | Description                                           |
| :--------- | :----------------------------------- | :---------------------------------------------------- |
| `...funcs` | [`unknown`, `unknown`, ...unknown[]] | An array of asynchronous functions or boolean values. |

#### Returns

`T`

An asynchronous function that combines the provided functions or boolean values.

#### Defined in

[core/and.ts:39](https://github.com/kacper-olszanski/boolchain.js/blob/cca7c726b6dd3d7319c5387e40412e9999db9188/lib/core/and.ts#L39)

---

### nand

▸ **nand**\<`T`\>(`...funcs`): `T`

#### Type parameters

| Name | Type                           |
| :--- | :----------------------------- |
| `T`  | extends `BoolchainType`\<`T`\> |

#### Parameters

| Name       | Type                                 |
| :--------- | :----------------------------------- |
| `...funcs` | [`unknown`, `unknown`, ...unknown[]] |

#### Returns

`T`

#### Defined in

core/nand.ts:6

---

### nandAsync

▸ **nandAsync**\<`T`\>(`...funcs`): `T`

#### Type parameters

| Name | Type                                |
| :--- | :---------------------------------- |
| `T`  | extends `BoolchainAsyncType`\<`T`\> |

#### Parameters

| Name       | Type                                 |
| :--------- | :----------------------------------- |
| `...funcs` | [`unknown`, `unknown`, ...unknown[]] |

#### Returns

`T`

#### Defined in

core/nand.ts:10

---

### not

▸ **not**\<`T`\>(`func`): `T`

Returns a new function that negates the result of the provided function.

#### Type parameters

| Name | Type                           | Description                        |
| :--- | :----------------------------- | :--------------------------------- |
| `T`  | extends `BoolchainType`\<`T`\> | The type of the provided function. |

#### Parameters

| Name   | Type      | Description             |
| :----- | :-------- | :---------------------- |
| `func` | `unknown` | The function to negate. |

#### Returns

`T`

- A new function that negates the result of the provided function.

#### Defined in

[core/not.ts:11](https://github.com/kacper-olszanski/boolchain.js/blob/cca7c726b6dd3d7319c5387e40412e9999db9188/lib/core/not.ts#L11)

---

### notAsync

▸ **notAsync**\<`T`\>(`func`): `T`

Wraps an asynchronous function and returns a new function that negates the result of the original function.

#### Type parameters

| Name | Type                                | Description                        |
| :--- | :---------------------------------- | :--------------------------------- |
| `T`  | extends `BoolchainAsyncType`\<`T`\> | The type of the original function. |

#### Parameters

| Name   | Type | Description                          |
| :----- | :--- | :----------------------------------- |
| `func` | `T`  | The original function to be wrapped. |

#### Returns

`T`

- A new function that negates the result of the original function.

#### Defined in

[core/not.ts:25](https://github.com/kacper-olszanski/boolchain.js/blob/cca7c726b6dd3d7319c5387e40412e9999db9188/lib/core/not.ts#L25)

---

### or

▸ **or**\<`T`\>(`...funcs`): `T`

Combines multiple functions or boolean values into a single function that returns true if any of the functions return true or any of the boolean values are true.

#### Type parameters

| Name | Type                           | Description                        |
| :--- | :----------------------------- | :--------------------------------- |
| `T`  | extends `BoolchainType`\<`T`\> | The type of the combined function. |

#### Parameters

| Name       | Type                                 | Description                                     |
| :--------- | :----------------------------------- | :---------------------------------------------- |
| `...funcs` | [`unknown`, `unknown`, ...unknown[]] | The functions or boolean values to be combined. |

#### Returns

`T`

- The combined function.

#### Defined in

[core/or.ts:11](https://github.com/kacper-olszanski/boolchain.js/blob/cca7c726b6dd3d7319c5387e40412e9999db9188/lib/core/or.ts#L11)

---

### orAsync

▸ **orAsync**\<`T`\>(`...funcs`): `T`

Combines multiple asynchronous functions or boolean values into a single function.
The resulting function returns `true` if any of the input functions return `true` or any of the input boolean values are `true`.
Otherwise, it returns `false`.

#### Type parameters

| Name | Type                                | Description                      |
| :--- | :---------------------------------- | :------------------------------- |
| `T`  | extends `BoolchainAsyncType`\<`T`\> | The type of the input functions. |

#### Parameters

| Name       | Type                                 | Description                            |
| :--------- | :----------------------------------- | :------------------------------------- |
| `...funcs` | [`unknown`, `unknown`, ...unknown[]] | The input functions or boolean values. |

#### Returns

`T`

- The combined function.

#### Defined in

[core/or.ts:38](https://github.com/kacper-olszanski/boolchain.js/blob/cca7c726b6dd3d7319c5387e40412e9999db9188/lib/core/or.ts#L38)

---

### xor

▸ **xor**\<`T`\>(`...funcs`): `T`

Performs an exclusive OR (XOR) operation on the provided functions.
Returns a new function that returns true if an odd number of the provided functions return true,
and false otherwise.

#### Type parameters

| Name | Type                           | Description                |
| :--- | :----------------------------- | :------------------------- |
| `T`  | extends `BoolchainType`\<`T`\> | The type of the functions. |

#### Parameters

| Name       | Type                                 | Description                                    |
| :--------- | :----------------------------------- | :--------------------------------------------- |
| `...funcs` | [`unknown`, `unknown`, ...unknown[]] | The functions to perform the XOR operation on. |

#### Returns

`T`

- A new function that performs the XOR operation.

#### Defined in

[core/xor.ts:16](https://github.com/kacper-olszanski/boolchain.js/blob/cca7c726b6dd3d7319c5387e40412e9999db9188/lib/core/xor.ts#L16)

---

### xorAsync

▸ **xorAsync**\<`T`\>(`...funcs`): `T`

Performs an exclusive OR (XOR) operation on the results of multiple asynchronous functions.

#### Type parameters

| Name | Type                                | Description                            |
| :--- | :---------------------------------- | :------------------------------------- |
| `T`  | extends `BoolchainAsyncType`\<`T`\> | The type of the asynchronous function. |

#### Parameters

| Name       | Type                                 | Description                         |
| :--------- | :----------------------------------- | :---------------------------------- |
| `...funcs` | [`unknown`, `unknown`, ...unknown[]] | An array of asynchronous functions. |

#### Returns

`T`

A new asynchronous function that performs the XOR operation on the results of the input functions.

#### Defined in

[core/xor.ts:27](https://github.com/kacper-olszanski/boolchain.js/blob/cca7c726b6dd3d7319c5387e40412e9999db9188/lib/core/xor.ts#L27)