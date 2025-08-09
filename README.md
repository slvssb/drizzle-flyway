# Drizzle Gateway on Fly.io ❤️

Deploy [Drizzle Gateway](https://gateway.drizzle.team) on [Fly.io](https://fly.io) with persistent storage.

> **Note**: The required volume for persistent storage will be created automatically during deployment.

## Setup

1. **Launch the app**:

   ```bash
   fly launch --copy-config
   ```

2. **Set environment variables**:

   ```bash
   fly secrets set MASTERPASS=your_master_password
   ```

3. **Deploy** (volume will be auto-created):

   ```bash
   fly deploy
   ```

4. **Access**: Your gateway will be available at `https://your-app-name.fly.dev`

## Environment Variables

- `MASTERPASS` - Master password for admin access
- `PORT` - Port number (default: 8080)
- `STORE_PATH` - Storage path (default: /app)

That's it! 🚀
