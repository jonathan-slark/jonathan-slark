# From Vulkan to SDL3: My Path Back into Game Development

Hi, I’m Jonathan. After a long break, I’m working my way back into games development. My goal is simple: finish good games and actually release them.

A while back I read that a solid way to get back into it is to complete three games. The first should be something basic — so I made **[bloc](https://github.com/jonathan-slark/bloc)**, a falling block puzzler with levels, sound, music, high scores and menus. It’s nothing revolutionary, but I finished it. That felt good.

Then life happened and I took a break.

When I returned, I wanted to rethink *how* I was building games. My first game used plain C89 and SDL1. I like C — it’s a small language I can keep in my head. I’ve tried C++ but kept trying to force OOP patterns where they didn’t belong.

So the question became: how low can I go?

I tried **[Vulkan](https://github.com/jonathan-slark/vulkan-triangle)**. I completed a triangle demo… and wow, it’s brutal unless you actually want to be a graphics programmer. I was just making a mess of myself.

Next I tried **[OpenGL](https://github.com/jonathan-slark/opengl_triangle)**. Much more reasonable. I did the triangle demo and used it for my second game — **[Break Bricks](https://github.com/jonathan-slark/break-bricks)**, a modern breakout-style game with a custom batched renderer. It was a much bigger challenge than I expected. Writing your own graphics engine is hard. Nothing kills motivation faster than spending hours debugging just to get a black screen.

At this point I had a realisation: unless your dream is to be a graphics programmer, building a full engine from scratch is probably not the best use of your time as a solo dev.

Enter **Raylib**. It’s simple, easy to use, and gets out of the way. For my third game, **Mythic Dash**, I switched to Raylib so I could finally focus on gameplay, polish, and actually finishing the damn thing.

Mythic Dash started as a simple maze runner using Shade’s excellent Philippine mythological creature sprites. It evolved into a maze chase hunted by creatures from Philippine folklore — with dungeon-crawler twists like traps, keys and locked doors. It shipped in 2026 — free in the browser — and I’m really happy with how it turned out.

---

### The Fourth Game

Shipping three games taught me a lot, but for the fourth I wanted to stop making learning projects and start building something I actually wanted to play — a real, commercial game. That meant two changes.

First, the technology. Raylib had served me well — it’s raw, lean, and great for getting something on screen fast — but it doesn’t suit the way I like to work. For this game I switched to **SDL3**. I daily-drive Ubuntu, and SDL3’s Wayland support is simply better. More importantly, SDL3 suits my style: solid, reusable code, with stricter error checking to back it up.

Second, the game itself. **Clean Kill** is a top-down zombie shooter with the gunplay of a modern FPS. Your cursor is the gun: land the headshot and it pops — hit-stop, screen shake, and a real 9mm gunshot. A heavy metal soundtrack, two enemy types that force target priority, and a boss you have to learn. No power-ups, no stat grinding — you get better, not the game.

Before committing, I ran a spike test to prove the stack: SDL3 building for Windows, Linux, and the web via Emscripten, with a fixed-timestep loop, sprite rendering, audio mixing, text, and a Tiled level loader. It all worked — and more importantly, it was fun. The gun sounds and soundtrack fit the graphic-novel art perfectly.

Clean Kill is in development now. The coming-soon page is live on itch.io with devlogs, and a free demo is on the way before the full game.

If you’re a solo dev, aspiring game programmer, or just curious about the journey from low-level graphics experiments to “I just want to make games” — feel free to say hi!
