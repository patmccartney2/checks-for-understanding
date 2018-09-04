## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!).

Note: When you're done, submit a PR.

### Week 1 Questions

1. List the five common HTTP verbs and what the purpose is of each verb.
get - read
post -create 
delete - destroy
put/patch- update

2. What is Sinatra?
Sinatra is a framework to run Rack to make web applications

3. What is MVC? 
The archictecture for a web app: Model View and Cotroller

4. Why do we follow conventions when creating our actions/path names in our Sinatra routes?
to protect our code from users

5. What types of variables are accessible in our view templates without explicitly passing them?
query parameters passed through the URI

6. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?

  ```ruby
  get '/horses' do
    @count = '1'
    name = 'Mr. Ed'
    erb :index :locals => { :name => name }
  end
  ```

7. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed` to the view?

8. What's the purpose of ERB?
An ability to manipulate data in our views

9. Why do I need a development AND test database?
One is for the live app and one is only for your tests.  You do not want to mess with a live database and risk losing all of its data

10. What is CRUD and why is it important?
Create
Read
Update
Destroy
it is the standard for building out the way a user can interact with our apps.

11. What does HTTP stand for?
Hypertext Transfer Protocol

12. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?
<% %> will not display on the page
<%= %> will display on the page

13. What's an ORM? What does it do?
Object Relational Mapping.  It is a way to query databases

14. What's the most commonly used ORM in ruby (Sinatra & Rails)?
SQL

15. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.
READ '/restaurants' - GET all restaurants from index.erb
READ '/restaurants/:id' - GET single restaurants from show.erb
CREATE 'restaurants/new' - GET a form to create a new restaurants in new.erb
CREATE '/restaurants' - POST new data to the server and redirect to '/restaurants'
UPDATE '/restaurants' - GET a form update an existing restaurants from edit.erb
UPDATE '/restaurants/:id/edit' - PUT data to the server to update existing restaurant
DELETE '/restaurants/:id' - DELETE existing information

16. What's a migration?
migrations are a way for us to make changes to our database

17. When you create a migration, does it automatically modify your database?
No.  You must run the migration, and make sure the changes are reflected int eh schema.

18. How does a model relate to a database?
models are the objects that make up each table

19. What is the difference between `#new` and `#create`?
New creates the object that can be saved to the data base with .save
create is new and save in one method

20. Given a table named `animals`, What is the SQL query that will return all info from that table?
    `id     name        number_of_legs
    -----   ------      --------------
      1     panda       4
      2     giraffe     4
      3     whale       0
      4     bird        2
      
 SELECT * FROM animals;
    `

21. Using the same table, What is the SQL query that will return only the animals that has 4 legs?
SELECT * FROM animal WHERE number_of_legs = 4


### Review Questions:  
22. Given a CSV file (“films.csv”) with these headers [id, title, description], how would you load these into your database to create new instances of Film?  
rake db:seed

23. Given the following hash:
```
activities = {
  hiking: {cost: $0, supplies: ['hiking shoes', 'water', 'compass']},
  karaoke: {cost: $10, supplies: ['courage', 'microphone']},
  brunch: {cost: $35, supplies: ['mimosa flutes']},
  antiquing: {cost: $200, supplies: ['list of antique stores']}
}
```
How would I add 'granola bar' to things you should have when hiking?
??

24. What are the 4 Principles of OOP? Give a one sentence explanation of each.
Abstraction 
Inheritance
Encapsulation
Polymorphism
unsure of defininitions


### Self Assessment:
Choose One: (erase the others)
* I was able to answer most questions independently, but utilized outside resources for a few


Choose One:
* I feel comfortable with the content presented this week

