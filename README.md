# Velvora – scroll landing page

React + Vite, GSAP ScrollTrigger and Lenis smooth scroll. 52 frames play on a full screen canvas while you scroll.

## Run
```bash
npm install
npm run dev      # open the local URL it prints
npm run build    # production build in /dist
```

## Where things are
```
public/frames/        frame-001.webp ... frame-052.webp   (the images)
src/data/content.js   ALL text, notes, timings, email  (edit copy here)
src/components/       Nav, Story (canvas + scroll), Beats, Longevity, Footer, Words
src/hooks/            useFrames (preload), useReveal (fade-in on scroll)
src/styles/           global, story, longevity, footer, reveal (.css)
```

## Common changes
- **Text / email / notes**: `src/data/content.js`
- **Scroll speed**: `#story { height: 800vh }` in `src/styles/story.css` (bigger = slower)
- **Different frames**: replace the files in `public/frames/` (keep the `frame-001.webp` naming) and set `FRAME_COUNT` in `content.js`
- **Colours**: the variables at the top of `src/styles/global.css`
