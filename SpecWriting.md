#Spec Writing Tips

When writing tickets, I often focus on the following points just to be as descriptive as possible.  STRONG SPECS ARE KING!

* UX / Visual Run Through
* Affected
* Dependencies
* Time Dimension
* Purpose & Stakeholders

##UX / Visual Run Through

Mockups are limited in that they only show a "snapshot" of the feature in time.  It does not show what *will happen* when a particular button is clicked, new data comes in, data is unavailable etc.  Often the terms used are a "concept" but don't repesent the implementation.

**Example 1:** *Infinite Scroll - I could ask for infinite scroll on a feed rather than pagination.  However mock does not specify how many posts are included in the beginning, how many come in per scroll, how many pixels away from the bottom of the screen triggers the next data fetch, as well as what happens if a user runs out of posts.  Changes in *state* need to be run through mentally.*

**Example 2:** *Wizard - How do I progress through the wizard?  What visual indications on the view show how far I have moved?  What do I see when I finish?*

##Affected

If this feature breaks or is not available, what is the expected behavior in other parts of the app?  Think about the pages/screens that are accessed prior to getting to this feature.  Think of both inbound and outbound links if it's a new view.

* How do I get there?
* What happens when I leave?
* What are the adjacent pages?

##Dependencies

What is necessary are needs to be done first before work can even be started on this feature?  

**Example:** *On feed pages, an API is required before UI work can be done. API Structure also needs to be clarified so the UI engineer knows what data to expect.  Will multiple features be dependant on this endpoint in the future?*

##Time Dimension

When will this feature be released?  If so, does it need a progressive release due to the affected above?

**Example:** *If a new uploader creates posts that are structured differently, how will this retroactively affect older posts that still exist?  Is there a new logic that needs to differentiate the two?*

##Purpose & Stakeholders

What is the purpose of this feature and who does it serve?  With this audience, it would help to present them with multiple mocks rather than jumping straight in with a single feature and no feedback prior to the work.



