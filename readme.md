# Adding SIM Swap Detection to your Web App's 2FA Login Flow with MessageBird Verify & **tru.ID** SIMCheck API

## Requirements

The requirements for this project are:

- [Node.js](https://nodejs.org)
- A [tru.ID Account](https://tru.id)
- A [MessageBird Account](https://dashboard.messagebird.com)

## Getting Started

This project uses MessageBird's [verify-guide](https://github.com/messagebirdguides/verify-guide) as the base in the `starter-files` branch.

Clone the `starter-files` branch via:

```
git clone -b starter-files --single-branch https://github.com/tru-ID/2fa-sim-swap-detection-messagebird.git
```

If you're only interested in the finished code in `main` then run:

```
git clone -b main https://github.com/tru-ID/2fa-sim-swap-detection-messagebird.git
```

Next you need to configure MessageBird's credentials

Copy the values of `example.env` into a `.env` file via:

```
cd 2fa-sim-swap-detection-messagebird && cp example.env .env
```

Open the `.env` file and configure the following values:

- `MESSAGEBIRD_API_KEY`: Your MessageBird API Key Found on [your dashboard](https://dashboard.messagebird.com/en/getting-started/verify)

Next, Create a [tru.ID Account](https://tru.id)

Install the **tru.ID** CLI via:

```bash
npm i -g @tru_id/cli

```

Input your **tru.ID** credentials which can be found within the tru.ID [console](https://developer.tru.id/console)

Create a new **tru.ID** project via:

```
tru projects:create 2fa-with-messagebird
```

configure the following values in your `.env`:

- `TRU_ID_CLIENT`: The client ID found in the `tru.json` file in the newly created **tru.ID** project.
- `TRU_ID_SECRET`: The client secret found in the `tru.json` file in the newly created **tru.ID** project.

## Restoring Dependencies

In order to restore dependencies run:

```bash
npm install
```

## Starting Project

In order to start the project run:

```bash
npm start
```

## References

- [**tru.ID** docs](https://developer.tru.id/docs)
- [MessageBird Verify Guide](https://github.com/messagebirdguides/verify-guide)

## Meta

Distributed under the MIT License. See [LICENSE](https://github.com/tru-ID/2fa-sim-swap-detection-messagebird/blob/main/LICENSE.md)

[**tru.ID**](https://tru.id)
