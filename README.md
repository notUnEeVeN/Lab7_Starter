# Lab 7 - Starter
Tybalt Mallet, No partner

1. Definitely #1, within a github action that runs whenever code is being pushed, this selection allows us to not rely on the developers remembering to do it every time (#2), and prevents a human mistake from ocurring. Also this automated check would happen before code is merged into the rest of the codebase, thus always catching bugs before they actually impact the rest of the project. Running after development becomes significantly more complicated, and it will often be more difficult to go back and fix everything after the fact, as major unnoticed issues could occur, that would otherwise be preventable from consistent testing.

2. No, end to end tests are for testing user flows through the whole app. Unit tests are the common for testing more simple things such as the validity of the output of a function.

3. Navigation mode analyzes the page right when it loads, and is meant to provide you with insight on things such as load time and other dynamic properties, the execution of your javascript and other metrics such as those that is dependant on the loading. The snapshot, as the name suggests just looks at the website at that specific moment in time, not taking into consideration loading or things like that, this would be more useful for the static properties that stay the same, meta data, header infromation etc. 

4. Three things we could improve based on Lighthouse:
    - The accesibility tab has a score of 90, due to the lack of [lang] attributes in the html, which limits different users ability to interpret the content of the webpage
    - The document is lacking meta descriptions according to the SEO section, which as the section implies would make it more difficult for users to actually find our website 
    - We seem to have a suboptimal 'Network dependancy tree' , and are chaining critical requests, by reducing the length of these chains, we could improve the page load.
