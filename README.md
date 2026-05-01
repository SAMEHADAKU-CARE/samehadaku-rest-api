# OFFICIAL SAMEHADAKU API

SRA IS A REST API WHICH IS SCRAPING TO [SAMEHADAKU](https://samehadaku.site) WEBSITE & MADE UP WITH EXPRESS.
[PREVIEW ON HEROKU](https://samehadaku-rest-api.herokuapp.com/)

USE [NPM](https://npmjs.com/) TO INSTALL SRA'S PKG.

* CLONE REPO
* INSTALL ALL PKG WITH COMMAND
```bash
npm install
```
START SERVER COMMAND:
```bash
npm start
```
```bash
npm run nodemon
```
RUN IN [LOCALHOST:3000](http://localhost:3000/)

## ENDPOINT

| Url        | Params           | Type | Description |
| ------------- |:-------------:| :-----:|  :-----|
| /      | - | - | homepage  
| /page/{page}    | page     |  number | homepage-pagination |
| /blog   | -     |  - | blog |
| /blog/{page}   | page     |  number | blog-pagination |
| /blog/read/{id}   | id     |  String | read blog |
| /anime/{id}   | id     |  String | detail anime |
| /anime/eps/{link}   | link     |  String | detail anime's eps |
| /search/{title}/{page}   | title, page     |  String, number | search anime |
| /season | -     |  - |list anime of this season|
| /date-release | -     |  - | anime release date |
| /list-anime/{page} | page     |  number | list of all anime |
| /blog-category/{category}/{page} | category, page     |  String, number | list items of category |
| /tag/{tag} | tag   |  String | list items of tag |
| /daftar-genre | -   |  String | genre list |
| /genre/{id} | id   |  String | show anime by genre |

## SAMPLE RESPONSE

API ENDPOINT : https://samehadaku-rest-api.herokuapp.com/
```json
{
    title: "Re:Zero kara Hajimeru Isekai Seikatsu Season 2",
    status: "Ongoing",
    link: "https://samehadaku.vip/anime/rezero-kara-hajimeru-isekai-seikatsu-season-2/",
    linkId: "rezero-kara-hajimeru-isekai-seikatsu-season-2",
    image: "https://i0.wp.com/samehadaku.vip/wp-content/uploads/2020/07/108005.jpg?quality=90&resize=150,210",
    rating: "8.79",
    sinopsis: "Musim Kedua dari Serial Re:Zero kara Hajimeru Isekai Seikatsu.",
    genre: [
        "Drama",
        "Fantasy",
        "Psychological",
        "Thriller"
    ]
},
```
---
