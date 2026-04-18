# Will You Be My Girlfriend?

A cute, funny, and interactive web page to ask someone to be your girlfriend. Built to make it *almost* impossible to say no.

**[Live Demo](https://lucifer-22.github.io/willyoubemygirlfriend/)**

## How It Works

The page takes you through a multi-phase experience:

1. **The Setup** — A shy typewriter intro: *"Hey... can we talk?"* — builds suspense without giving anything away.
2. **The Question** — Reveals *"Will you be my girlfriend?"* with Yes and No buttons. The No button starts dodging your cursor after 2 hovers, sliding away with escalating guilt-trip text.
3. **The Convincing** — If they manage to click No, it enters a debate mode with 8 funny arguments presented one by one (unlimited hoodies, no judgment on 3am snacks, carrying all grocery bags in one trip, etc.). A progress bar fills up. The Yes button grows. The No button shrinks and fades.
4. **The Celebration** — Heart-shaped confetti explosions, floating emoji hearts, and a funny victory message.

## Features

- **Dodging No button** — slides away from your cursor so you can't click it
- **Escalating guilt text** — *"Are you sure??"* → *"You're breaking my heart..."*
- **Convincing debate mode** — 8 funny reasons with a progress bar
- **Growing Yes / shrinking No** — visual pressure that gets funnier each round
- **Heart confetti** — pink heart-shaped confetti explosion on Yes
- **Phase transitions** — background gradient shifts per phase (pink → orange → green)
- **Floating hearts** — ambient emoji hearts floating in the background
- **Typewriter intro** — suspenseful reveal animation
- **Fully responsive** — works on desktop and mobile
- **Zero dependencies to install** — just HTML, CSS, and vanilla JS

## Getting Started

```bash
git clone https://github.com/Lucifer-22/willyoubemygirlfriend.git
```

Open `index.html` in your browser. That's it — no build step needed.

## Project Structure

```
willyoubemygirlfriend/
├── index.html       # The entire app (HTML + CSS + JS)
├── images/
│   ├── image1.gif   # Valentine bear (unused reserve)
│   ├── image2.gif   # Shy sparkly cat (intro + convincing)
│   ├── image3.gif   # Crying cat (convincing)
│   ├── image4.gif   # Sad panda (question phase)
│   ├── image5.gif   # Peeking character (convincing)
│   ├── image6.gif   # Sad corner character (convincing)
│   └── image7.gif   # Happy couple cats (celebration)
└── README.md
```

## Customization

| What | Where | How |
|------|-------|-----|
| Intro text | `<span class="typewriter">` | Change the typewriter message |
| Convincing arguments | `reasons` array in JS | Edit the funny texts |
| No button messages | `noTexts` array in JS | Change the guilt-trip escalation |
| Celebration messages | `celebrationMessages` array in JS | Edit the victory notes |
| GIF images | `images/` folder | Replace with your own GIFs |
| Background colors | `.phase-*` classes in CSS | Change the gradient hex codes |
| Confetti colors | `colors` array in `fireConfetti()` | Swap in any hex codes |
| Dodge speed | `.btn-no.dodge` transition in CSS | Adjust the `0.8s` duration |
| Dodge range | `rangeX` / `rangeY` in `dodge()` | Change the pixel values |

## Technologies

- HTML5
- CSS3 (animations, gradients, glassmorphism)
- Vanilla JavaScript
- [canvas-confetti](https://www.npmjs.com/package/canvas-confetti) via CDN

## License

Do whatever you want with it. Go get 'em.
