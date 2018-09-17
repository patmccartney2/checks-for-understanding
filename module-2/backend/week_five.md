### Week 5 Questions

Re-pull from this repository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!).

Note: When you're done, submit a PR.

### Week 5 Questions
1. How do we make flash messages display on a page?  set up a flash message in the layout and then call it in the controller when you need it.

2. Where is cart information/temporary information usually stored? in a session

3. What might be some reasons not to store a cart in our database? Are there any reasons why we would want to persist that information? It will make us manipulate/query the database more making our lives more difficult and slowing down the speed of the app.

4. What is the purpose of the asset pipeline?
asset pipelines are ways to edit the views of our apps.  IT allows the use of javascript, css, and erb in our code.

5. Why do we precompile our assets?
to save data and processing speed?

6. What do each of the following tags do?

```ruby 
<%= stylesheet_link_tag "application" %> -> imports css to allow styling
<%= javascript_include_tag "application" %> -> allows importation of javascript
<%= image_tag "rails.png" %> -> adds an image to the view
```

7. What are some of the elements of a great read me? What are some of the benefits of taking the time to update a readme for our project?
set up instructions
a brief explanation of the appplication
any requirements for your system to use the application
any gems or cross dependencies that your app relies on

8. What are the top four accessibility issues that we as developers should be aware of?
Visual
Motor
Hearing
Cognitive

9. `before_save` is an example of a what? Where in our Rails application would we find a `before_save`?
it is an example of a callback.  When something is saved it will execture an action.  We use it when creating or updating an object.

10. Given the following object, how would we create a scope for all users who are active?

```ruby 
User.create(name: "Happy", active: true)
```
User.where(active: true)

11. What is the difference between a scope and a class method?
scope narrows database queries a method is just a class function.


### Review Questions:  
12. Given the following hash:  

```ruby
{cart: {"17" => 4, "204" => 52, "29" => 22}}
```

  12a. How would you add item with id of 48 with a quantity of 4?  
  cart[48] = 4
  12b. How would you increase the quantity of item 29? 
  cart["29"] + quantity
  12c. How would you find out how many items your user is thinking about purchasing? 
  cart.count
  
13. What is polymorphism? How does it relate to duck-typing? What are two ways you use this in everyday Rails applications? 
It alllows a model to belong to multiple objects. 
14. How would you clean the string "(630) 854-5483" to "630.854.5483"?  you can use gsub.


### Self Assessment:
Choose One:

* I was able to answer most questions independently, but utilized outside resources for a few

Choose One:
* I feel comfortable with the content presented this week

