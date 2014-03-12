# Technical Lead (Restaurant Apps) - Technical Test

Thank you for taking the time to do our technical test. It should take between 105 and 165 minutes to complete - depending on whether you attempt the optional (but highly valued) Functional Testing exercise - and consists of three parts:

* Coding- please don’t spend more than 60 minutes on this part

* Functional testing [OPTIONAL] - please don’t spend more than 60 minutes on this part

* Technical questions - please don’t spend more than 45 minutes on this part

In order to avoid bounced emails (some ISP's appear to be blocking emails with candidates' test result attachments) we would like you to submit your results by uploading the relevant zip file to a shared Google Drive folder. In order to supply you with the URL for this folder please send an email to tech.recruitment@just-eat.com stating your Google email address. (Alternatively, you can let your agent know your Google address.) If you don't already have a Google email address, please obtain one so that you can be given access to the JUST EAT test results folder. 

Please make this a single zip file named {yourname}-{role-you-apply-for}.zip containing 1 markdown file with the answers to the technical questions and 1 folder containing the technical test.

## Coding - 60 minutes

JUST EAT has a public API available at [http://api-interview.just-eat.com/](http://api-interview.just-eat.com/) that you can use to get restaurant information, including which restaurants deliver to what areas.

### How to use the API

##### With the following headers:

`Accept-Tenant: uk`

`Accept-Language: en-GB`

`Accept-Charset: utf-8`

`Authorization: Basic VGVjaFRlc3RBUEk6dXNlcjI=`

`Host: api.just-eat.com`

* [http://api-interview.just-eat.com/](http://www.google.com/url?q=http%3A%2F%2Fapi.just-eat.com%2Frestaurants%3Fq%3Dse19&sa=D&sntz=1&usg=AFQjCNGDTQ2r7AuFD45sUZl1a6dDucGMUg)[restaurants?q=se19](http://api.just-eat.com/restaurants?q=se19) returns a list of restaurants that deliver to an outcode, including some basic restaurant information (for outcode = se19)

* [http://api-interview.just-eat.com/](http://www.google.com/url?q=http%3A%2F%2Fapi.just-eat.com%2Frestaurants%2F17266%2Fmenus&sa=D&sntz=1&usg=AFQjCNFKO4jULs6DZVhMg3xuCF4b9DIXwA)[restaurants/17266/menus](http://api.just-eat.com/restaurants/17266/menus) returns a list of menues for a restaurant (for restaurantid = 17266)

* [http://api-interview.just-eat.com/](http://www.google.com/url?q=http%3A%2F%2Fapi.just-eat.com%2Fmenus%2F57443%2Fproductcategories&sa=D&sntz=1&usg=AFQjCNE7c-6fiQ9T8BT2xPHwkcIdaLaR4w)[menus/57443/productcategories](http://api.just-eat.com/menus/57443/productcategories) returns a list of categories for a menu (for menuid = 57433)

* [http://api-interview.just-eat.com/](http://www.google.com/url?q=http%3A%2F%2Fapi.just-eat.com%2Fmenus%2F57443%2Fproductcategories%2F5%2Fproducts&sa=D&sntz=1&usg=AFQjCNF5bQudY1V7FRgRVn41PVWdcxSWZA)[menus/57443/productcategories/5/products](http://api.just-eat.com/menus/57443/productcategories/5/products) returns a list of products for a given category for a given menu (for. menuid = 57433 & categoryid = 5)

### What you need to do

Please create a website using C#, ASP.NET MVC and Visual Studio. The website should have a single page that allows users to enter a postcode and get back a list of restaurants that deliver to that postcode, including the following information:

* Name

* Average rating

* Restaurant logo

* A link to the restaurant on the JUST EAT website

* A list of products the restaurant sell

The restaurants should be ordered from highest average rating to lowest average rating and the restaurants should be loaded using some form of AJAX.

Please take the time to write code and any tests to the standard you would expect in a real application.

### Functional Testing [OPTIONAL] - 60 minutes

Using Ruby & Cucumber or .NET & SpecFlow, write a functional test (both Gherkin scenario and code implementation) which

* Returns a list of restaurants, if the given the postcode is valid; and

* Displays an error message on the site, if the postcode is invalid.

Describe how to run the tests.

## Questions - 45 minutes

1. Did you have time to complete the coding test? What would you add to your solution if you had more time?

2. How would you automate the testing of the website you built?

3. How would you decrease the time taken for the www.just-eat.co.uk home page to load in a browser?

4. What is the most interesting feature in your opinion in CSS 3? Please include a snippet of CSS that shows how you've used it.

5. What's your favourite JavaScript library? Why?

6. How would you improve the customer experience on [www.just-eat.co.uk?](http://www.just-eat.co.uk?)

7. Please describe yourself using JSON.

8. Using [https://gomockingbird.com/mockingbird/](https://gomockingbird.com/mockingbird/) draw the architecture of a system you’ve been working on and you’re proud of. Describe all the moving pieces. Export to PNG and include it in the zip file.

9. Write a list of 5 technologies/frameworks/tools you could not live without.

10. Describe how web form authentication works in .NET. What are the moving pieces, try to be as detailed as possible.

11. Describe the biggest challenge you had when hiring and growing your team