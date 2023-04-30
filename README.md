# Tonic Events

## Usage

`https://raw.githubusercontent.com/tonic-cash/tonic-events/main/${hexifiedChainIdWith0xPrefix}/${lowerCasedContractAddress}.json`

- `fromBlock`: `number`
- `endBlock`: `number`
- `events`
  - `returnValues`
    - `0`
    - `1`
    - `2`
    - `commitment`
    - `leafIndex`
    - `timestamp`
  - `blockNumber`: `number`

## Benchmark
(fetching all events `contract.getPastEvents` w/ binary search vs using archived events)

```
...
**** { avgOldTime: 25336.8, avgNewTime: 214.5, times: 118.12027972027971 }
✨  Done in 261.91s.
```

25.34s vs 0.214s, that's roughly **118.12 times** faster!
