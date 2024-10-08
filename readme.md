# Discord Bot for a kill count of the top 20 players on a HLL Server running CRCON

This Discord bot tracks and ranks the top 20 players based on their kill counts in one hll game round for the whole day.
It fetches player data from the HLL CRCON API and posts the top 20 players to a specified Discord channel.

## Features

- Fetches detailed player data from HLL CRCON API.
- Summarizes the top 20 players based on their kill counts.
- Sends updates to a designated Discord channel.
- Automatically updates Discord every 15 seconds.


## Setup

### Prerequisites

- Node.js (v18 or newer)
- npm (Node Package Manager)
- A Discord bot token
- HLL CRCON API credentials for fetching player data

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/s1lence-aut/hll-top-killer-of-the-day.git
   cd hll-top-killer-of-the-day

2. Generate a .env File

Note: RCON_API_BASE_URL_1 should be like http://<your_vps_ip>:8010 (where 8010 is a port of your CRCON server)

EXAMPLE:

   ```bash
   DISCORD_TOKEN=your_discord_bot_token
   DISCORD_CHANNEL_ID=your_discord_channel_id
   RCON_API_SERVER_NAME_1=your_server_name
   RCON_API_BASE_URL_1=your_api_base_url
   RCON_API_TOKEN_1=your_api_token
   RCON_API_SERVER_NAME_2=your_server_name
   RCON_API_BASE_URL_2=your_api_base_url
   RCON_API_TOKEN_2=your_api_token
   RESTART_TIME=04:00 (UTC)

Support multiple servers by appending _X to their respective fields, where X is a number.

If you have the old version: It is required to update the single server setups to append _1 to the end of these fields.

   
### File Format

This project uses ES Modules and is structured with the `.mjs` file extension.
