

# DISCORD CLONE
It is a Discord clone focusing on real-time messaging with attachments, message editing, and deletion. It supports text, audio, and video calls, including 1:1 conversations and video calls between members. The platform includes robust member management, an advanced invite system, and a modern UI with TailwindCSS and ShadcnUI, featuring Light and Dark mode themes. Built for scalability, it utilizes Prisma ORM with a MySQL database hosted on Aiven.io and ensures secure authentication through Clerk.


## Features

- Ability to send attachments as messages using UploadThing
- Real-time message editing and deletion capabilities for all users
- Establishment of Text, Audio, and Video call Channels
- Support for 1:1 conversations between members
- Enable 1:1 video calls between members
- Comprehensive member management functionalities including Kick and Role changes (Guest/Moderator)
- Implementation of a unique invite link generation system and fully functional invite mechanism
- Infinite message loading in batches of 10 using tanstack/query
- Creation and customization of servers
- Implementation of a visually appealing UI using TailwindCSS and ShadcnUI
- Full responsivity and mobile-friendly UI design
- Support for Light and Dark mode themes
- Websocket fallback mechanism: Polling with alerts
- Integration of ORM using Prisma for database operations
- Utilization of MySQL database provided by Aiven.io
- Implementation of authentication mechanisms using Clerk

 
## Getting Started

Instructions on setting up your project locally. To get a local copy up and running, follow these steps.

### Prerequisites

**Node version 18.x.x**

### Cloning the repository

```shell
git clone https://github.com/Deepcoders30/Discord-Clone.git
```

### Install packages

```shell
npm i
```

### Setup .env file

```js
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=
NEXT_PUBLIC_CLERK_SIGN_UP_URL=
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=


DATABASE_URL=

UPLOADTHING_SECRET=
UPLOADTHING_APP_ID=

LIVEKIT_API_KEY=
LIVEKIT_API_SECRET=
NEXT_PUBLIC_LIVEKIT_URL=
```

### Setup Prisma

Add MySQL Database (I used Aiven.io MySQL Database)

```shell
npx prisma generate
npx prisma db push

```

### Start the app

```shell
npm run dev
```

## Available commands

Running commands with npm `npm run [command]`

| command | description                              |
| :------ | :--------------------------------------- |
| `dev`   | Starts a development instance of the app |




