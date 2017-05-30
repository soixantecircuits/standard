# Keep Control REST API

Keep Control uses Wordpress REST API coupled with Custom Post Types, so the data on wordpress is easily changed and also accessible for other applications to use.
Since Keep Control is Wordpress based, the base REST API is used. You can find the documentation [here](https://developer.wordpress.org/rest-api/).
As the custom post types are... customized, their json object may vary. But here's a sample of Keep Control's response when sending a request to a custom post type endpoint:

```json
[
  {
    id: 42,
    date: "2017-05-15T18:52:30",
    date_gmt: "2017-05-15T18:52:30",
    guid: {
      rendered: "http://keepcontrol.site/project/?post_type=my-type&#038;p=42"
    },
    modified: "2017-05-16T13:38:29",
    modified_gmt: "2017-05-16T13:38:29",
    slug: "example-post",
    status: "publish",
    type: "my-type",
    link: "https://keepcontrol.site/project/my-type/example-post/",
    title: {
      rendered: "Example Post"
    },
    content: {
      rendered: "<p>This is an example</p>",
      protected: false
    },
    excerpt: {
      rendered: "<p>My excerpt</p> ",
      protected: false
    },
    author: 1,
    featured_media: 0,
    template: "",
    categories: [ 1, 5 ],
    metas: {
      cover-image: {
        image: {
          id: 60,
          title: "Example Image",
          filename: "example.jpg",
          url: "https://keepcontrol.site/content/uploads/example.jpg",
          alt: "",
          author: "1",
          description: "",
          caption: "",
          name: "example",
          date: "2017-05-16 13:24:23",
          modified: "2017-05-16 13:24:23",
          mime_type: "image/jpeg",
          type: "image",
          icon: "https://keepcontrol.site/images/media/default.png",
          width: 334,
          height: 334,
          sizes: {
            thumbnail: "https://keepcontrol.site/5/2017/05/example-150x150.jpg",
            thumbnail-width: 150,
            thumbnail-height: 150,
            medium: "https://keepcontrol.site/5/2017/05/example-300x300.jpg",
            medium-width: 300,
            medium-height: 300,
            medium_large: "https://keepcontrol.site/5/2017/05/example.jpg",
            medium_large-width: 334,
            medium_large-height: 334,
            large: "https://keepcontrol.site/5/2017/05/example.jpg",
            large-width: 334,
            large-height: 334,
            post-thumbnail: "https://keepcontrol.site/5/2017/05/example.jpg",
            post-thumbnail-width: 334,
            post-thumbnail-height: 334
          },
          meta: false
        }
      },
      custom-details: {
        date: "01/05/2017",
        subtitle: "My subtible"
      }
    },
    _links: {
      self: [
        {
          href: "https://keepcontrol.site/project/wp-json/wp/v2/custom/42"
        }
      ],
      collection: [
        {
          href: "https://keepcontrol.site/project/wp-json/wp/v2/custom"
        }
      ],
      about: [
        {
          href: "https://keepcontrol.site/project/wp-json/wp/v2/types/custom"
        }
      ],
      author: [
        {
          embeddable: true,
          href: "https://keepcontrol.site/project/wp-json/wp/v2/users/1"
        }
      ],
      wp:attachment: [
        {
          href: "https://keepcontrol.site/project/wp-json/wp/v2/media?parent=42"
        }
      ],
      wp:term: [
        {
          taxonomy: "category",
          embeddable: true,
          href: "https://keepcontrol.site/project/wp-json/wp/v2/categories?post=42"
        }
      ],
      curies: [
        {
          name: "wp",
          href: "https://api.w.org/{rel}",
          templated: true
        }
      ]
    }
  }
]
```