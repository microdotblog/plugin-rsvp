# RSVP shortcode

Adds a Hugo shortcode for sending an IndieWeb RSVP.

To RSVP to an event, find the URL for the event and then use the shortcode in a blog post like this:

```
I'm going to this! {{< rsvp href="https://events.indieweb.org/2022/03/micro-camp-2022-IW2Qp3ygHike" >}}
```

It will create a link to the event with the appropriate Microformats reply markup. Micro.blog will notice the post and send a Webmention for it.

To keep it simple, Micro.blog links the event URL with the calendar emoji, so the above post will look like this:

```
I'm going to this! 📅
```

You use your own text instead of the emoji with a `text` parameter:

```
{{< rsvp href="https://events.indieweb.org/2022/03/micro-camp-2022-IW2Qp3ygHike" text="Micro Camp 2022" >}}
```
