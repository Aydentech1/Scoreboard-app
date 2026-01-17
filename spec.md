# Scoreboard App

## Overview
A real-time scoreboard application that supports basketball and volleyball games with separate display and control interfaces.

## Core Features

### Scoreboard Management
- Users can create new scoreboards by providing a name and selecting sport type (basketball or volleyball)
- All scoreboards are stored in the backend with their configuration and current state
- Users can browse and select from existing scoreboards

### Display and Control Modes
- When selecting a scoreboard, users choose between "Display" or "Control" mode
- **Display Mode**: Shows live scoreboard view with current scores, team names, and game state
- **Control Mode**: Allows updating scores, team names, and managing game state (start, stop, reset)

### Sport-Specific Features

#### Basketball
- Track scores for two teams
- Display current quarter
- Show game timer
- Control timer (start, stop, reset)

#### Volleyball  
- Track sets won by each team
- Display points for current set
- Show set history
- Track total sets played

### Real-time Synchronization
- All changes made in control mode instantly appear in display mode
- Multiple users can view the same scoreboard simultaneously
- Backend stores and broadcasts all scoreboard updates

## Backend Data Storage
- Scoreboard configurations (name, sport type, team names)
- Current game state (scores, timer, quarter/set information)
- Real-time state synchronization across all connected clients

## User Interface
- Clean, responsive design that works on desktop and mobile
- Sport-specific layouts optimized for each game type
- Large, readable fonts suitable for display screens
- Intuitive controls for game management
- Application content displayed in English

## Deployment Configuration
- Frontend optimized for Vercel deployment using Vite build system
- Single Page Application (SPA) routing configuration with fallback to index.html
- Production environment variables configured for Internet Computer backend canister connection
- Package.json scripts optimized for Vercel build and deployment process
