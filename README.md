> This is the [Red Devil Hackathon](https://reddevilhacks.github.io/) markdown submission template. Replace *italicized* placeholders with your project details and remove the markdown quotes as well.

> Here are some example submissions from Boosung's previous hackathons: [Frody](https://devpost.com/software/temptemp) and [Albatross](https://devpost.com/software/albatross).

# More YouTube Analytics
### As a YouTube creator, I feel that there are some important metrics missing from the site's built-in analytics. In this project, I used YouTube's API to add a few more charts and graphs to help me better understand my performance.
**Team:** Mandy Grawl

**Submission video:** *Link to video.*
> ⏱️ The video should be 5 minutes or less. In the video, you should include the project inspiration, what it does, and a demo showcasing the key features.

> 🎥 The easiest way to make a video here would be to use OBS or Zoom for screen recording. You can upload the video as an unlisted video on YouTube and add the link here.

## Inspiration
I have recently begun posting regularly on YouTube and trying to figure out what gives my videos the most traction, and so I have been engaging a lot with YouTube's built-in analytics. While the offerings are relatively extensive when you go into the advanced features, there are still some ways it falls short, and some things that I feel could be beneficial additions.
In particular, a metric that is completely left out of YouTube studio is the time of day that the video is posted. For smaller channels, the time of day a video is posted can make or break it: the algorithm seems to decide whether to push a video or not by how it performs in the first few hours, and one does not yet have a loyal following who will go to the channel page to find the video. 
Being a small channel myself, I have been wondering for the past few months if I could code something to grab that information for me and compile it into something easy to read (rather than my current strategy of manually clicking through every video to keep track). Today, I finally decided to learn how to do it.

## What it does
This project is built for a relatively niche audience: small YouTube creators looking for more analytics on their videos. It is a straightforward html document, showing a few extra numbers and graphs to compliment YouTube’s existing ones. For the purposes of this Hackathon demo, I put in my channel’s information as an example case, but it is generalized so that one could put in their own channel’s information and receive the same analysis.

## How we built it
I imported YouTube’s API in order to access creator statistics, went through a few approval processes with my channel itself to allow the information to be exported, and then used R for the data analysis. The coding is 100% done in R.

## Challenges & Accomplishments
This project was more ambitious than I realized, as I had a lot of challenges along the way for something so deceptively straightforward. I have never worked with data taken from a live source before (it has always already been imported to a csv), so it was a huge learning curve figuring out how to import an API and sort through all of the data from that. I also spent a few hours trying to import daily data, but this ultimately did not work as YouTube requires several verifications along the way (so any code dependent on this would not work on any computer besides mine, so it would not be able to be evaluated in this competition), which was a time setback. 
	Generally, this was something above my skill level. I have only completed intro programming classes, so most of this was completely new for me. It also unfortunately took so much time on the backend that it is not very graphically pleasing on the frontend because I simply did not have time to also learn how to make that look more cohesive. 
	In the end, however, I learned how to do all of it and I completed the project. I think that is an accomplishment in and of itself. I have spent months wondering if I could export the data and do something with it, and I finally put in all of the work to do it. I created the graphs that I wanted to display, and I finally have the data I have been wondering about. For a solo project done in one sitting, I think I did a pretty good job.

## What's next?
I would have liked to make the site housing the data more visually appealing, so the first improvements should be made on that front. Beyond that, I would like to try to import the daily data for my own personal analysis, although that is difficult to replicate on other devices because of the amount of logins and confirmation codes. If I could figure out a way around these deterrents, I would love to eventually create a generalized program for anyone to see even more additional YouTube stats, as these are super important metrics for small creators that I think everyone should have access to.

## Try it out
Example data is already hard-coded in, so all of the information is directly on the html document. All graphs can be hovered over and zoomed in.