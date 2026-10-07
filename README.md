# MI 337 Project 1

### Chris Currier

### Snack Bag Generator



##### Goals

1. Create a tool that can be used to generate snack bags of various shapes, sizes, and other adjustable attributes.
2. The tool should have tools relevant to creating game-ready assets, including the ability to generate LODs quickly, scalable UV maps, and more.
3. Include enough documentation and examples for the tool to be usable by anyone with basic Blender knowledge.


### Definitions

<img width="550" height="500" alt="image" src="https://github.com/user-attachments/assets/c251286a-9491-4611-bd47-b478dce92ab7" />

Firstly, we must define the parts of the bag.

The main body of the snack bag is referred to as the Bag section in parameters and throughout documentation.

The 2 end cap sections on the top and bottom of the Bag are called the Ridge section of the snack bag, and have their own set of adjustable parameters.

The two sections are related, but mostly separated, with the ability for each to have their own length and unique materials.

## Workflow

The general workflow will be as follows:
1. Duplicate the Template Collection collection, and adjust parameters/materials of the newly duplicated template snack bag to your liking.
2. Once the snack bag looks as you'd like, duplicate the snack bag and adjust the detail level of each duplicate to generate LODs.
3. Export the collection with all of the LODs enabled and drag the FBX into your game engine.

## LODs

To create LODs, first make sure your bag has the correct parameters that you want to be duplicated across all LODs.

Adjusting parameters becomes tedious after duplication, so it's important to make sure the parameters are set correctly before duplicating.

Next, duplicate the snack bag as many times as you want LODs for, and adjust the detail level of each to reflect the LOD level.

## Parameter Documentation

**Bag X Width:** Multiplier for the X width of the Bag.

**Bag Y Width:** Multiplier for the Y width of the Bag.

**Bag Z Height:** Multiplier for the Z height of the Bag.

**Bag Horizontal Sharpness:** Determines how sharp or round the bag is horizontally. Higher values create sharper corners along the horizontal edges of the bag.

**Bag Vertical Sharpness:** Determines how sharp or round the bag is vertically. Higher values create sharper corners along the vertical edges of the bag.

**Bag Horizontal Loop Detail:** The number of loop cuts running horizontally along the bag.

**Bag Vertical Loop Detail:** The number of loop cuts running vertically along the bag.

**Ridge Height:** Z height off the ridges running along the top and bottom of the bag.

**Bag Top State:** Determines whether top of the bag is Closed (default) or Open.

**Openness Multiplier:** (Only shown if Bag Top State is set to Open) An additional multiplier for how open the bag is. Higher values open the bag further.

**Poly Mode:** Determines whether the bag is low poly or high poly.

**Randomization Seed:** (Shown only if Poly Mode is set to High-Poly) The seed used for randomization during high-poly noise randomization.

**High-Poly Detail Level:** (Shown only if Poly Mode is set to High-Poly) Determines the subdivision detail level of the high-poly.

**Wrinkle Strength Multiplier:** (Shown only if Poly Mode is set to High Poly) Multiplier for how strong the noise-generated wrinkles are throughout both the Bag and Ridge sections.

**Bag Material:** The material that will be applied to the Bag.

**Ridge Material:** The material that will be applied to the Ridge.

## Example Bags (Included In The Blender Project)

### Example Chip Bag at highest LOD level

<img width="417" height="470" alt="image" src="https://github.com/user-attachments/assets/9187cf75-079a-435a-b4ef-47cc5d9fa00f" />

### Example Popcorn Bag at highest LOD level

<img width="412" height="464" alt="image" src="https://github.com/user-attachments/assets/14a32f2c-61a4-4fd0-8034-ad89a0b7f4d7" />

## Hope you have fun generating snack bags!
