# Assignment 3 - Write UP

## Description
This assignment completes our movie chatbot system by implementing action functions that query our movie database and building a natural language interface. You implemented functions to search for movies by year, director, and actors, as well as the core search system that matches user queries to appropriate database operations. This builds directly on the pattern matching work from Assignment 2 to create a functional conversational AI system.

## What to complete
1. Complete all action functions in `a3.py` (title_by_year, title_by_year_range, etc.)
2. Implement the `search_pa_list` function to handle pattern matching and responses  
3. Add at least one new movie to the database with proper formatting
4. Create a new pattern/action pair and add it to the pa_list
5. Ensure all provided assert statements pass
6. Complete the reflection questions below
7. Push your code to github for grading

## Reflection Questions

1. What are some key programming concepts or techniques that you learned while completing this assignment?

While completing this assignment, I learned more about specific things in python that you can't do in Java. For example, I learned that when you're using multiple conditional statements, python makes it easier. For example, if you wanted to check if z < x < y, in Java, you would have to do if x > z && x < y. In Python, you can just do if z < x < y. Another thing that I learned while completing this assignment was how to create an assert statement. Also, I learned how to create a "project" by using multiple different files and components, such as the match function, the database, etc, and seeing how they all interact and work with each other in order to create the chatbot. 

2. How does the overall movie chatbot system work? Explain the flow from when a user types a query to when they receive an answer.

First the user enters a query. Then, the match function takes the query andd extracts the necessary information from it, like the movie title, actors, year it was made, director, etc. Then, it takes the original source and uses it in the search_pa_list function in order to determine which action function needs to be called in response to the query. Once the necessary action function is determined, the program inputs the list of Strings that it extracted from the match function into the action function and returns the output.

3. What are some real-world applications where this type of pattern-matching chatbot system could be useful? How might you extend or improve this system for practical use?

Some real-world applications where this type of pattern-matching chatbot could be useful are for creating chatbots about anything in general. The way that the chatbot is set up makes it so that it is very easy to change the database, whether it be adding, deleting, or changing things, so that it's easily adaptive. This makes it so that the chatbot has longevity and can be used for a long time. If I were to extend or improve this system for practical use, I would maybe make the database bigger, or make it so that the database can access the internet so that the program could pull the information directly from the internet.