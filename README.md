# mint Token
This project provides mint piggy token interface built on Farcaster Frames. Users can mint to. The project also includes integration with BlockScout to view transaction details.

# Installation
1. Clone the repository
```
git clone git@github.com:goftok/hackathon5.git
```

2. Install dependencies and run the project
```
yarn install
```

3. Run the development server:

```
yarn dev
```

3. Open the dev env:

```
http://localhost:<port>/api/dev
```


### Main Components
**FrogUI**: This project uses FrogUI to create a dynamic interface for ENS registration.
**Warpcast**: Integrates with Warpcast Frames.
**BlockScout**: Provides transaction tracking capabilities.

## mintTO Process
1. press the mint button:

Call the mintTo function with contract.
```
return c.contract({
    ...
    abi: [],
    functionName: 'mintTo',
    args: [address, 1n],
    ...
})
```

2. DO Transaction:

3. Success:

Users receive confirmation of a successful mint token and can view the transaction on BlockScout.

## Connect with fatcaster
### hub
Use pinata:

```
import { pinata } from 'frog/hubs'

hub: pinata()
```
### ngrok
Forwarding:

```
ngrok config add-authtoken <your authtoken>
ngrok http http://localhost:<port>
```
ngrok website: [https://ngrok.com/]
