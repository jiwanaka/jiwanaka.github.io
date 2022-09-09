---
layout: essay
type: essay
title: "Asking Smart Questions"
# All dates must be YYYY-MM-DD format!
date: 2022-09-08
published: true
labels:
  - StackOverflow
  - Thoughts
  - SMART Question
---


Have you ever just gotten stuck on a problem or a situation that feels beyond you and you need an answer that clears all the confusion? I’m sure that every single person has had a burning question that absolutely required an answer. You can ask a question, but the person providing the answer needs to receive a SMART question to be able to answer concisely and correctly. To provide a smart question you should exhaust these options before attempting to write a query to a forum or a site because your question might already have been answered in a discernible way. Such options are:


1. Try to find an answer by searching the archives of the forum or mailing list you plan to post to.
2. Try to find an answer by searching the Web.
3. Try to find an answer by reading the manual.
4. Try to find an answer by reading a FAQ.
5. Try to find an answer by inspection or experimentation.
6. Try to find an answer by asking a skilled friend.
7. If you're a programmer, try to find an answer by reading the source code.


The first thing to look out for when formulating a smart question would be to understand the problem you are trying to solve because if you do not know what you are asking then how can the person answering understand how they need to answer the question. Formatting the question is also extremely important because you need to be able to get your question across without any confusion from things such as grammar issues. The title of the question also needs to be specific so people who are experts in what you are trying to ask are able to see it when scrolling through countless other questions. Finally, you need to show that you have made attempts at understanding your own question through things such as the code you wrote and a rundown of what you are trying to achieve. Many will be more willing to help if you made it look like you have put effort into trying to solve your own problem. 
There are many programming questions constantly being asked day after day on Stack Overflow which is filled with both smart and silly questions. By showing an example of both a smart question and a not so smart question, it should hopefully help those that have issues asking questions on these types of forums.

## Example: Asking a Smart Question

Link to question asked by Felix Kling on [StackOverflow](https://stackoverflow.com/questions/14220321/how-do-i-return-the-response-from-an-asynchronous-call)
```
Q: “How do I return the response from an asynchronous call”

How do I return the response/result from a function foo that makes an asynchronous request?
I am trying to return the value from the callback, as well as assigning the result to a local variable inside the function and returning that one, but none of those ways actually return the response — they all return undefined or whatever the initial value of the variable result is.
Example of an asynchronous function that accepts a callback (using jQuery's ajax function):

Example of an asynchronous function that accepts a callback (using jQuery's ajax function):

function foo() {
    var result;

    $.ajax({
        url: '...',
        success: function(response) {
            result = response;
            // return response; // <- I tried that one as well
        }
    });

    return result; // It always returns `undefined`
}
Example using Node.js:

function foo() {
    var result;

    fs.readFile("path/to/file", function(err, data) {
        result = data;
        // return data; // <- I tried that one as well
    });

    return result; // It always returns `undefined`
}
Example using the then block of a promise:

function foo() {
    var result;

    fetch(url).then(function(response) {
        result = response;
        // return response; // <- I tried that one as well
    });

    return result; // It always returns `undefined`
}
```

This is considered a smart question because the format is clear and their question is specific enough that there can be a clear answer. The question provides code that the original poster attempted in understanding the topic they were trying to ask. In the end, the post received thousands of upvotes because it proved useful to many other users and was a smart question to ask. The responses are clear and detailed due to how the question was provided.

## Example: Not So Smart Question:

Link to question asked by Datamatiker50 on [StackOverflow](https://stackoverflow.com/questions/73650419/why-cant-i-get-the-loop-to-work-wombats-not-targeting-leaf-within-1-cell)
```
Q: “why can't I get the loop to work? Wombats not targeting Leaf within 1 cell?”
 
Can't seem to find the issue with the loop. created in a Greenfoot scenario, new to programming here:
 
     /** Enables Wombat to 'seek' for Leaves within 1 cell 360 degrees. */
    public void goToLeaf() {
        for (int x = -1; x <= 1; x++) {
            Actor blad = getOneObjectAtOffset(x, getY(), Leaf.class);
            if (blad != null) {
    
            }
            if (x == -1) {
                setDirection(WEST);
            } else if (x == 1) {
                setDirection(EAST);
            }
        }
        for (int y = -1; y <= 1; y++) {
            Actor blad = getOneObjectAtOffset(getX(), y, Leaf.class);
    
            if (blad != null) {
    
            }
            if (y == -1) {
                setDirection(NORTH);
            } else if (y == 1) {
                setDirection(SOUTH);
            }
        }
    }
 ```
The question above is particularly bad because the wording of the question does not show any thought into what they are asking and reads like someone just wanting answers for their own homework question. They just show a block of code for someone to figure out and discern what they have even attempted and show a lack of effort and research. This leads to no responses and a few individuals downvoting and reporting the post for its lack of research. 
 
## Conclusion
 
I’m sure there are many out there who never even really thought about how their question is perceived by those reading their question. There will always be a need for questions as no one is a master of every single subject, so learning how to ask a proper SMART question is a necessity. 
