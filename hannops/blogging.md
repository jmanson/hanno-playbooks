# Blogging

_Our strategy and process for creating and managing inbound marketing blogs_

## Blogging strategy

### Choosing what to write about

* Frontend development
* UX design
* Shipbuilding: internal team development, growth and culture
* Remote work

### Finding a spot in the schedule

* We use CoSchedule to stay on top of our content publishing calendar.
* Our blogging days are on __Tuesday__ and __Thursday__. We aim to ship 2 blogs every week.
* If the upcoming schedule is packed out, and you want to ship your blog, you might want to consider shipping it on a Wednesday. But Mondays and Fridays are poor days to publish, so should be avoided if possible.
* Keep ahead of the schedule - if you're booked in, make sure your blog is scheduled and loaded up in WordPress four days before it's due to publish.
* If there is a heavy schedule coming up from one writer (often [Jon]() will monopolise the schedule), feel free to contact them and ask if they can swap with you.

### Setting up a blog in the CoSchedule listing

Head to the [CoSchedule calendar](https://app.coschedule.com/#/calendar/). Look at the upcoming weeks, and find a blank spot.

![blogging1](https://www.datocms-assets.com/1058/1495449265-blogging1.png?w=1000&fit=max)

Click the small pencil icon in the top-right of the calendar cell, and select Blog Post.

![blogging2](https://www.datocms-assets.com/1058/1495449281-blogging2.png?w=1000&fit=max)

Select a blog title (you can change this later), your name, and a category. Try to only publish in a single blog category. __Please make sure the publication time is at 00:00 GMT. This is the easiest solution, given our multiple timezones, and allows us to promote the blog early in the morning in Asia.__

![blogging3](https://www.datocms-assets.com/1058/1495449296-blogging3.png?w=1000&fit=max)

Once you click to confirm, you'll be in the schedule. Now, feel free to head back to Google Docs and write your blog.

### Adding your blogs into WordPress

Most of us write our blogs in Google Docs so that other shipmates can review them before we publish. This is faster than doing things in WordPress, really.

Once you have a solid draft, you're ready to add the standard blog shipping tasklist to the post. Click on the post in the CoSchedule calendar, and in the modal which pops up, select the small icon under the Tasks heading on the right-hand side. Select the __New Blog__ task template, to apply this.

![blogging4](https://www.datocms-assets.com/1058/1495449376-blogging4.png?w=1000&fit=max)

Click to __*Edit Post in WordPress*__ and make sure you're on the VPN. You'll be able to open up the WordPress editor.

And then you should be able to simply copy your blog from Google Docs, into WordPress. Just make sure the _Visual_ editor is selected (check out the top-right of the entry field in this screenshot).

![blogging5](https://www.datocms-assets.com/1058/1495449404-blogging5.png?w=1000&fit=max)

Hint: If you've created and linked a Google document inside of CoSchedule, then you'll be able to convert this document into a Wordpress post right from the app.

![blogging6](https://www.datocms-assets.com/1058/1495449413-blogging6.png?w=1000&fit=max)


This is quite reliable, but there are a few things to watch out for when you copy and paste:

* You'll need to read through the post and make sure it pasted okay. Sometimes there are some little issues.
* It can struggle with bullet points. Especially if they have bold text in them. Pay attention to those, in particular.
* It won't copy images across. You'll need to upload those manually and drop them into the post.
* Watch out for links and bold or italic text in the body of articles: sometimes, the spaces between these text strings, and the text which follows, will be mushed together.

Once you're done with all your edits and have previewed the post on the blog to make sure it looks okay, you're ready to hit the Schedule button inside WordPress or CoSchedule.

### Adding an excerpt to the post

This is important, because we need a little summary to show up when we display this blog on the site. To do it, you'll first need to enable the excerpt field:

First, select __Screen Options__ on the top-right of the blog editing page:

![blogging7](https://www.datocms-assets.com/1058/1495449459-blogging7.png?w=1000&fit=max)

Then, look for the checkbox alongside __Excerpt__. Click it:

![blogging8](https://www.datocms-assets.com/1058/1495449471-blogging8.png?w=1000&fit=max)

And now, an excerpt field should appear further down the page, where you can enter your post summary. It'll stick around, now:

![blogging9](https://www.datocms-assets.com/1058/1495449487-blogging9.png?w=1000&fit=max)

### Sourcing and adding images for blogs

We have a library of images in WordPress. If maintained properly, this will really help other people out. But it relies upon you correctly naming and tagging your images.

#### Good image sources

* Existing images! Before you use an image, particularly if it's an internal Hanno one, please go ahead and search in the WordPress media library, to see if it's there already. If it's from a team trip, or you're just looking for a photo of shipmate(s), there's a good chance you'll find something useful.
* [Unsplash](https://unsplash.com/) and [Pexels](https://www.pexels.com/) are great, of course. There's also a very handy [Unsplash search tool](http://www.arthurweill.fr/Unsplash/en). If you use images from these sites, you don't strictly need to attribute it.
* [Flickr Creative Commons search](https://www.flickr.com/search/?sort=relevance&license=4%2C5%2C6%2C9%2C10&text=personal%20goal&advanced=1) is great for specific images. It's easiest if you just bookmark this link, so you can open it up quickly. If you use one of these images, you'll need to attribute it.

#### How to add the image to the post

Let's assume we've found a [great image on Flickr](https://www.flickr.com/photos/21218849@N03/5016229588/) for our post, and we've downloaded it. It's best to pick the image size which is 1000px or bigger because WordPress will take care of scaling it down for us. We'll need to keep a copy of the original location, to use shortly.

![blogging10](https://www.datocms-assets.com/1058/1495449524-blogging10.jpg?w=1000&fit=max)

We head to our post and click the __Add Media__ button:

![blogging11](https://www.datocms-assets.com/1058/1495449537-blogging11.png?w=1000&fit=max)

Then, we upload the JPG or PNG file.

![blogging12](https://www.datocms-assets.com/1058/1495449550-blogging13.png?w=1000&fit=max)

It'll upload to the site, and be copied over to Amazon S3, which is where we store all of our images. But if you look to the right-hand side of the modal, you'll see that all the image data is empty. We need to do something about this:

![blogging14](https://www.datocms-assets.com/1058/1495449569-blogging14.png?w=1000&fit=max)

There are 3 things we need to fill in:

* __Title__. This should just have a simple, clear title to tell us what the picture is
* __Caption__ (optional). This gets shown on the main site when we add the image. If you're using a copyrighted image, you should add the credit here. It supports HTML, so for the photo we've just used, we might say:

```
Photo by <a href="https://www.flickr.com/photos/21218849@N03/5016229588/">Samuel Mann</a>
```

* __Alt text__. Describe what's in the picture. This is for accessibility reasons, to help visually impaired readers browse our site. Please don't skip it. For this example, we might use:
```
A man sits at a desk with a laptop, talking to a user in a relaxed manner.
```
* __Description__. This is just for our own benefit, but we're able to search it! So again, it helps to be descriptive. It's also recommended that you add the photo credit to this field, too. Let's opt for
```
Interviewing users, conversation. Photo by <a href="https://www.flickr.com/photos/21218849@N03/5016229588/">Samuel Mann</a>
```

Once you're done, you can click the __Insert__ button, and the image will be added to your post. You'll be able to see your caption, too.

![blogging15](https://www.datocms-assets.com/1058/1495449591-blogging15.png?w=1000&fit=max)

### Blogging tips

CoSchedule provides a very good collection of videos (7 in total) with plenty of tips on blogging strategies, best practices and how to use CoSchedule most efficiently. When logged in, you can access the Master Class via [this link](https://app.coschedule.com/#/course/1) or go to CoSchedule directly and click on the "Master Course" icon in the left sidebar.

If you don't have time to watch the videos, here is a summary of the most important hints on how to create consistent content:

1. Plan out editorial content in advance
2. Set aside time to brainstorm new ideas
3. Stick to your deadline
4. Think strategically on your editorial calendar
