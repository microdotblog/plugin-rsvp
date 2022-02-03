# RSVP shortcode

Adds a Hugo shortcode to sending an IndieWeb RSVP.

To RSVP to an event, find the URL for the event and then use the shortcode in a blog post like this:

```
I'm going to this! {{< rsvp href="https://events.indieweb.org/2022/03/micro-camp-2022-IW2Qp3ygHike" >}}
```

It will create a link to the event with the appropriate Microformats reply markup. Micro.blog will notice the post and send a Webmention for it.

To keep the parameters simple, Micro.blog links the event URL with the emoji 📅. To change this, add a `text` parameter:

```
I'm going to this! {{< rsvp href="https://events.indieweb.org/2022/03/micro-camp-2022-IW2Qp3ygHike" text="Micro Camp 2022" >}}
```
