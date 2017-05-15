# Microblog

This is an incomplete implementation of a Twitter-like single-user microblog timeline. 

Please implement the spec (design and product) using these instructions. 

## Resources

* [Zeplin spec](https://zpl.io/Tycej) - use this as the design reference; request an invite first
* [Roboto font](https://fonts.google.com/specimen/Roboto)
* [Material Icons](http://google.github.io/material-design-icons/)
* [Better logo](better-icon.svg)

## Technical requirements

* The stub data (i.e. the posts and users) in `index.html` should not be modified. Everything else can be changed as necessary.
* There is no need for persistence (database or otherwise) - feel free to only use the client-side data.
* Feel free to use any libraries you like (or no libraries at all).
* Please keep the original Git commit as is.

## Spec

* Create a single-user timeline of posts.
* The timeline must support new posts by the current user.
* New posts must appear before older posts.
* Every post must have the following elements:
  * User identifiers: name, real name, photo, and verified status
  * Text of the post
  * A relative timestamp of the time the post was published; this should be updated in real time
  * Zero or more photo attachments that are automatically generated if an image link is detected in the post text
    * There is no need to design any upload or cropping functionality - if an image link exists in text, it should be converted to an attachment and the image should be loaded and "cropped" via CSS as best as possible
* New post length must be limited and must not be zero; the character counter must be functional (check Zeplin spec for more details).
* Posts must support the following interactions:
  * Reply: this creates a new post in reply to the original post; replies are visually distinct in the timeline
  * Repost: this would show the original post in the reposting user's timeline; in this project, it's only used to count reposts
  * Like: this would save the original post in the reposting user's liked posts lists; in this project, it's only used to count likes
* The interface should be responsive; it should scale with the viewport size.

## How to submit your work

* Fork this repo
* Push your changes
* Open a pull request

Please contact us if you have any questions.
