# CommunityConnect - Community Management App

CommunityConnect is a community management application built with Next.js 13, React, Socket.io, Prisma, TailwindCSS, MySQL, and other technologies. It provides a versatile platform for real-time communication, server management, and member interaction.

## Features

- **Real-time Messaging:**
  - Utilizes Socket.io for instant messaging.
  - Send attachments as messages using UploadThing.

- **Communication Channels:**
  - Create Text, Audio, and Video call Channels.
  - 1:1 conversation between members.
  - 1:1 video calls between members.

- **Message Management:**
  - Delete and Edit messages in real-time for all users.
  - Infinite loading for messages in batches of 10 (tanstack/query).

- **Server Management:**
  - Server creation and customization.
  - Member management - Kick, Role change (Guest/Moderator).
  - Unique invite link generation and a fully working invite system.

- **UI/UX:**
  - Beautiful UI using TailwindCSS and ShadcnUI.
  - Full responsiveness and mobile UI.
  - Light/Dark mode support.

- **Websocket Fallback:**
  - Provides a WebSocket fallback with Polling and alerts.

- **Backend and Database:**
  - ORM using Prisma.
  - MySQL database using Planetscale.

- **Authentication:**
  - Authentication with Clerk.

## Environment Variables

Ensure you have the following environment variables set in your `.env` file:

```env
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
### Install Dependencies

```shell
npm i
```

### Setup Prisma

Add a MySQL database.

Run the following commands:

```shell
npx prisma generate
npx prisma db push

```

### Start the app

```shell
npm run dev
```
