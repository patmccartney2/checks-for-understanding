## Week Four Recap

### Instructions
Fork or re-pull this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Week 4 Questions

1. What is a cookie? information stored locally on the user's computer containing data for a site.
2. What’s the difference between a session and a cookie? sessions are stored on the server and cookies are stored locally
3. What’s a flash and when do you want to use flashes? a flash is a message that you can display on the page to alert the user to a change they make, ie. adding a user, or putting something into the cart
4. Why do people say “HTTP is stateless”? because HTTP requests don't relate to eachother unless you use a session or a cookie
5. What’s authentication? Explain.  authentication is the use of username and passwords (which are encrypted in a hash)
6. What’s the difference between authentication and authorization? Authenitcation is checking who the user is, i.e. registered user, admin, visitor, while authorization is what each of those roles is given access to.
7. What’s a before filter? its a way to make sure a user has to have the right authorization to access a page. i.e. to check iff a user is an admin before moving to the bike-share admin data pages
8. How do we keep track of a user once they’ve logged in? we keep track of users in the sessions
9. When do you want to namespace a resource? When do you want to nest a resource? What's the differences between those two approaches? Name spacing gives the program the ability to have a seperate folder for admin controllers where we can keep admin only information and features.  Nesting resources gives the resource_1/resource_1.id/resource_2.  You use it to make relationships more apparent in the routing.
10. At a high level, what tools can you use to implement authorization? How would you use them? I'm slightly confused by the question.
11. What's an enum, and what advantages does it offer? What data type needs to be in your database to use an enum? Where do you declare an enum?   Its a way to 'give more attributes' to a table by assigning an integer value to a column.  You can then assign names to each number that can be placed into the column, 1 = thing_1, 2 = thing_2, 3 = thing_3.
12. What are some strategies you can use to keep your views DRY?


### Reviews Questions 
13. Given the following array of hashes, how would I print an alphabetical list of holidays?
```ruby
[
 {holiday: {name: "St Patrick's Day", supplies: ["Corned Beef and Cabbage"]}},
 {holiday: {name: "Halloween", supplies: ["Candy", "Costume"]}},
 {holiday: {name: "Hanukkah", supplies: ["Menorah"]}}
]
return_value = []
array.each do |holiday|
 return_value << holiday[:name]
 end
 return_value.sort
end
```  

holidays.
14. How would you clean incoming data to ensure "$300" or "300.00" is stored as 300? 
string.to_i ?

### Self Assessment:
Choose One:

* I was able to answer most questions independently, but utilized outside resources for a few


Choose One:
* I feel overwhelmed by the content presented this week
*** but bike share is improving my comfort with these concepts.

