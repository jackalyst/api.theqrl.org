# qrllegacy.proto


<a name="BKData"/>


## BKData

```python
   
```

```javascript
   
```


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| mrData | [MRData](#MRData) |  |  |
| block | [Block](#Block) |  |  |


<a name="FBData"/>

## FBData

```python
   
```

```javascript
   
```


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| index | [uint64](#uint64) |  |  |


<a name="LegacyMessage"/>

## LegacyMessage

```python
   
```

```javascript
   
```


Adding old code to refactor while keeping things working


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| func_name | [LegacyMessage.FuncName](#LegacyMessage.FuncName) |  |  |
| noData | [NoData](#NoData) |  |  |
| veData | [VEData](#VEData) |  |  |
| plData | [PLData](#PLData) |  |  |
| pongData | [PONGData](#PONGData) |  |  |
| mrData | [MRData](#MRData) |  |  |
| block | [Block](#Block) |  |  |
| fbData | [FBData](#FBData) |  |  |
| pbData | [PBData](#PBData) |  |  |
| bhData | [BlockHeightData](#BlockHeightData) |  |  |
| txData | [Transaction](#Transaction) |  |  |
| mtData | [Transaction](#Transaction) |  |  |
| tkData | [Transaction](#Transaction) |  |  |
| ttData | [Transaction](#Transaction) |  |  |
| ltData | [Transaction](#Transaction) |  |  |
| slData | [Transaction](#Transaction) |  |  |
| ephData | [EncryptedEphemeralMessage](#EncryptedEphemeralMessage) |  |  |
| syncData | [SYNCData](#SYNCData) |  |  |
| chainStateData | [NodeChainState](#NodeChainState) |  |  |
| nodeHeaderHash | [NodeHeaderHash](#NodeHeaderHash) |  |  |
| p2pAckData | [P2PAcknowledgement](#P2PAcknowledgement) |  |  |



<a name="MRData"/>

## MRData

```python
   
```

```javascript
   
```


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| hash | [bytes](#bytes) |  | FIXME: rename this to block_headerhash |
| type | [LegacyMessage.FuncName](#LegacyMessage.FuncName) |  | FIXME: type/string what is this |
| stake_selector | [bytes](#bytes) |  |  |
| block_number | [uint64](#uint64) |  |  |
| prev_headerhash | [bytes](#bytes) |  |  |
| reveal_hash | [bytes](#bytes) |  |  |



<a name="NoData"/>

## NoData

```python
   
```

```javascript
   
```

<a name="PBData"/>

## PBData

```python
   
```

```javascript
   
```


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| block | [Block](#Block) |  |  |


<a name="PLData"/>

## PLData

```python
   
```

```javascript
   
```


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| peer_ips | [string](#string) | repeated |  |
| public_port | [uint32](#uint32) |  |  |



<a name="PONGData"/>

## PONGData

```python
   
```

```javascript
   
```


<a name="SYNCData"/>


## SYNCData

```python
   
```

```javascript
   
```


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| state | [string](#string) |  |  |



<a name="VEData"/>

## VEData

```python
   
```

```javascript
   
```


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| version | [string](#string) |  |  |
| genesis_prev_hash | [bytes](#bytes) |  |  |
| rate_limit | [uint64](#uint64) |  |  |



<a name="LegacyMessage.FuncName"/>

## LegacyMessage.FuncName

```python
   
```

```javascript
   
```


| Name | Number | Description |
| ---- | ------ | ----------- |
| VE | 0 | Version |
| PL | 1 | Peers List |
| PONG | 2 | Pong TODO: Obsolete |
| MR | 3 | Message received |
| SFM | 4 | Send Full Message |
| BK | 5 | Block |
| FB | 6 | Fetch request for block |
| PB | 7 | Push Block |
| BH | 8 | Block Height |
| TX | 9 | Transfer Transaction |
| LT | 10 | Lattice Transaction |
| EPH | 11 | Ephemeral |
| MT | 12 | Message Transaction |
| TK | 13 | Token Transaction |
| TT | 14 | Transfer Token Transaction |
| SL | 15 | Slave Transaction |
| SYNC | 16 | Add into synced list, if the node replies |
| CHAINSTATE | 17 | Chain State |
| HEADERHASHES | 18 |  |
| P2P_ACK | 19 | P2P Acknowledgement |
