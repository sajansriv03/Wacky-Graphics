# 🤠 Wacky Wacky West - Online Multiplayer Board Game 🌵

A fully playable online version of the classic board game **Wacky Wacky West** with authentic game graphics, multiplayer support, and smooth drag-and-drop gameplay.

## ✨ Features

- ✅ **Authentic Graphics**: Uses actual photos from your physical game board, pieces, and cards
- ✅ **2-4 Player Multiplayer**: Same-browser multiplayer (open in multiple tabs)
- ✅ **Drag & Drop**: Smooth tile placement with visual feedback
- ✅ **Complete Game Rules**: Secret buildings, voting system, worker placement
- ✅ **Real-Time Updates**: Game state syncs across tabs every second
- ✅ **Responsive Design**: Works on desktop, tablet, and mobile

## 🎮 Game Components

### What's Included:
- **Game Board**: Exact 10x15 grid from your physical board
- **60 Tiles**: Roads, Rivers, Railroads in sizes 1-3 (with bridges)
- **6 Building Types**: General Store (5pts), School (4pts), Saloon/Bank (3pts), Stable (2pts), Jail (1pt)
- **18 Outhouses**: Trigger voting when covered
- **Voting Cards**: Yes (+/++/+++), No (!/!!/!!!), Wildcard, Indifferent
- **4 Workers**: Track building crew positions

## 📦 Deployment Instructions

### Prerequisites
- GitHub account (free)
- Vercel account (free - sign up with GitHub)
- Web browser

### Step 1: Upload to GitHub

1. Go to https://github.com and sign in
2. Click "New repository" (green button)
3. Repository name: `wacky-wacky-west`
4. Make it **Public**
5. Click "Create repository"

6. On your computer, extract the downloaded ZIP file
7. Go to your new GitHub repository page
8. Click "uploading an existing file"
9. Drag ALL these files into the upload area:
   ```
   index.html
   package.json
   vite.config.js
   vercel.json
   src/
     ├── App.jsx
     └── main.jsx
   ```
10. Click "Commit changes"

### Step 2: Deploy to Vercel

1. Go to https://vercel.com
2. Click "Sign Up" → "Continue with GitHub"
3. Authorize Vercel to access your repositories
4. Click "Add New..." → "Project"
5. Find "wacky-wacky-west" and click "Import"
6. **Framework Preset**: Should auto-detect as "Vite"
7. **Build Command**: `npm run build` (should be auto-filled)
8. **Output Directory**: `dist` (should be auto-filled)
9. Click "Deploy" (big blue button)
10. Wait 2-3 minutes for build to complete

### Step 3: Get Your Shareable Link

Once deployment finishes, you'll see:
```
🎉 Congratulations! Your project is deployed!
```

Your link will be something like:
```
https://wacky-wacky-west-abc123.vercel.app
```

Copy this link and share it with friends!

## 🎯 How to Play

### Starting a Game:

1. **Player 1** opens the link
2. Enters their name and clicks "Join Game"
3. **Player 2-4** also open the SAME link
4. Each enters their name and clicks "Join Game"
5. Once 2-4 players have joined, the host clicks "START GAME"

### Gameplay:

1. **Get Your Secret Building**: You'll be assigned a building type to protect
2. **Place Tiles**: Click a tile in your hand, then click a valid green spot on the board
3. **Rotate Tiles**: Click the same tile again to rotate 90°
4. **Covering Outhouses**: When someone tries to cover an outhouse (🚽), all players vote:
   - Green cards = YES (let it be covered)
   - Red cards = NO (save the outhouse!)
   - Yellow Wildcard = Your choice
   - Yellow Indifferent = Abstain
5. **Win Condition**: Keep your secret buildings uncovered! Start at 15 points, lose points for each covered building of your type

### Important Rules:

- **Size-3 tiles with bridges** can cross over same-type tiles (Road over Road, River over River, etc.)
- **Vote card strengths**: One symbol (!, +) = 1 vote, Two (!!, ++) = 2 votes, Three (!!!, +++) = 3 votes
- **Wildcard** = Choose YES or NO with strength 3
- **Game ends** when all tiles are played or no valid moves remain

## 🔧 Troubleshooting

### "Page Not Found" (404 Error)
- Make sure `vercel.json` file is in the repository
- Redeploy from Vercel dashboard

### Build Failed
- Check that ALL files were uploaded to GitHub
- Verify `src` folder contains both `App.jsx` and `main.jsx`
- Make sure file names match exactly (case-sensitive)

### Game Won't Load
- Check browser console for errors (F12 → Console tab)
- Try a different browser (Chrome, Firefox, Safari)
- Clear cache and reload (Ctrl+Shift+R or Cmd+Shift+R)

### Multiplayer Not Working
- All players must open the SAME exact link
- Each player should use a different browser tab
- For true cross-device multiplayer, you'd need to add a backend (Firebase, Supabase)

## 📝 Technical Details

### Built With:
- **React 18**: UI framework
- **Vite**: Build tool and dev server
- **localStorage**: For same-browser multiplayer sync
- **Base64 Images**: All game graphics embedded directly

### File Sizes:
- **Total Bundle**: ~4 MB (mostly images)
- **Game Board**: 1 MB
- **Building Cards**: ~120 KB each
- **Tiles**: ~40-80 KB each
- **Vote Cards**: ~70-100 KB each

### Browser Compatibility:
- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers

## 🚀 Future Enhancements (Optional)

Want to add features? Here are some ideas:

1. **True Cross-Device Multiplayer**: Add Firebase or Supabase backend
2. **Game Lobby System**: Create/join games with unique codes
3. **Undo Button**: Allow players to undo their last move
4. **Game History**: Track all moves and replay games
5. **Animated Tiles**: Add animations when placing tiles
6. **Sound Effects**: Wild west sounds for tile placement and votes
7. **Leaderboard**: Track wins across multiple games

## 📄 License

Personal use only. Based on the physical board game "Wacky Wacky West".

## 🎉 Credits

- **Game Design**: Original Wacky Wacky West creators
- **Graphics**: Your physical game photos
- **Implementation**: Built with React + Vite
- **Deployment**: Vercel

---

**Enjoy rebuilding the wild west town of Rossdorf!** 🏜️🤠

For questions or issues, check the Vercel deployment logs or open a GitHub issue.
