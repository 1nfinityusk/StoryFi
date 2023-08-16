# StoryFi
Prototype_code


Objective
To create a prototype of a browser application called "StoryFi". As the frontend design has been developed in WIX, we aim to integrate it with Azure Open AI and other tools to ensure the application is fully functional.

Overview
From the mobile site developed in Wix, we offer a service that creates a personal guide for users based on the information they provide.

System Method & Structure
Users are asked to upload a character of a famous person they admire on Wix.

Based on the uploaded data, Azure Open AI searches for the character on Google to verify its identity.

Once the character verification is complete and the person is identified, the following prompt is sent to Azure Open AI to generate a response:

Prompt:
"I admire a way of life like [name of the selected person will automatically appear here]. From this, please list 50 values that you believe might inherently exist within me."

→ The response will be output within Azure: We'll refer to this response as Response A.

Next, considering Response A, the following prompt is sent to receive a reply:

"Based on the above 50 values, please deduce and formulate my brand personality in regards to:

Belief
Strengths and Weaknesses
Talent
The ideal future worldview
The most cherished value in one word
Please include a creative and concise catchphrase for each."
→ The response will be output within Azure: This will be termed as Response B.

Users are asked to choose their business skills, creative skills, and soft skills via tabs. Based on this information, the following prompt is sent to Azure:

"My creative skills are '[the chosen skills will be sent here]'. My business skills are '[the chosen skills will be sent here]', and my soft skills are '[the chosen skills will be sent here]'. Combining this information with the 50 values listed and my brand personality, please formulate:

Vision (Purpose of life)
Mission (Mission statement)
Core Values (Values you possess)
Strategy (Methodology)
Concept (Theme) for my life's brand story."
→ This will be termed as Response C.

5-2 Based on Response C, a roadmap for achieving the vision over three years is generated.

"Please formulate a three-year roadmap to achieve my vision."

→ This will be referred to as Response C'.

When users enter their favorite scenery in text on Wix, the scenery will be uploaded onto Wix from Azure Open AI. This output will be stored and termed as Response D.
6-2 Based on Response D, the action plan created by Response C' is plotted on a world map that uses the D scenery as a motif. → This will be termed as Response E.

Prompt:
"Create an original flat map for me using the scenery derived from Response D. On this map, please mark landmarks using star shapes based on the roadmap from Response C'."

6-3
The personality from Response B is embedded into the Wix page.
The brand story from Response C is embedded into the Wix page.
The map from Response E is embedded into the Wix page.

Users can choose to either start over or confirm that everything is okay.

If "OK" is chosen, users can log in and ask questions regarding the next actions anytime.
