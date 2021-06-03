# How to publish your mod

!!! warning "Obsolete"
    This guide is for versions prior `0.85`. New guide is coming soon.

## Introduction

This step-by-step guide is intended for mod creators who want to feature their creations on the in-game Mod Gallery. Like this:

![20180514-192535](https://user-images.githubusercontent.com/1748681/78776106-042ce200-79a0-11ea-8131-852ba1d15bcc.png)

!!! note
    Current implementation is temporary. After the release of the game on Steam, we will incorporate Steam Workshop support, so the publishing process may change.

## Prepare mod for publishing

### Add preview image

Take a screenshot of your mod in action, and save it as `preview.png`. Drop the image into your mod's root folder. It should be square and its dimensions should be at least `512x512` pixels.

### Set custom title and description

Create a new `.txt` file, rename it to `mod.json`, and place it in your mod's root folder. Its contents should be set up as follows:

```json
{
    "Title" : "My awesome mod",
    "Description" : "This mod contains some cool stuff!"
}
```

## Publish, update, and unpublish

Just click on your mod in the **Installed** tab, and choose the appropriate action.

![20180514-193710](https://user-images.githubusercontent.com/1748681/78776110-04c57880-79a0-11ea-87cc-67dcc39c14f6.png)

!!! note
    You can publish only mods that are not tracked as **installed**, i.e. was not downloaded from the gallery but manually placed to `Content/` by you.

If you are updating a mod that is already published, users that have it installed will see that an update is available for it.

## Limits

To prevent our servers from being completely filled with content, we're temporarily restricting how many packs users can publish. Your limit can be seen at  [https://voxeltycoon-mods.herokuapp.com/limits?uid=`your_secret_key`](https://voxeltycoon-mods.herokuapp.com/limits?uid=your_secret_key), where "your_secret_key" is the one stored in your specific `identity.json` file.
