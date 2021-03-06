# Frontend/Mobile Challenge

## About the Challenge 

We're using GraphQL here, so that's gonna be the way you're going to receive the data (sounds good, right?).

### What you should develop?
It's simple. The user needs to type an address inside a field and be redirected to a products list page. So your job as a front-end engineer will be to create 2 simple screens consuming and sending data to our API.

You can check out an example of this flow at: https://ze.delivery/ (our production env)

We're using GraphQL (give a look to https://www.graphql.com/guides/)

### Visual
We want you to feel free to develop the markup the way you want, we have no wireframes or something like that for this task. You will create 2 screens:
  - Home:
    - Needs to have a header, a footer and a input for the user to fill up with the address.
  - Products page:
    - We want to see the products as cards, with the product title, price and buttons to add/remove the product.

### About the API
The   API   link   is:    https://api.code-challenge.ze.delivery/public/graphql 
  - Home
    - To   find   the   latitude   and   longitude   of   an   address, you can use Google Maps API or use any other Geocoder API that you feel comfortable with.
    - Use   the   following   address   to   find   a   distributor (PoC):    Rua   Américo   Brasiliense,   São   Paulo . 
    - The   Query   needed   to   get   the   right   distributor   (get   the   first   distributor):
        - Query:       https://bit.ly/32Gb2Qi
        - Arguments:
          - Algorithm:   "NEAREST".
          - Lat:   Use   as   String.
          - Long:   Use   as   String.
          - Now:   Pass   the   current   Date   formatted.
  - Product   List
      - The   Query   needed   to   get   the   products
        - Query:    https://bit.ly/2N3JQ7k
        - Arguments:
          - Id:   id   of   the   distributor retrieved from the previous query (PocSearch).
          - Search:   if   ""   (empty),   does   not   filter   by   search.
          - CategoryId:   if   null,   does   not   filter   by   category.
      - The   Query   needed   to   get   the   category   list
        - Query:    https://bit.ly/2pMG8Xy


### Tech Requirements (for both positions):
- You need to create a repo on GitHub to host your code
  - Github users:
      - @ze-engineering-code-challenge
- Avoid using scaffolds (Create React App etc.), we want to see how you make your project structure
- Keep it simple, no need for fancy stuff :)
- TESTS 💛 We really love testing our code and features here!

#### If you are running for a front-end position:
- You're not allowed to use any CSS Frameworks (Bootstrap, Bulma, PureCSS etc.)
- React will be a plus, but you can use whatever you want =)
- I want to be able to run your project locally by using `npm start`

#### If you are running for a mobile position:
- You should use React Native to develop your application.
- I want to be able to run your project with one single command
- Hosting it its a BIG plus (Expo should do the job for ya)


## Evaluation Method

Your code will be under review of the Zé Engineering team. What we will look for:
- **Good Practices and patterns**
- **Code and Folder Structure**
- **Componentization and data flow**
- **Easy to understand code (again, no need for fancy stuff)**
- **Tests**

Feel free to implement it the way you feel more confortable :)

## How to deliver it

Please, use Github to host your code and add @ze-engineering-code-challenge as a collaborator for it. This Github account (@ze-engineering-code-challenge) is solely used by Zé's engineers to download your code and review it

**Once you have finished the challenge, please follow these [instructions](https://github.com/ZXVentures/ze-code-challenges#how-to-deliver).**
