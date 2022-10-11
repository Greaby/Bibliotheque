---
authors: [Angus Russell]
type: [Article]
category: [Tech]
tag: ["Stable diffusion", "text to image", "AI art", "Dall-e", NightCafe]
---

# How to use Stable Diffusion to generate images from a text prompt

https://medium.com/nightcafe-creator/stable-diffusion-tutorial-how-to-use-stable-diffusion-157785632eb3

Stable Diffusion is the hottest new algorithm in the AI art world. In this article I’ll give it a brief introduction, then get straight into “how can I use it”?

But, before I do either of those things, here’s a sample of the types of images you can create with Stable Diffusion, just to whet your appetite.

One year ago — almost to the day — I published an article “How to use VQGAN+CLIP to generate images from a text prompt”. It’s incredible to think that in that year, images generated using completely open-source AI algorithms and models have gone from this:
VQGAN+CLIP generated images. The state of the art in AI image generation just 1 year ago. They’re beautiful, but not particularly coherent.

To this:
Stable diffusion generated images. State of the art open-source AI text-to-image algorithm. Beautiful AND coherent.

Yes, Stable Diffusion is pretty incredible, and is undeniably the new darling of the AI art world, but what is it and who developed it?
What is Stable Diffusion?

Stable Diffusion is an algorithm developed by Compvis (the Computer Vision research group at Ludwig Maximilian University of Munich) and sponsored primarily by Stability AI, a startup that aims to be the driving-force behind a grass-roots, open-source AI revolution. The algorithm itself builds on ideas from Open AI’s DALL-E 2, Google’s Imagen and other image generation models, with a lot of optimisations on top.

Stability AI employ Katherine Crowson as their lead coder. If you haven’t heard the name, Katherine is one of the main driving forces behind the AI art explosion in the last 1.5 years. She was the first to combine VQGAN with OpenAI’s CLIP, and then she went on to develop the CLIP-Guided diffusion method underpinning Disco Diffusion, NightCafe and various other AI image generation websites.

Stable Diffusion is a bit different to those algorithms in that it is not “CLIP-Guided”. Instead, a version of CLIP is “Frozen” and embedded into the generation algorithm itself. This is an idea borrowed from Imagen, and makes stable diffusion a LOT faster than it’s CLIP-guided ancestors.

Incredibly, compared with DALL-E 2 and Imagen, the Stable Diffusion model is a lot smaller. While DALL-E 2 has around 3.5 Billion parameters, and Imagen has 4.6 Billion, the first Stable Diffusion model has just 890 million parameters, which means it uses a lot less VRAM and can actually be run on consumer-grade graphics cards.
How to use Stable Diffusion

Stable Diffusion is open source, so there are a few different ways you can use it. But, since I work at NightCafe, I’m going to show you how to use NightCafe to create images with Stable Diffusion. Before I do, even though I’m a little biased, I’ll outline why I think NightCafe is the best place to try Stable Diffusion. Don’t care about this? Feel free to skip ahead.

Why use NightCafe for Stable Diffusion

    It’s free to try. On NightCafe you get 5 free credits every day, and you can also earn credits by doing simple things like sharing your creations and participating in the community.
    It has a very simple interface for beginners, and more control available for advanced users.
    Your images are all saved to your account.
    It’s easy to duplicate and tweak your images. You can even duplicate and tweak other people’s images.
    You can save your favourite prompts and modifiers, then quickly add them to future generations.
    You can organise your creations into collections.
    There’s a whole community of users doing the same thing, learning together, sharing their creations and giving you constructive feedback!

Stable Diffusion on NightCafe

NightCafe is an online AI-powered Art Generator. It provides the means to run algorithms like Neural Style Transfer, VQGAN+CLIP, CLIP-Guided Diffusion, and now Stable Diffusion — without needing any technical knowledge or coding skills.

To start your AI image generation journey, go to this page → Stable Diffusion on NightCafe. You’ll see a page that looks something like this.
Create images using Stable Diffusion on NightCafe

This is a mini version of the normal creation form on NightCafe. It’s a really easy way to get started, so as your first step on NightCafe, go ahead and enter a text prompt (or click “Random” for some inspiration), choose one of the 3 styles, and click “Create” (the button underneath the styles, not in the main menu).
You’ll see something like this when your creation is ready. I used the prompt “Ruins of a medieval castle” and the “Matte” style.

As I mentioned earlier, Stable Diffusion is fast, so your creation will be ready in less than a minute. If you’re new to AI image generation, that might not seem fast, but previous algorithms took a LOT longer than that. Congratulations! You just made your first Stable Diffusion artwork.

I also mentioned earlier that you were using the mini version of the creation form. Now it’s time to try the full version, where you have a lot more control. Click “Create” in the main menu, then choose the “Stable” algorithm (or click here to go straight there). You’ll arrive at a page that looks like this:
How to create a Stable Diffusion artwork on NightCafe

There’s not too much more on this page other than more styles to choose from. Feel free to try another prompt with a different style, or just move on to the next section — Advanced Options.
Advanced Stable Diffusion Options on NightCafe

Go back to the create → Stable page again if you’re not still there, and right at the top of the page, activate the “Show advanced options” switch. Now you’ll see a page that looks like this:
Advanced Create Mode — Stable Diffusion on NightCafe

As you can see, you now have a lot more options in front of you! Go ahead and enter another text prompt, but then — wait — where did the styles go?

Fear not — the preset styles are just a tool for beginners to more easily create beautiful artworks. Without them, the output images are generally more like photos than artworks. Instead of presets, the advanced mode has that single little “Add Modifiers” button. Click on that and you’ll see this popup:

Hey look, there are our presets again! Except now if you click on one, it just adds some words to your text prompt. Confused? I can settle your confusion. In non-advanced mode, all that the preset styles actually do is add these words to your prompt behind the scenes! In advanced mode, clicking a preset adds it to your prompt, so you can still tweak it to your liking, or even use multiple presets at once!

There are other tabs in this popup though, too. Under “Modifiers” you’ll find a long list of more basic, low-level modifiers that you can combine as you wish to create your own styles, all with minimal typing (or even thinking).

Once you’ve added you’re keyword modifiers to your prompt, we’ll move on to the other settings. I’ll quickly summarise each, though many of them are self-explanatory.

Seed — The seed is just a number that controls all the randomness that happens during the generation. By using the same seed and the same settings in two different generations, you’ll get the same output. But, if you change only the seed, you’ll get a completely different output. You might find this useful later. For now, just leave it as-is.

Aspect ratio — Aspect ratio is self-explanatory, however it’s worth mentioning that the Stable Diffusion algorithm was trained on square images, and is therefore better at generating square (or close to square) images than it is at generating rectangular images.

Prompt weight — Prompt weight is a variable supplied to the algorithm which tells it how much importance to give to the prompt. In other stable diffusion tools, it is often referred to as cfg_scale.

Number of images — Self-explanatory, but please note that more images will cost you more credits!

Sampling method — The sampling methods listed here are just different ways to run the algorithm on the back end. For the most part, they yield barely imperceptible differences. Leave it on the default for now — you’re much better off experimenting with other parameters before this one.

Runtime — You have the option to run the algorithm for longer, which in some cases will improve the result. However, longer runtime also costs more, and the lowest runtime is usually enough.

Output resolution — Even though Stable Diffusion was trained on square images at a resolution of 512x512, you can choose to output at larger resolutions. Please note though: higher resolutions cost more credits, and are often worse due to how Stable Diffusion was trained.

After choosing your options and before clicking “Create”, take note of how many credits your generation is going to consume. If you want to figure out why it costs more than 1 credit (the default), you can click on “Show breakdown” to see exactly how credit costs are calculated. Remember, single-credit creations are generally very good, so it’s worth experimenting with the cheapest settings before moving on to more expensive ones.
What’s next?

Now that you’re making (hopefully) incredible art with Stable Diffusion, what’s next? Well, you can do whatever you like, but here are some suggestions.

    Publish your favourite pieces to the NightCafe community.
    Browse the NightCafe explore page to see what other people are creating.
    Follow your favourite creators and keep track of them on your personal feed.
    Enhance your favourite creations. NightCafe’s “Enhance” option uses another AI algorithm to upscale your creation to very high resolution while keeping sharp edges and detail.
    Download your creations and do whatever the hell you want with them. NightCafe gives you complete ownership, so you can put them on a t-shirt, sell them as prints or NFTs, use it as a cover for your band’s upcoming album, etc.
