# Mazhuang's Blog

My personal blog: <https://mazhuang.org>, feel free to Star and Fork.

## Overview

<!-- vim-markdown-toc GFM -->

* [Preview](#preview)
* [Fork Guide](#fork-guide)
* [Usage Documentation](#usage-documentation)
* [Experiences and Thoughts](#experiences-and-thoughts)
* [Contact Me](#contact-me)
* [Acknowledgments](#acknowledgments)

<!-- vim-markdown-toc -->

## Preview

**[Online Preview &rarr;](https://mazhuang.org)**

![screenshot home](https://mazhuang.org/assets/images/screenshots/home.png)

## Fork Guide

After forking this project, you need to do a few things to get your page running properly.

1. Correctly set the project name and branch.

   According to GitHub Pages' requirements, projects named `username.github.io` can automatically generate GitHub Pages from the master branch, or from the gh-pages branch for other project names.

2. Modify the domain name.

   If you need to bind your own domain name, change the content of the CNAME file and refer to [Configuring a custom domain for your GitHub Pages site](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site) for configuration; if not, delete the CNAME file.

3. Modify the configuration.

   Most of the website's configuration is in the \_config.yml file. Replace the personal information sections with your own, such as the website's url, title, subtitle, and third-party comment module settings.

   **Comments module:** Currently, it supports disqus, gitment, gitalk, utterances, beaudar, and giscus. Choose one, with giscus recommended. Links to their official configuration guides are in the Comments section of \_config.yml. Please refer to the official guides for configuration.

   **Note:** If using disqus, due to a flaw in disqus' username and domain whitelist strategy, be sure to change disqus.username to your own, or leave it blank. My record of this flaw can be found at [Issues#2][3].

4. Delete my articles and images.

   In the following folders, you can delete everything except the template.md file and add your own content.

   * \_posts folder contains my published blog articles.
   * \_drafts folder contains my unpublished blog articles.
   * \_wiki folder contains my published wiki pages.
   * \_fragments folder contains my published short pieces.
   * images folder contains images used in my articles and pages.

5. Modify the "About" page.

   The content of pages/about.md corresponds to the "About" page of the website. Replace the personal information with your own, including the data in the \_data directory's skills.yml and social.yml files.

   The meanings of the content in skills.yml and social.yml can be referred to here: [Meaning of yml file content in the _data directory](https://mazhuang.org/2020/05/03/blog-template-qna/#_data-%E7%9B%AE%E5%BD%95%E4%B8%8B%E7%9A%84-yml-%E6%96%87%E4%BB%B6%E5%86%85%E5%AE%B9%E5%90%AB%E4%B9%89).

## Usage Documentation

- [Common Questions and Answers for this Blog Template](https://mazhuang.org/2020/05/03/blog-template-qna/).

- To preview the blog locally, refer to [Setting up your Pages site locally with Jekyll][2].

## Experiences and Thoughts

* Follow certain formatting rules, recommended: [Chinese Copywriting Guidelines (Simplified Chinese)][1].

* Simplicity is key; avoid displaying unnecessary content on each page.

* Sometimes a picture is worth a thousand words, but it can also slow down the page load.

* Meaningful content over empty words.

* If writing technical articles, ensure a thorough understanding of the technical principles before writing. Organizing articles while exploring technology is less efficient.

* Avoid long, difficult-to-understand sentences. If they cannot be split into several concise short sentences, it indicates a lack of clear understanding.

* Learn from high-quality bloggers, observing their writing and content organization for valuable insights.

## Contact Me

If you have any suggestions regarding this blog template or its content, you can reach me through [Issues](https://github.com/mzlogin/mzlogin.github.io/issues) or the WeChat public account "Mensa Programmer."

<img width="192px" height="192px" src="https://mazhuang.org/assets/images/qrcode.jpg"/>

## Acknowledgments

The appearance of this blog is modified based on [DONGChuan](https://dongchuan.github.io). Thanks!

[1]: https://github.com/mzlogin/chinese-copywriting-guidelines
[2]: https://help.github.com/articles/setting-up-your-pages-site-locally-with-jekyll/
[3]: https://github.com/mzlogin/mzlogin.github.io/issues/2