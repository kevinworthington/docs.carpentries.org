## Collaborative Blog Post Writing

The Carpentries welcomes blog posts from our community members including workshop host sites, instructors, learners, and more. Are you interested in publishing a post on The Carpentries blog?

### Sharing blog post ideas

- Join The Carpentries Slack and share your blog post idea in the #blog-post-ideas channel to start discussion and invite other community members to collaborate with you (<mark>preferred</mark>)

- Email community[at]carpentries[dot]org with your idea and one of the team will facilitate amplification of the idea in the community so others can reach out and collaborate with you (<mark>option</mark>)


### Sharing ready-to-publish drafts

Our blog content is formatted in Markdown, and rendered as html thanks to Jekyll. You can submit your blog post draft in one of three ways
- Email your blog post draft to community[at]carpentries[dot]org, or
submit it through [this form](https://docs.google.com/forms/d/e/1FAIpQLSeiu5NzJsLxYueaQrNn_qKbaa5JR2Sz12CeCRyedKQxwb54Dw/viewform) and one of the team will follow up with you to get it published. (<mark>low time requirement</mark>)

If you wish to submit a blog post about your favourite tool or workflow, you can submit the post through [this form](https://docs.google.com/forms/d/e/1FAIpQLSeiu5NzJsLxYueaQrNn_qKbaa5JR2Sz12CeCRyedKQxwb54Dw/viewform) and we will post it on the blog for you.

- Create a [CodiMD](https://codimd.carpentries.org/) file, convert your post to Markdown [[see Markdown cheatsheet](https://www.markdownguide.org/cheat-sheet/)], add a YAML header to the top of your Markdown file, open an issue in The Carpentries blog GitHub repository with new post appended to the issue title. One of the team will help get it published. (<mark>moderate-time requirement</mark>)

- Convert your post to Markdown [[see Markdown cheatsheet](https://www.markdownguide.org/cheat-sheet/)], add a YAML header to the top of your Markdown file, and submit a Pull Request to The Carpentries blog GitHub repository (<mark>more tasking</mark>).

Read below and find out how to contribute a blog post to

  - [The Carpentries blog](#how-to-contribute-a-blog-post-to-the-carpentries-blog)
  - [Data Carpentry blog](#how-to-contribute-a-blog-post-to-data-carpentry)
  - [Library Carpentry blog](#how-to-contribute-a-blog-post-to-library-carpentry)
  - [Software Carpentry blog](#how-to-contribute-a-blog-post-to-software-carpentry)


#### General recommendations

* For our websites, we use lower kebab case for our file names pages. So
  `example-page.md` is a valid file name but `ExamplePage.md` or `example_page`
  are not.
* Try to avoid using shorthand, acronyms, or contractions in the file names (and
  by extension in the permalinks).
* Favor using the actual numbers in the file names and permakinks instead: use
  `12` rather than `twelve`.
* When relevant, include `carpentries` in the file names and permalinks: favor
  `new-carpentries-team-member` over `new-team-member`.
* Use 3 to 6 words to compose the file names (and permalinks) and the headings
  on your page and blog posts.
* For titles:
  * Please use title case 
  * We recommend making sure the title is descriptive and uses no more than 5-7 words. 
  * When possible, use an action verb or call to action EX:"Amending the Carpentries Bylaws in 2020" or "Expanding The Carpentries Community in California"
* For headers/previews: 
  * We recommend a full sentence that succinctly describes the contents of the blog. EX: "Read on to learn about our strategic plan progress through Q3 2020 (July - September)" or "Join us in welcoming our new Maintainer Community Lead!"
  * Please avoid "in this blog post..."
  * If your title does not have a direct call to action, please include one in the header/preview text


You can include a `time:` entry in the YAML header of the blog posts. The time
is in the 24-hour format and in UTC. It is useful to think of this time as the
earliest the post will appear on the website, but it could end up being
published a few hours later. Our website is being built every 6 hours at 00:30,
06:30, 12:30, 18:30 UTC. So if you include `time: 08:00:00` in the YAML header
of your post, your post will appear after the 12:30 build completes. However, if
there is a manual update to the website at 9:00, your post will appear soon
after completion of the build triggered by this change.


#### How to Contribute a Blog Post to The Carpentries blog

1.  If you wish to contribute a blog post,
    please work in <https://github.com/carpentries/carpentries.org>,
    which can be viewed at <https://carpentries.org/blog/>.

1.  Posts go in the `_posts` folder.

1.  Posts need to be created in [Markdown](https://guides.github.com/features/mastering-markdown/) and named
    according to this convention and case (lower kebab case).

    `YYYY-MM-DD-filename.md`

    e.g.

    `2018-04-29-book-review-teaching.md`

1.  In order to render correctly, posts need to have a header block, which should be created like [this example](https://github.com/carpentries/carpentries.org/blob/gh-pages/_posts/2018/04/2018-04-25-website-launch.md), e.g.

    ```
    ---
    layout: page
    authors: ["Tracy Teal", "Belinda Weaver"]
    teaser: "New website for access to all things Carpentries"
    title: "Launching The Carpentries Website"
    date: 2018-04-25
    time: "09:00:00"
    tags: ["Website", "Communications"]
    ---
    ```

    Separate the header block from the post text by inserting a new line.

1.  All fields should be filled in. If there is more than one author, separate the author names like this: `["Name 1", "Name 2"]`.

1.  Images should be uploaded to the `images` folder. Images should be linked using Markdown, and paths to the image should be relative.

    Example:
    ```md
    ![Image Description]({{ site.filesurl }}/images/myimage.jpg)
    ```
    A web link should be used for images hosted elsewhere. Please be sure you have rights to use this image before including it.

    Example:
    ```md
    ![Image Description](https://web_address/pathway_to_full_image_filename)
    ```

    If you are not sure how to add images in Markdown format, look at an [existing post with a locally hosted image](https://github.com/datacarpentry/datacarpentry.github.io/blob/master/_posts/2017-12-19-frb_carpentry.md) and copy the formatting from there.

1. Once you have previewed your file, commit the Markdown file to your fork and start a Pull Request. We automatically run tests using [TravisCI](https://travis-ci.org/) on your Pull Requests. Please review your pull request a few minutes after you have submitted it to make sure those tests have passed. These tests look for valid YAML headers and make sure that the post will build properly. Once tests have passed, Carpentries Core Team will review and merge your Pull Request or reach out to you with more questions.


#### How to Contribute a Blog Post to Data Carpentry

1.  If you wish to contribute a blog post,
    please work in <https://github.com/datacarpentry/datacarpentry.github.io>,
    which can be viewed at <http://www.datacarpentry.org/blog/>.

1.  Posts go in the `_posts` folder.

1.  Posts need to be created in [Markdown](https://guides.github.com/features/mastering-markdown/) and named
    according to this convention:

    `YYYY-MM-DD-filename.md`

    e.g.

    `2017-07-10-assess_report.md`

1.  In order to render correctly, posts need to have a header block, which should be created like [this example](https://github.com/datacarpentry/datacarpentry.github.io/blob/master/_posts/2015-01-23-genomics-hackathon.md), e.g.

    ```
    ---
    layout: post
    subheadline: "Lessons"
    title: Data Carpentry Genomics and Asssessment Hackathon
    teaser: "Announcing a Data Carpentry Genomics and Assessment Hackathon"
    header:
       image_fullwidth: "light-blue-wood-texture.jpg"
    categories:
       - blog
    comments: true
    show_meta: true
    authors: ["Tracy Teal", "Belinda Weaver"]
    ---
    ```

    Separate the header block from the post text by inserting a new line.

1.  `Subheadline` is an optional field, as is `teaser`, but the other fields should be filled in. If there is more than one author, separate the author names like this: `["Name 1", "Name 2"]`.

1.  Images should be uploaded to the `images` folder. Images should be linked using Markdown, and paths to the image should be relative.

    Example:
    ```md
    ![Image Description]({{ site.filesurl }}/images/myimage.jpg)
    ```
    A web link should be used for images hosted elsewhere. Please be sure you have rights to use this image before including it.

    Example:
    ```md
    ![Image Description](https://web_address/pathway_to_full_image_filename)
    ```

    If you are not sure how to add images in Markdown format, look at an [existing post with a locally hosted image](https://github.com/datacarpentry/datacarpentry.github.io/blob/master/_posts/2017-12-19-frb_carpentry.md) and copy the formatting from there.

1. Once you have previewed your file, commit the Markdown file to your fork and start a Pull Request. We automatically run tests using [TravisCI](https://travis-ci.org/) on your Pull Requests. Please review your pull request a few minutes after you have submitted it to make sure those tests have passed. These tests look for valid YAML headers and make sure that the post will build properly. Once tests have passed, Carpentries Core Team will review and merge your Pull Request or reach out to you with more questions.



#### How to Contribute a Blog Post to Library Carpentry

1.  If you wish to contribute a blog post,
    please work in <https://github.com/LibraryCarpentry/librarycarpentry.github.io>,
    which can be viewed at <https://librarycarpentry.org>.

1.  Posts go in the `_posts` folder.

1.  Posts need to be created in [Markdown](https://guides.github.com/features/mastering-markdown/) and named
    according to this convention:

    `YYYY-MM-DD-filename.md`

    e.g.

    `2018-09-12-data-in-the-desert.md`

1.  In order to render correctly, posts need to have a header block, which should be created like [this example](https://github.com/LibraryCarpentry/librarycarpentry.github.io/blob/master/_posts/2018/09/2018-09-12-data-in-the-desert.md), e.g.

    ```
    ---
    layout: page
    authors: ["Tracy Teal", "Belinda Weaver"]
    title: "Data in the desert"
    teaser: "Library Carpentry workshop at the University of Arizona"
    date: 2018-09-12
    tags: ["University of Arizona", "Library Carpentry", "The Carpentries", "Workshop"]
    category: ["blog"]
    ---
    ```

    Separate the header block from the post text by inserting a new line.

1.  All fields should be filled in. If there is more than one author, separate the author names like this: `["Name 1", "Name 2"]`.

1.  Images should be uploaded to the `images` folder. Images should be linked using Markdown, and paths to the image should be relative.

    Example:
    ```md
    ![Image Description]({{ site.filesurl }}/images/myimage.jpg)
    ```
    A web link should be used for images hosted elsewhere. Please be sure you have rights to use this image before including it.

    Example:
    ```md
    ![Image Description](https://web_address/pathway_to_full_image_filename)
    ```

    If you are not sure how to add images in Markdown format, look at an [existing post with a locally hosted image](https://github.com/LibraryCarpentry/librarycarpentry.github.io/blob/master/_posts/2018/09/2018-09-12-data-in-the-desert.md) and copy the formatting from there.

1. Once you have previewed your file, commit the Markdown file to your fork and start a Pull Request. We automatically run tests using [TravisCI](https://travis-ci.org/) on your Pull Requests. Please review your pull request a few minutes after you have submitted it to make sure those tests have passed. These tests look for valid YAML headers and make sure that the post will build properly. Once tests have passed, Carpentries Core Team will review and merge your Pull Request or reach out to you with more questions.

##### Alternative Ways to Post

If you are new to GitHub and want to submit a blog post without using this workflow, you can submit it through [this form](https://goo.gl/forms/xXDUwhq0rPY0jC5r2) and we will post it to the blog for you.


#### How to Contribute a Blog Post to Software Carpentry

1.  If you wish to contribute a blog post,
    please work in <https://github.com/swcarpentry/website>,
    which can be viewed at <https://software-carpentry.org/blog>.

1.  Posts go in the `_posts` folder, which is divided up first by year,  e.g. `2017`, and then by month, e.g. `07`. Be sure to start creating your file in the correct folder.

1.  Posts need to be created in [Markdown](https://guides.github.com/features/mastering-markdown/) and named according to this convention:

    `YYYY-MM-DD-filename.md`

    e.g.

    `2017-07-10-assess_report.md`

1.  In order to render correctly, posts need to have a header block, which should be created like [this example](https://github.com/swcarpentry/website/blob/gh-pages/_posts/2017/06/2017-06-19-mqu-ttt.md), e.g.

    ```
    ---
    layout: post
    subheadline: "Assessment"
    title: "Analysis of Software Carpentry Workshop Impact"
    date: 2017-07-10
    time: "08:00:00"
    authors: ["Tracy Teal", "Belinda Weaver"]
    category: ["surveys", "workshops", "impact", "assessment"]
    ---
    ```

    Separate the header block from the post proper by a new line.

1.  `Subheadline` is an optional field, as is `time`, but the other fields should be filled in. If there is more than one author, separate the author names like this: `["Name 1", "Name 2"]`. Separate any categories the same way.

1.  Images should be uploaded to the appropriate year in the `files/<year>/<month>` folder. Images should be linked using Markdown, and paths to the image should be relative.

    Example:

    ```md
    ![Image Description]({{ site.filesurl }}/2017/07/myimage.jpg)
    ```

    A web link should be used for images hosted elsewhere. Please be sure you have rights to use this image before including it.

    Example:

    ```md
    ![Image Description](https://web_address/pathway_to_full_image_filename)
    ```

    If you are not sure how to add images in Markdown format, look at an [existing post with a locally hosted image](https://github.com/swcarpentry/website/blob/gh-pages/_posts/2017/06/2017-06-19-mqu-ttt.md) or [one with a web link](https://github.com/swcarpentry/website/blob/gh-pages/_posts/2017/07/2017-07-10-assess_report.md) and copy the formatting from there.

7.  Once you have previewed your file, commit the Markdown file to your fork and start a Pull Request. We automatically run tests using [TravisCI](https://travis-ci.org/) on your Pull Requests. Please review your pull request a few minutes after you have submitted it to make sure those tests have passed. These tests look for valid YAML headers and make sure that the post will build properly.



#### Troubleshooting

The most likely reason posts fail to build is because of 'rogue' characters in the YAML header. Rogue characters generally occur because material has been pasted in directly from programs like Word or Google documents. The most common rogue characters that cause issues are smart quotes (curly quote marks as opposed to plain ones), but others might be em or en dashes, mathematical or other symbols, or other characters that cannot be rendered in plain text by typing on a keyboard. Replace smart quotes with plain quote marks and smart em or en dashes with plain hyphens to avert any problems.
