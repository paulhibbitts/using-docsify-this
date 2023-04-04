# Using Docsify-This for Publishing, Sharing and Reusing Markdown Content

Are you interested in leveraging Markdown for online content without any website setup or build process? How about seamlessly embedding constraint-free Markdown/HTML into other platforms (e.g. CMS or LMS)? The open-source project Docsify-This.net (based on Docsify.js.org) provides an easy way to publishing, sharing and reusing Markdown content.

## Docsify-This

[Docsify-This](https://github.com/hibbitts-design/docsify-this) is an open source Web app, built using the [Docsify Open Publishing Kit](https://github.com/hibbitts-design/docsify-open-publishing-starter-kit), that can quickly display online Markdown files as web pages (i.e. no file uploads or build processes).   

_Being open source, you can even host your own Docsify-This instance! No platform lock-in here._

### Example Docsify-This Usage Scenarios

* Publish your Markdown files as standalone web pages, with no website setup or build process required
* Visually style your standalone web pages using a point-and-click Web Page Builder
* Share existing GitHub-hosted Markdown files as standalone web pages, with an optional 'Edit this Page' link
* Seamlessly embed constraint-free Markdown/HTML, which you have authored, into other platforms (e.g. LMS or CMS)
* Reuse existing Markdown content by seamlessly embedding it within other platforms (e.g. LMS or CMS)
* Utilize the supported URL parameters when embedding content to match each destination platform better visually

### Docsify-This Web Page Builder

To use the Docsify-This **Web Page Builder** enter the URL for an online Markdown file and tap the ‘View as Standalone Web Page’ button. The Markdown file will then  be rendered as a standalone Web page with it’s own URL that can then be copied and shared.

![Docsify-This Web Page Builder](images/docsify-this-web-page-builder.jpg ':class=image-75-border')  
_Figure 1. Docsify-This Web Page Builder_

### Example Docsify-This URL

```html
https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-article/main&homepage=home.md
```

![Docsify-This Rendered Markdown File](images/docsify-this-rendered-markdown-file.jpg ':class=image-75-border')  
_Figure 2. Docsify-This Rendered Markdown File_

Docsify-This rendered Web pages are also perfect for embedding, with the ability to visually style Docsify-This pages to the destination platform.

### Docsify-This URL Editing

You can also render other Markdown files in the same repository by directly editing the Docsify-This URL parameter **homepage**, for example:

```html
https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-article/main&homepage=anotherfile.md
```

### Docsify-This Web Page Appearance

#### URL Parameters

[URL Parameters](https://docsify-this.net/#/?id=page-appearance-url-parameters) (any Markdown file)  
For example, **font-family**, **font-size**, **link-color** and **line-height**   

```
https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-article/main&homepage=home.md&font-family=Open%20Sans,sans-serif
```

#### Markdown CSS Classes

[Markdown CSS Classes](https://docsify-this.net/#/?id=supported-markdown-css-classes)  
For example, **banner-image**, **button**, and **image-75/image-50/image-25**  

```
![UX - User Experience](images/12650723674_d5c85af332_k.jpg ':class=banner-image')
```

```
[Required Reading Quiz due Jun 4th](https://canvas.sfu.ca/courses/44038/quizzes/166553 ':class=button')
``` 

#### Custom Markdown CSS Classes

In addition to the Markdown CSS classes supported by Docsify-This, you can also define your own custom classes within your displayed Markdown files, for example:

CSS in Markdown file:  
```css
<style>
.markdown-section .mybutton, .markdown-section .mybutton:hover {
  cursor: pointer;
  color: #CC0000;
  height: auto;
  display: inline-block;
  border: 2px solid #CC0000;
  border-radius: 4rem;
  margin: 2px 0px 2px 0px;
  padding: 8px 18px 8px 18px;
  line-height: 1.2rem;
  background-color: white;
  font-family: -apple-system, "Segoe UI", "Helvetica Neue", sans-serif;
  font-weight: bold;
  text-decoration: none;
}
</style>
```

Markdown:  
```markdown
[Required Reading Quiz due Jun 4th](https://canvas.sfu.ca/courses/44038/quizzes/166553 ':class=mybutton')
```

#### HTML Snippets

As supported by standard Markdown, HTML snippets can also be included (and mixed) within Markdown , for example:  

```html
<div class="row">
<div class="column">

Lorem ipsum dolor sit amet, consectetur adipiscing elit.

</div>
<div class="column">

Lorem ipsum dolor sit amet, consectetur adipiscing elit.

</div>
</div>
```

### Embedding Docsify-This Pages

#### Example Docsify-This Redirect Tool URL 

![Docsify-This Module](images/docsify-this-page.jpg ':class=image-75-border')  
_Figure 3. Docsify-This External URL (used with the Redirect Tool), for example https://canvas.sfu.ca/courses/76289/external_tools/36154_

```html
url=https://docsify-this.net/?basePath=https://raw.githubusercontent.com/paulhibbitts/cmpt-363-222-pages/main&homepage=resources.md&edit-link=https://github.com/paulhibbitts/cmpt-363-222-pages/blob/main/resources.md&font-family=Lato%20Extended,Lato,Helvetica%20Neue, Helvetica,Arial,sans-serif&font-size=1&hide-credits=true
```

#### Example Docsify-This External URL 

![Docsify-This Module](images/docsify-this-module.jpg ':class=image-75-border')  
_Figure 4. Docsify-This External URL (used as a Canvas LMS Module), for example https://canvas.sfu.ca/courses/76289/modules/items/2816273_

```html
https://docsify-this.net?basePath=https://raw.githubusercontent.com/paulhibbitts/cmpt-363-222-pages/main&homepage=week-01.md&toc-narrow=true&font-family=Lato%20Extended,Lato,Helvetica%20Neue,Helvetica,Arial,sans-serif&font-size=1&hide-credits=true
```

#### Example Docsify-This iFrame HMTL

![Docsify-This iFrame](images/docsify-this-iframe.jpg ':class=image-75-border')  
_Figure 5. Docsify-This iFrame (within the Canvas LMS Homepage), for example https://canvas.sfu.ca/courses/76289_

```html
<p><iframe style="overflow: hidden; border: 0px #ffffff none; margin-top: -26px; background: #ffffff;" src="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/paulhibbitts/cmpt-363-222-pages/main&homepage=home.md&font-family=Lato%20Extended,Lato,Helvetica%20Neue,Helvetica,Arial,sans-serif&font-size=1&hide-credits=true" width="800px" height="950px" allowfullscreen="allowfullscreen"></iframe></p>
```

## Docsify-This + GitHub or Codeberg Markdown Files 

To fully leverage the benefits of version control, and potentially collaboration, store your Docsify-This Markdown pages within a GitHub or Codeberg repository and use an app such as GitHub Desktop to push/pull changes

### Setting up GitHub Desktop

1. Install GitHub Desktop (https://desktop.github.com)
1. Enter your GitHub credentials as prompted
1. Go to a GitHub repository web page, tap **< > Code** and then choose **Open with GitHub Desktop** OR go to a Codeberg repository web page, copy the HTTPS address, then in GitHub Desktop choose **File > Clone Repository** and paste the copied URL
1. Choose the location for your cloned repository and tap the **Clone** button

### Desktop Text Editors

Once your Docsify-This Markdown files are synced (i.e. cloned) to your desktop via GitHub Desktop you can then use the text editor of your choice, such as VSCode, Pulsar Beta (was Atom.io), Typora etc.

Using GitHub Desktop you can preview any changes and then commit those changes back to the repository. VSCode can also be used alone to both sync and editing files.

![Docsify-This + GitHub Markdown Files](images/docsify-this-github.jpg ':class=image-75-border')  
_Figure 10. Docsify-This + GitHub Markdown Files Workflow_

![Docsify-This + Webserver Markdown Files_](images/docsify-this-webserver.jpg ':class=image-75-border')  
_Figure 11. Docsify-This + Webserver Markdown Files_

## An Easy On-Ramp to Markdown Publishing

With Docsify-This the benefits of Markdown-based publishing, and the power of the magical documentation site generator Docsify, are now available to a broader audience - try it out today at [Docsify-This.net](https://docsify-this.net)!