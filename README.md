# LayerCake
LayerCake is a PyQt tool for procedural image generation based on randomized PNG layers.
  
  
There are two phases to creating any great procedural image collection: Construction and Curation.
  
LayerCake's Construction workflow is as follows:
  
  
## Layer Construction Tab
![image](https://user-images.githubusercontent.com/96316841/167516555-da040e64-674a-4d9c-b732-c47be5e224e2.png)
Start with the Layer Construction Tab to determine the arrangement of PNG layers in your composite.
Here you can specify things like composite order, asset tinting, trait rarity, and more.
### Key Features include:
- Drag and drop Layer Order
- Live preview of composited images based on user selection or a simple Shuffle function
- Selection weights to influence rarity of Traits in the final collection
- Various Merge operations per-layer such as Over, Multiply, Screen, etc...
- Dynamic tinting of image assets using pre-selected user generated Palettes
- ..and plenty of convenience features such as a fully functional clipboard and autosave!
  
  
## Palette Construction Tab
![image](https://user-images.githubusercontent.com/96316841/167517016-5494eda6-ff64-4c10-b90b-d5bccf56d532.png)
Palettes are a way to group user-selected colors for dynamic tinting. Why should you need to export the same t-shirt layer a dozen times with a dozen different colors? Instead, you may use a single white t-shirt which is tinted in accordance with a specific palette. This is a huge time saver, especially for assets under heavy iteration.
### Key features include:
- Paste hex codes directly from the clipboard. No need to format them, as they are parsed with regular expressions! You could even paste the source code of an entire webpage, and the palette will be extracted.
- Assign shared palettes across multiple PNG assets; those colors will be maintained across each Shuffle
- Give nicknames to frequently used colors to help with legibility or branding
  
  
## Rules and Restrictions Tab
![image](https://user-images.githubusercontent.com/96316841/167517578-0179a5e7-b100-4e98-992b-de067fbe6a7e.png)
Rules can be used to specify how Layers and Palettes interact with each other. Users can assert Rules such as, "Do not allow pink haired avatars to wear leather jackets", or "If the midnight environment is used, turn off the sunglasses layer".
### Key features include:
- Users can name their own rules and use our 'human readble format' to define them, rather than a complex permissions matrix
- If a user specifies a combination in the Construction Tab which breaks a Rule, they will be alerted with a UI element.

  

Once a user has exported a Collection from LayerCake's Construction workflow, they can import that same Collection for analysis using our Curation workflow!

  
    
      

## Collection Curation Workflow
![image](https://user-images.githubusercontent.com/96316841/167518155-1c2cf78f-df89-40de-a873-100155a4e1c2.png)
Users can quickly and easily search through the images they've generated via per-trait filters, or filter for combinations of traits. They can examine percentage-based representations of each Trait and dynamically assigned Color to ensure the Collection is representative of the desired diversity.
(This feature suite is still a WIP)
  
  
## Collection Metadata Design
Should the user want to generate per-image metadata for the Collection, they will have the ability to do so using our Metadata Designer tool. This set of features will allow users to choose how each PNG layer or Palette Color is described, independent of filenames or pre-assigned Color names, so that their Collection may be branded to taste. Users will also be empowered to omit Layers from the metadata altogether, should they choose to do so.
(This feature suite is still a WIP)
  
  
# Where is the Source Code?
As a studio, we decided that rather than use existing, blackbox, third-party solutions at cost, we'd like to make our own tool in service of our first NFT PFP drop, and then liberate that tool unto our beloved Web3 community! As such, we'll be iterating on LayerCake and perfecting its execution along with the development of our first Collection.
  
TLDR: We will take a moment to clean up, comment, and push v1 of this tool in Q2 2022 :)
