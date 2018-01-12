## 설정 관련 문서

아래의 문서에서  사이트 설정이 가능하다.`_config.yml`

```
# Site Settings
title: Jamy | Designer
email: youremail@gmail.com
description: Some text about your blog.
baseurl: "" # the subpath of your site, e.g. /blog/ or empty.
url: "https://www.rossener.com" # the base hostname & protocol for your site
google_analytics: "UA-XXXXXXXX-X"

# User settings
username: Thiago Rossener # it will appear on each page title after '|'
user_description: Some text about you.
disqus_username: disqus_username

# Social Media settings
# Remove the item if you don't need it
github_username: github_username
facebook_username: facebook_username
twitter_username: twitter_username
instagram_username: instagram_username
linkedin_username: linkedin_username
medium_username: medium_username
```

## 색상 설정 관련 

All color variables are in [src/styl/_variables.styl](src/styl/_variables.styl).

Default colors:

![#ff0a16](https://placehold.it/15/ff0a16/000000?text=+) `#FF0A16` Theme Color

![#141414](https://placehold.it/15/141414/000000?text=+) `#141414` Primary Dark

![#ffffff](https://placehold.it/15/ffffff/000000?text=+) `#FFFFFF` Accent Dark

![#f2f2f2](https://placehold.it/15/f2f2f2/000000?text=+) `#F2F2F2` Light Gray

![#333333](https://placehold.it/15/333333/000000?text=+) `#333333` Texts

## Creating drafts

You can use the `initdraft.sh` to create your new drafts. Just follow the command:

```
./initdraft.sh -c Post Title
```

The new file will be created at `_drafts` with this format `date-title.md`.

## 포스트 작성 관련 

You can use the `initpost.sh` to create your new posts. Just follow the command:

```
./initpost.sh -c Post Title
```

The new file will be created at `_posts` with this format `date-title.md`.

## Front-matter 

When you create a new post, you need to fill the post information in the front-matter, follow this example:

```
---
layout: post
title: "Welcome"
description: Lorem ipsum dolor sit amet, consectetur adipisicing elit.
image: 'http://res.cloudinary.com/dm7h7e8xj/image/upload/c_scale,w_760/v1504807239/morpheus_xdzgg1.jpg'
category: 'blog'
tags:
- blog
- jekyll
twitter_text: Lorem ipsum dolor sit amet, consectetur adipisicing elit.
introduction: Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
---
```

**Your image size should have the proportion of a 600x315 image to look good on home page.**

## Run locally

In order to compile the assets and run Jekyll on local you need to follow those steps:

- Install [NodeJS](https://nodejs.org/) (remember to use the latest version)
- Run `sudo npm install`
- Run `sudo npm install -g gulp gulp-cli`
- Run `sudo gulp`

## 마크 다운 관련 
**[Markdown](http://whatismarkdown.com/)**은 텍스트 기반의 마크업언어로 2004년 존그루버에 의해 만들어졌으며 쉽게 쓰고 읽을 수 있으며 HTML로 변환이 가능하다. 특수기호와 문자를 이용한 매우 간단한 구조의 문법을 사용하여 웹에서도 보다 빠르게 컨텐츠를 작성하고 보다 직관적으로 인식할 수 있다.
마크다운이 최근 각광받기 시작한 이유는 깃헙([https://github.com](https://github.com)) 덕분이다. 깃헙의 저장소Repository에 관한 정보를 기록하는 README.md는 깃헙을 사용하는 사람이라면 누구나 가장 먼저 접하게 되는 마크다운 문서였다. 마크다운을 통해서 설치방법, 소스코드 설명, 이슈 등을 간단하게 기록하고 가독성을 높일 수 있다는 강점이 부각되면서 점점 여러 곳으로 퍼져가게 된다.

## 마크 다운 사용법 
해당 공간은 문장을 적는공간입니다. 😆

> 인용구 적을 일 있으면 사용하세요. 🤗

강조 구문  있을시 **강조 구문** 사용하세요 

## 제목 관련 

HTML defines a long list of available inline tags, a complete list of which can be found on the [Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Web/HTML/Element).

- **To bold text**, use `<strong>`.
- *To italicize text*, use `<em>`.
- Abbreviations, like <abbr title="HyperText Markup Langage">HTML</abbr> should use `<abbr>`, with an optional `title` attribute for the full phrase.
- Citations, like <cite>&mdash; Thiago Rossener</cite>, should use `<cite>`.
- <del>Deleted</del> text should use `<del>` and <ins>inserted</ins> text should use `<ins>`.
- Superscript <sup>text</sup> uses `<sup>` and subscript <sub>text</sub> uses `<sub>`.

Most of these elements are styled by browsers with few modifications on our part.

# Heading 1

## Heading 2

### Heading 3

#### Heading 4

우용하게 사용합니다.

## Code

코드 관련  내용`code element` 아래와 같이 사용합니다.

```js
// Example can be run directly in your JavaScript console

// Create a function that takes two arguments and returns the sum of those arguments
var adder = new Function("a", "b", "return a + b");

// Call the function
adder(2, 6);
// > 8
```

위와 같이 나옵니다.

## Lists

리스트 표기시는 아래와 같은 방법으로 활용합니다.

* Praesent commodo cursus magna, vel scelerisque nisl consectetur et.
* Donec id elit non mi porta gravida at eget metus.
* Nulla vitae elit libero, a pharetra augue.

Donec ullamcorper nulla non metus auctor fringilla. Nulla vitae elit libero, a pharetra augue.

1. Vestibulum id ligula porta felis euismod semper.
2. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
3. Maecenas sed diam eget risus varius blandit sit amet non magna.

Cras mattis consectetur purus sit amet fermentum. Sed posuere consectetur est at lobortis.

## Images
이미지 테스트 구관입니다.

![placeholder](https://placehold.it/800x400 "Large example image")
![placeholder](https://placehold.it/400x200 "Medium example image")
![placeholder](https://placehold.it/200x200 "Small example image")

## Tables

표 사용 방법 입니다.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Upvotes</th>
      <th>Downvotes</th>
    </tr>
  </thead>
  <tfoot>
    <tr>
      <td>Totals</td>
      <td>21</td>
      <td>23</td>
    </tr>
  </tfoot>
  <tbody>
    <tr>
      <td>Alice</td>
      <td>10</td>
      <td>11</td>
    </tr>
    <tr>
      <td>Bob</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <td>Charlie</td>
      <td>7</td>
      <td>9</td>
    </tr>
  </tbody>
</table>
-----
