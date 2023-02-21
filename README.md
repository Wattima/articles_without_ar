# Magazine Article Tracker
This is a Magazine Management System that allows users to manage magazines, authors, and articles. The system allows users to create new magazines, authors, and articles, as well as view and edit existing ones.


## How to Use
Once you've run the run.rb file in the lib folder *(ruby bin/run.rb)*, you can interact with the code by following the prompts in the terminal. The code includes the following classes and methods:

### Author
initialize(name): Creates a new author with the given name.

name: Returns the name of the author.

articles: Returns an array of all the articles written by the author.

magazines: Returns a unique array of all the magazines the author has contributed to.

add_article(magazine, title): Creates a new article with the given title and associates it with the author and the given magazine.

topic_areas: Returns a unique array of all the topic areas the author has written about.

#### BDD
Given an Author with a name,
When I call the `name` method,
Then it should return the name of the Author.

Given an Author with a list of Article instances,
When I call the `articles` method,
Then it should return an array of Article instances the author has written.

Given an Author with a list of Article instances,
When I call the `magazines` method,
Then it should return a unique array of Magazine instances for which the author has contributed to.

Given an Author,
When I call the `add_article` method with a magazine instance and a title,
Then it should create a new Article instance and associate it with the author and the magazine.

Given an Author with a list of Article instances,
When I call the `topic_areas` method,
Then it should return a unique array of strings with the categories of the magazines the author has contributed to.


#### Pseudo Code
class Author
1. Start.Create a class called Author
2. Add an initialize method that takes one parameter, name
3. Set an instance variable called name to the name parameter
4. Add a getter method called name that returns the value of name
5. Add an instance variable called articles set to an empty array
6. Add an instance variable called magazines set to an empty array
7. Add an instance method called add_article that takes two parameters, magazine and title
8. Create a new Article instance with the author, magazine, and title parameters
9. Add the Article instance to the articles array of the author
10.Add the magazine to the magazines array of the author
11. Add an instance method called articles that returns the articles array of the author
12. Add an instance method called magazines that returns the magazines array of the author
13. Add an instance method called topic_areas that returns a unique array of strings with the categories of the magazines the author has contributed to.
14. end


### Magazine
initialize(name, category): Creates a new magazine with the given name and category.

name: Returns the name of the magazine.

category: Returns the category of the magazine.

all: Returns an array of all the magazines that have been created.

find_by_name(name): Returns the first magazine object that matches the given name.

article_titles: Returns an array of all the article titles for the magazine.

contributors: Returns an array of all the authors who have written for the magazine.

#### BDD
Given a Magazine with a name and category,
When I call the `name` method,
Then it should return the name of the Magazine.

Given a Magazine with a name and category,
When I call the `category` method,
Then it should return the category of the Magazine.

Given a Magazine with a name and category,
When I call the `name=` method with a new name,
Then it should update the name of the Magazine.

Given a Magazine with a name and category,
When I call the `category=` method with a new category,
Then it should update the category of the Magazine.

Given a list of Magazine instances,
When I call the `all` method,
Then it should return an array of all Magazine instances.

Given a list of Magazine instances and a name,
When I call the `find_by_name` method,
Then it should return the first magazine object that matches the name.

Given a Magazine with a list of Article instances,
When I call the `article_titles` method,
Then it should return an array string of the titles of

#### Pseudo Code
1. Start. Create a class called Magazine
2. Add an initialize method that takes two parameters, name and category
3. Set instance variables called name and category to the name and category parameters
4. Add getter methods called name and category that return the values of name and category
5. Add a class variable called all set to an empty array
6. Add an instance method called article_titles that returns an array string of the titles of all articles written for that magazine
7. Add an instance method called contributors that returns an array of Author instances who have written for this magazine
8. Add a class method called find_by_name that takes a string name and returns the first Magazine object that matches
9. end


### Article
initialize(author, magazine, title): Creates a new article with the given author, magazine, and title.

title: Returns the title of the article.

all: Returns an array of all the articles that have been created.

author: Returns the author of the article.

magazine: Returns the magazine of the article.

#### BDD
Author.new(name) takes a string name and returns an instance of Author with the name instance variable set to name.

Author#name returns the name instance variable.

Author#articles returns an array of all Article instances that have this author as their author.

Author#magazines returns a unique array of Magazine instances that this author has contributed to.

Author#add_article(magazine, title) takes a Magazine instance and a string title, creates a new Article instance with this author, the given magazine, and the given title, and returns the new Article instance.

Author#topic_areas returns a unique array of category strings for Magazine instances that this author has contributed to.

#### Pseudo code
1. Create a class called Article
2. Add an initialize method that takes three parameters: author, magazine, and title
3. Set instance variables called author, magazine, and title to the author, magazine, and title parameters
4. Add getter methods called author, magazine, and title that return the values of author, magazine, and title
5. Add a class variable called all set to an empty array
6. Add a class method called all that returns an array of all Article instances




## License
This project is licensed under the MIT License. Feel free to use and modify this code for your own purposes.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
Copyright (c) 2023 **Daryl Wattima**









