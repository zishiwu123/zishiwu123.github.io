---
layout: post
title: "CardExplorer Part 1"
date: 2024-10-01 05:00:00 -0000
categories: lorcana
---

This is the first article in my series to create a website to search for [Disney Lorcana][disney-lorcana] cards.
I have built a simple backend API that reads all the cards up to Lorcana Set 5 from a CSV file and provides
API routes to search for cards by id, name, set number, card number, ink color, and rarity. For now, there
is no fancy frontend and no database as I am focused on just backend web development. After I refresh my skills
on this, I will move on to the other parts: frontend, database, CI/CD pipelines.

I have written the backend API using two different frameworks, see https://github.com/zishiwu123/cardexplorer
1. [FastAPI][fastapi] in Python, see https://github.com/zishiwu123/cardexplorer
2. [NodeJS][nodejs] and [ExpressJS][expressjs] in TypeScript, see https://github.com/zishiwu123/cardexplorer-ts

For cardexplorer repo using FastApi, it runs on localhost:8000

![CardExplorer API using FastAPI](/assets/images/lorcana/fastapi_no_query.png){: width="250"}

For cardexplorer-ts repo using Node.js and ExpressJS, it runs on localhost:3000. I used [Zod][zod]
to help generate schemas and OpenAPI documentation. I borrowed a template for creating a 2024
Node.js and ExpressJS project by using https://github.com/edwinhern/express-typescript-2024 as a template. 

![CardExplorer API using Node.js and Express](/assets/images/lorcana/nodejs_openapi_doc.png){: width="250"}

We can search by a specific card id:

![Search by card id](/assets/images/lorcana/nodejs_search_by_card_id.png){: width="250"}

We can search by name, set number, card number, ink color, and/or rarity:

![nodejs_demo_search_query_params](/assets/images/lorcana/nodejs_demo_search_query_params.png){: width="250"}


[fastapi]: https://github.com/fastapi/fastapi
[nodejs]: https://nodejs.org/
[expressjs]: https://expressjs.com/
[zod]: https://zod.dev/