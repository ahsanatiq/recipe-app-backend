# Recipe Service (Backend Task) 

The goal of this task is to assert (to some degree) your coding and architectural skills. You're given a simple problem so you can focus on showcasing development techniques. We encourage you to overengineer the solution a little to show off what you can do - assume you're building a production-ready application that other developers will need to work on and add to over time.

You're **allowed and encouraged** to use third party libraries and **framework or microframework** as long as you know what your using. An effective developer knows what to build and what to reuse, but also how his/her tools work. Be prepared to answer some questions about those libraries, like why you chose them and what other alternatives you're familiar with.

### Technology

- Linux Ubuntu (LTS version) >= 18.04
- PHP >= 7 or NodeJS >= 14 or Python >= 3
- Persist data to MySQL or MongoDB, Redis, Elasticsearch.

## Instructions

- Clone this repository.
- Create a new branch called `dev`.
- Once done, create a pull request from your `dev` branch to the master branch. This PR should contain setup instructions for your application and a breakdown of the technologies & packages you chose to use, why you chose to use them, and the design decisions you made.

## Requirements

We'd like you to build a simple Recipes API. The API **MUST** conform to REST practices and **MUST** provide the following functionality:

- List, create, read, update, and delete Recipes
- Search recipes

### Endpoints

Your application **MUST** conform to the following endpoint structure and return the HTTP status codes appropriate to each operation. Endpoints specified as protected below **SHOULD** require authentication to view. The method of authentication is up to you.

##### Recipes

| Name   | Method      | URL                  | Protected |
| ---    | ---         | ---                  | ---       |
| List   | `GET`       | `/recipes`           | ✘         |
| Create | `POST`      | `/recipes`           | ✓         |
| Get    | `GET`       | `/recipes/{id}`      | ✘         |
| Update | `PUT/PATCH` | `/recipes/{id}`      | ✓         |
| Delete | `DELETE`    | `/recipes/{id}`      | ✓         |

An endpoint for recipe search functionality **MUST** also be implemented. The HTTP method and endpoint for this **MUST** be clearly documented. Recipes **SHOULD** be searched by `name` and `description` from `elsasticsearch` based on a single keyword.


### Schema

- **Recipe**
    - Unique ID
    - Name
    - Description
    - Prep time
    - Difficulty (1-3)
    - Vegetarian (boolean)


### Data Analytics

We would like to see which `search keywords` and `recipes` are used a lot on daily/weekly/monthly basis.


## Criteria

These are some aspects we pay particular attention to:

- Your application **MUST** include a documentation regarding the setup instructions & API usage.
- The API **MUST** return valid JSON and **MUST** follow the endpoints set out above.
- You **MUST** write testable code and demonstrate unit testing it.
- You **SHOULD** pay attention to best security practices.
- You **SHOULD** follow SOLID principles where appropriate.
- **Follow** the industry standard style guide for the language you choose to use - `PSR-2`, `eslint`, etc.
- You do **NOT** have to build a UI for this API.
- A git history (even if brief) with **clear**, **concise** commit messages.

---

Good luck!