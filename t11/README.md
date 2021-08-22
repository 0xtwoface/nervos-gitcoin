## TASK11 - Use A Tron Wallet To Execute A Smart Contract Call

### 1- Screenshot of the accounts you created

<img src="https://github.com/0xtwoface/nervos-gitcoin/blob/master/t11/accounts.png" />

### 2- A link to the Layer 1 address you funded on the Testnet Explorer

<a href="https://explorer.nervos.org/aggron/address/ckt1qyq9e3j2pp5y9u0hmufn2tfgrszjr0guy8fs87rk98"> Explorer Link </a>

### 3- Screenshot of the console output, CKByte deposit to your Tron account on Layer 2

<img src="https://github.com/0xtwoface/nervos-gitcoin/blob/master/t11/deposit.png" />

### 4- Screenshot of the console output, smart contract calls on Layer 2

- Steps: Playlist with id 1 called. Added a new song to that playlist. Playlist's <b>songs</b> parameter changed

<img src="https://github.com/0xtwoface/nervos-gitcoin/blob/master/t11/contract-call.png"/>

### 5- The transaction hash of the "Contract call"

```bash
0x2af5cb775f5bd8659f63e77ac9f0502977402aed6bf8b60c3ba82089a74928c0
```

### 6- The contract address that you called


```bash
 0xAFb93EF21bC061a88afB539d5fdD926DB942869A
```

### 7- The ABI for contract you made a call on

```javascript
[
    {
      "inputs": [],
      "stateMutability": "nonpayable",
      "type": "constructor"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": false,
          "internalType": "uint256",
          "name": "id",
          "type": "uint256"
        },
        {
          "indexed": false,
          "internalType": "string",
          "name": "name",
          "type": "string"
        },
        {
          "indexed": false,
          "internalType": "address",
          "name": "creator",
          "type": "address"
        },
        {
          "indexed": false,
          "internalType": "uint256",
          "name": "songs",
          "type": "uint256"
        }
      ],
      "name": "PlaylistCreated",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": false,
          "internalType": "uint256",
          "name": "id",
          "type": "uint256"
        },
        {
          "indexed": false,
          "internalType": "uint256",
          "name": "playlistId",
          "type": "uint256"
        },
        {
          "indexed": false,
          "internalType": "string",
          "name": "name",
          "type": "string"
        },
        {
          "indexed": false,
          "internalType": "address",
          "name": "creator",
          "type": "address"
        }
      ],
      "name": "SongAdded",
      "type": "event"
    },
    {
      "inputs": [
        {
          "internalType": "uint256",
          "name": "",
          "type": "uint256"
        }
      ],
      "name": "playlists",
      "outputs": [
        {
          "internalType": "uint256",
          "name": "id",
          "type": "uint256"
        },
        {
          "internalType": "string",
          "name": "name",
          "type": "string"
        },
        {
          "internalType": "address",
          "name": "creator",
          "type": "address"
        },
        {
          "internalType": "uint256",
          "name": "songs",
          "type": "uint256"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "uint256",
          "name": "",
          "type": "uint256"
        }
      ],
      "name": "songs",
      "outputs": [
        {
          "internalType": "uint256",
          "name": "id",
          "type": "uint256"
        },
        {
          "internalType": "uint256",
          "name": "playlistId",
          "type": "uint256"
        },
        {
          "internalType": "string",
          "name": "name",
          "type": "string"
        },
        {
          "internalType": "address",
          "name": "creator",
          "type": "address"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "totalPlaylist",
      "outputs": [
        {
          "internalType": "uint256",
          "name": "",
          "type": "uint256"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "totalSong",
      "outputs": [
        {
          "internalType": "uint256",
          "name": "",
          "type": "uint256"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "string",
          "name": "_name",
          "type": "string"
        }
      ],
      "name": "createPlaylist",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "string",
          "name": "_name",
          "type": "string"
        },
        {
          "internalType": "uint256",
          "name": "_playlistId",
          "type": "uint256"
        }
      ],
      "name": "addSongToPlaylist",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "uint256",
          "name": "_playlistId",
          "type": "uint256"
        }
      ],
      "name": "getPlaylistSongs",
      "outputs": [
        {
          "components": [
            {
              "internalType": "uint256",
              "name": "id",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "playlistId",
              "type": "uint256"
            },
            {
              "internalType": "string",
              "name": "name",
              "type": "string"
            },
            {
              "internalType": "address",
              "name": "creator",
              "type": "address"
            }
          ],
          "internalType": "struct Playlists.Song[]",
          "name": "",
          "type": "tuple[]"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    }
  ]

```

### 8- Your Tron address 

```bash
TEYBKzteoZFo1bQkTLUep2N9BY7peAnTPW
```
