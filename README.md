# Website Code Refactor Demonstration

This project is a demonstration of refactoring an existing website. The client, a marketing company, requested that their website have several improvements made to improve accessibility features, SEO performance, and code readability. This was accomplished primarily by replacing generic div tags with semantic HTML. 

## Goals and Methods 

The primary objective of this effort was to augment the site's accessibility which will allow people with disabilities to access the site and improve SEO performance. The secondary objective was to reorganize the codebase to improve readability and ease future development. This was achieved in the following steps:

* Adapting non-descriptive div elements into semantic HTML elements (e.g. Snippet 1 and 2);
* Consolidating pre-existing CSS code into robust general purpose classes (Snippet 1 and 2);
* Restructuring CSS code to follow site layout (Snippet 3 and 4); and
* Creating alt text for all site images.

(Snippet 1) Below is a representative snippet of the original codebase making use of div elements:
```HTML
    <div class="header">
        <h1>Hori<span class="seo">seo</span>n</h1>
        <div>
            <ul>
                <li>
                    <a href="#search-engine-optimization">Search Engine Optimization</a>
                </li>
                <li>
                    <a href="#online-reputation-management">Online Reputation Management</a>
                </li>
                <li>
                    <a href="#social-media-marketing">Social Media Marketing</a>
                </li>
            </ul>
        </div>
    </div>
```
(Snippet 2) Semantic HTML was implemented to improve readability, accessibility, and functionality:
```HTML
    <header>
        <h1>Hori<span>seo</span>n</h1>        
        <nav>
            <a href="#search-engine-optimization">Search Engine Optimization</a>
            <a href="#online-reputation-management">Online Reputation Management</a>
            <a href="#social-media-marketing">Social Media Marketing</a>
        </nav>
    </header>
```
Snippet 1 also serves to show how CSS hooks were written for the site. Such hooks were not necessary after the restructuring the site using semantic HTML as shown in Snippet 2.

(Snippet 3) The following snippet of original code illustrates how classes were used to style the site:
```CSS
.search-engine-optimization h2 {
    margin-bottom: 20px;
    font-size: 36px;
}

.online-reputation-management h2 {
    margin-bottom: 20px;
    font-size: 36px;
}

.social-media-marketing h2 {
    margin-bottom: 20px;
    font-size: 36px;
}
```
(Snippet 4) Such class calls are verbose and were condensed:
```CSS
h2 {
    margin-bottom: 20px;
    font-size: 36px; 
}
```
---

## Prerequisites

Other than a web brower no software installation is needed.

---

## Built With

* [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
* [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
* [Git](https://git-scm.com/)
* [GitHub](https://github.com/)

## Deployed Link



---



 
