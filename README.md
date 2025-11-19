# Flag Football Play Lab

A professional-grade, browser-based play designer for 5-on-5 flag football. Create, organize, and share your playbook with an intuitive drag-and-drop interface, route drawing tools, and AI-powered coaching insights.

## Features

- **Interactive Play Designer**: Drag-and-drop players, draw custom routes, and visualize plays on a realistic field
- **Quick Route Templates**: Pre-built route patterns (Fly, Slant, Out, In, Corner, Post, Hitch, Flat, Wheel)
- **Playbook Management**: Save, organize, duplicate, and delete plays
- **AI Coach**: Get strategic insights and coaching tips powered by Gemini AI
- **Export Plays**: Download plays as SVG images for sharing or printing
- **Responsive Design**: Works seamlessly on desktop and mobile devices

## Tech Stack

- **React** - UI framework
- **TypeScript** - Type safety
- **Vite** - Build tool and dev server
- **Tailwind CSS** - Styling
- **Lucide React** - Icon library
- **Google Generative AI (Gemini)** - AI coaching insights

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/xmChen24/flag-football-play-lab.git
   cd flag-football-play-lab
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env.local` file in the root directory and add your Gemini API key:
   ```
   GEMINI_API_KEY=your_api_key_here
   ```

   You can also copy the example file and edit it:
   ```bash
   cp .env.example .env.local
   ```

4. Start the development server:
   ```bash
   npm run dev
   ```

5. Open your browser and navigate to `http://localhost:5173`

## Usage

### Creating a New Play

1. Click "New Play" from the playbook view
2. Drag players to position them on the field
3. Click a player to select it, then click on the field to draw route points
4. Use the Quick Routes panel for common route patterns
5. Add defenders using the "Add Defense" button
6. Save your play and add tags for organization

### AI Coaching

Click "Ask AI Coach" to get strategic insights about your play, including:
- Coverage vulnerabilities
- Route combinations
- Defensive matchup analysis
- Suggested adjustments

### Exporting Plays

Click the Download button in the editor to export your play as an SVG image.

## Project Structure

```
flag-football-play-lab/
├── components/          # React components
│   └── Field.tsx       # Main field canvas component
├── services/           # Business logic and services
│   ├── storage.ts      # LocalStorage playbook management
│   └── geminiService.ts # AI integration
├── App.tsx             # Main application component
├── types.ts            # TypeScript type definitions
└── index.tsx           # Application entry point
```

## Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

MIT

## Acknowledgments

Built with passion for flag football coaches and players looking to elevate their game.
