# From Vulkan to Raylib: My Path Back into Game Development

Hi, I’m Jonathan. After a long break, I’m working my way back into games development. My goal is simple: finish good games and actually release them.

A while back I read that a solid way to get back into it is to complete three games. The first should be something basic — so I made **[bloc](https://github.com/jonathan-slark/bloc)**, a falling block puzzler with levels, sound, music, high scores and menus. It’s nothing revolutionary, but I finished it. That felt good.

Then life happened and I took a break.

When I returned, I wanted to rethink *how* I was building games. My first game used plain C89 and SDL1. I like C — it’s a small language I can keep in my head. I’ve tried C++ but kept trying to force OOP patterns where they didn’t belong.

So the question became: how low can I go?

I tried **[Vulkan](https://github.com/jonathan-slark/vulkan-triangle)**. I completed a triangle demo… and wow, it’s brutal unless you actually want to be a graphics programmer. I was just making a mess of myself.

Next I tried **[OpenGL](https://github.com/jonathan-slark/opengl_triangle)**. Much more reasonable. I did the triangle demo and used it for my second game — **[Break Bricks](https://github.com/jonathan-slark/break-bricks)**, a modern breakout-style game with a custom batched renderer. It was a much bigger challenge than I expected. Writing your own graphics engine is hard. Nothing kills motivation faster than spending hours debugging just to get a black screen.

At this point I had a realisation: unless your dream is to be a graphics programmer, building a full engine from scratch is probably not the best use of your time as a solo dev.

Enter **Raylib**. It’s simple, easy to use, and gets out of the way. For my third game, **Mythic Dash**, I switched to Raylib so I could finally focus on gameplay, polish, and actually finishing the damn thing.

Mythic Dash started as a simple maze runner using Shade’s excellent Southeast Asian myth assets. It evolved into a hybrid arcade dungeon dash with multiple difficulty levels and progression. I’m really happy with how it turned out.

---

### Looking Ahead

I’ve got plenty of ideas for the next game. The hard part, as always, is picking something achievable in a reasonable timeframe. But I’m in a much better place now — I have a workflow that lets me actually ship games instead of fighting technology.

If you’re a solo dev, aspiring game programmer, or just curious about the journey from low-level graphics experiments to “I just want to make games” — feel free to say hi!
