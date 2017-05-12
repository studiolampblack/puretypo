---
layout: page
title: Contact
navigation: True
logo: 'assets/images/merakipost.svg'
current: contact
cover: 'assets/images/cover1.jpg'
permalink: /contact/
---

Hey there, it's good to see you!

Meraki Post works for the reader community, as journalists to ensure that the world of literature remains a good place to be. We're constantly reading loads (and loads) of books, so we could quench the thirst of the community. At times, we behave like Alan in the _Two and a Half Men_ episode, _That Special Tug_&mdash;of course, sans the emotional breakdown.

Our to-read queues are at least five books long, at any given point in time. So if you request a review for a book (either because you're planning to buy it, or because you wrote it), we might take a while to post it here. If you would rather have us review your book on priority for some reason, we certainly do that, but at a nominal charge.

The charge helps us keep afloat, with respect to the charges we incur to run the site, and all. And after that's covered, we'd definitely love a cup of coffee; who doesn't? Oh, and please understand that in any case, the review would be honest. Be careful before you ask!

If you'd like a review, or have any questions about the world of books, or even need our help with literature (short of writing your English Literature exams for you), please feel free to get in touch! Fill out the form below:

<form id="formaction" method="POST">
  <div><input name="name" placeholder="Your name" type="name" /></div>
  <div><input name="email" placeholder="Your email" type="email" /></div>
  <div><textarea name="message" placeholder="Your message"></textarea></div>
  <input type="hidden" name="_next" value="{{ site.url }}/contact/thanks/" />
  <div><input type="text" name="_gotcha" style="display:none" /></div>
  <div><button type="submit">Send</button></div>
</form>
<script>
    var contactform =  document.getElementById('formaction');
    contactform.setAttribute('action', '//formspree.io/' + 'contact' + '@' + 'merakipost' + '.' + 'com');
</script>

You can find us on [Facebook](https://www.facebook.com/{{ site.facebook }}) or [Twitter](https://twitter.com/{{ site.twitter }}).

Cheers,
Team Meraki Post
