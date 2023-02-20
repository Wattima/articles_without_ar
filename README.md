# Magazine Article Tracker
This is a simple Ruby project that allows you to track articles and authors for various magazines. It includes three classes: Author, Magazine, and Article.


## How to Use
Once you've run the run.rb file, you can interact with the code by following the prompts in the terminal. The code includes the following classes and methods:

### Author
initialize(name): Creates a new author with the given name.
name: Returns the name of the author.
articles: Returns an array of all the articles written by the author.
magazines: Returns a unique array of all the magazines the author has contributed to.
add_article(magazine, title): Creates a new article with the given title and associates it with the author and the given magazine.
topic_areas: Returns a unique array of all the topic areas the author has written about.

### Magazine
initialize(name, category): Creates a new magazine with the given name and category.
name: Returns the name of the magazine.
category: Returns the category of the magazine.
all: Returns an array of all the magazines that have been created.
find_by_name(name): Returns the first magazine object that matches the given name.
article_titles: Returns an array of all the article titles for the magazine.
contributors: Returns an array of all the authors who have written for the magazine.

### Article
initialize(author, magazine, title): Creates a new article with the given author, magazine, and title.
title: Returns the title of the article.
all: Returns an array of all the articles that have been created.
author: Returns the author of the article.
magazine: Returns the magazine of the article.


## License
This project is licensed under the MIT License. Feel free to use and modify this code for your own purposes.









