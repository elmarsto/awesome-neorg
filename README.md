# Awesome Neorg

A collection of [Neorg](https://github.com/nvim-neorg/neorg) awesomeness, including config examples and inspo. [Here's the thread where I kicked this here project off.](https://github.com/nvim-neorg/neorg/issues/215).

Contributions accepted delightedly! Throw up a Gist and submit a PR to this repo, adding a link to your gist (or whatever) to the README.md.

## The Collection

### Concealer Presets
Don't want to change each icon individually? Neorg has different presets to automate this for you.
These presets don't exist only for icons, but for markup concealing too!

This snippet will set up your preferred icon or markup preset:
```lua
["core.norg.concealer"] = {
    config = {
        icon_preset = "basic|varied|diamond",
        markup_preset = "safe|brave|dimmed",
    }
}
```

#### Available Presets
Here are all the available icon presets:

- `basic` - the default preset that neorg ships with:

  ![preset-basic](https://user-images.githubusercontent.com/76052559/148407368-6c9c8105-7a6c-47e4-b2a0-ff82d9a50494.png)

- `varied` - a mix n match of several different icon styles:

  ![preset-varied](https://user-images.githubusercontent.com/76052559/148407369-dd1126af-9151-4929-8229-ec8d861a6eb5.png)

- `diamond` - the neorg team's personal favourite! Diamonds, diamonds everywhere:

  ![preset-diamond](https://user-images.githubusercontent.com/76052559/148407374-0d10bf92-9b85-4307-847c-2bd429c3b113.png)

And here are all the available markup presets:

- `safe` - a simple concealing implementation that converts all icons into whitespace.
  this doesn't modify the structure of your text but hides away all of the special characters:

  ![preset-safe](https://user-images.githubusercontent.com/76052559/148408895-2f867396-9822-4b44-98ce-06436351c389.png)

- `brave` - for the people who aren't scared of bugs. This implementation replaces all special characters with word joiners,
  which is known to work only on certain systems. Currently there is no easily controllable concealing in Neovim core,
  [and it may take a while for it to be implemented](https://github.com/neovim/neovim/issues/15706):
  
  ![preset-brave](https://user-images.githubusercontent.com/76052559/148408896-00fa450e-631e-42d7-8169-77cf55885e6b.png)

- `dimmed` - the default concealing method for Neorg. Dims your markup to make it more pleasant to look at:

  ![preset-dimmed](https://user-images.githubusercontent.com/76052559/148408903-d9f86222-df8a-44fb-b188-14ff3c482e7f.png)

# FAQ

### Wot's all this about? 

Neorg is an org-mode-alike for [Neovim](https://github.com/neovim/neovim).

And if you're wondering what _that_ is about, then you're in for a treat :) [Check out Neovim awesomeness here.](https://github.com/rockerBOO/awesome-neovim) 

### Who are you? 

Just a software engineer, helping out of personal interest.  

### What's your relation to the Neorg project? the Neovim Project? 

I'm basically a megafan of Neovim and most of its surrounding ecosystem, especially Neorg.

They said "be the change you want to see in the world," and I wanted to see more Neorg. Like, a *lot* more. 
