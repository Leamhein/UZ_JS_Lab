# RS Lang Backend

| Start        | Deadline         |
| ------------ | ---------------- |
| 23.06.2021   | 13.07.2021 23:59 |

## Details
1. Backend should realize such API [RS Lang Backend API Doc](https://react-learnwords-example.herokuapp.com/doc/#):
   - Words endpoints:
     - ```GET /words``` - get a chung of words
     - ```GET /words/{id}``` - get a words with assets by id
   ------------------------------------------------------
   - Users endpoints:
     - ```POST /users``` - create new user
     - ```GET /users/{id}``` - get user by id
     - ```PUT /users/{id}``` - update user
     - ```DELETE /users/{id}``` - delete user
     - ```GET /users/{id}/tokens``` - get new user token
   ------------------------------------------------------
   - User words endpoints:
     - ```GET /users/{id}/words``` - Get all users words
     - ```POST /users/{id}/words/{wordId}``` - Create a user word
     - ```GET /users/{id}/words/{wordsId}``` - Get a user word by Id
     - ```PUT /users/{id}/words/{wordId}``` - Update a user word
     - ```DELETE /users/{id}/words/{wordId}``` - Delete user word
   ------------------------------------------------------
   <s>- User aggregated words endpoints:
     - ```GET /users/{id}/aggregatedWords``` - Get all user aggregated words
     - ```GET /users/{id}/aggregatedWords/{wordId}``` - Get a user aggregated word by word id</s>
   ------------------------------------------------------
   - User statistics endpoints:
     - ```GET /users/{id}/statistics``` - Get user statistics
     - ```PUT /users/{id}/statistics``` - Upset statistics
   ------------------------------------------------------
   - User settings endpoints:
     - ```GET /users/{id}/settings``` - Get user settings
     - ```PUT /users/{id}/settings``` - Upset settings
   ------------------------------------------------------
   - Sign In endpoint:
     - ```POST /signin``` - Sign in

2. The JWT token received upon successful login must be used with each request to endpoints requiring authorization. 
   - This token get by POST request to `/signin` endpoint.
   - Tokens have a limited lifetime (4 hours for example).
3. The system supports the differentiation of data by users. To do this, you need to use the POST endpoint at `/users`. In the request, you need to pass a JSON object that contains the user's email address and password. The password must be at least 8 characters long.

## Technical Requirement
1. Express allowed to use

## Criteria for evaluation
**Max points: 550 **

1. ```POST /signin```, ```GET /words```, ```POST /users```, ```GET /users/{id}``` endpoint is must have.
2. For each correctly working endpoint, 30 points are awarded.
3. Using typescript - 40 points.

## Wiki
 - [Creating mongodb in Mongo Atlas](https://github.com/rolling-scopes-school/react-rslang-be/wiki/%D0%A1%D0%BE%D0%B7%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-%D0%B1%D0%B0%D0%B7%D1%8B-mongodb-%D0%B2-Mongo-Atlas)
 - [Loading word data into Mongo Atlas](https://github.com/rolling-scopes-school/react-rslang-be/wiki/%D0%97%D0%B0%D0%B3%D1%80%D1%83%D0%B7%D0%BA%D0%B0-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85-%D0%BE-%D1%81%D0%BB%D0%BE%D0%B2%D0%B0%D1%85-%D0%B2-Mongo-Atlas)
 - [Deploy application to Heroku](https://github.com/rolling-scopes-school/react-rslang-be/wiki/%D0%94%D0%B5%D0%BF%D0%BB%D0%BE%D0%B9-%D0%BF%D1%80%D0%B8%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D1%8F-%D0%BD%D0%B0-Heroku)
 - [Examples of request](https://github.com/rolling-scopes-school/react-rslang-be/wiki/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B-%D0%B7%D0%B0%D0%BF%D1%80%D0%BE%D1%81%D0%BE%D0%B2-%D0%BA-API)

## Useful links
 - [NodeJS Introduction (RU)](https://www.youtube.com/watch?v=Bs3MUHB_o8U&list=PLzLiprpVuH8eLZd665rBTYaLRw7TONz7E&index=1)
 - [NodeJS Modules (RU)](https://www.youtube.com/watch?v=RXFOAqsWzFA&list=PLzLiprpVuH8eLZd665rBTYaLRw7TONz7E&index=2)
 - [TypeScript in NodeJS part 1 (RU)](https://www.youtube.com/watch?v=I_aTbZcH8Do&list=PLzLiprpVuH8eLZd665rBTYaLRw7TONz7E&index=9)
 - [TypeScript in NodeJS part 2 (RU)](https://www.youtube.com/watch?v=CegrbRXGw20&list=PLzLiprpVuH8eLZd665rBTYaLRw7TONz7E&index=10)
 - [MongoDB, mongoose (RU)](https://www.youtube.com/watch?v=Iyuf0GBgETs)
 - [Authentication. Security + CORS (RU)](https://www.youtube.com/watch?v=K0K4bCQAfUM)
 - [NodeJS debugging in VS Code (EN)](https://www.youtube.com/watch?v=2oFKNL7vYV8)
 - [NodeJS debugging in WebStorm (RU)](https://www.youtube.com/watch?v=5-YfjWaLj2w&t=301s)
 - [Complex guide for NodeJS, Express and MongoDB (RU)](https://metanit.com/web/nodejs/)
