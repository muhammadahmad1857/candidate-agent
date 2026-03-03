# Multi-Agent Autonomous Human Capital (HR) System

## Core Multi-Agent Functionalities

1. Job Search Agent
Crawls job boards, company career pages, and platforms (keep in mind same company posts
job on different platforms, you have to remove the duplication)
Matches roles based on skills, experience, location, and preferences

2. Resume & Profile Building Agent
Generates and optimizes resumes tailored to specific roles
ATS-optimized formatting and keyword alignment
LinkedIn and professional profile enhancement

3. Apply Agent
Fetches the HR emails of shortlisted organisations
Prepare to apply to relevant jobs on Gmail
Customizes resumes and cover letters per application and send to HR
Tracks application status and responses

4. Job Preparation Agent
Interview preparation (technical + behavioral)
Mock interviews and Q&A simulations
Skill gap analysis and learning recommendations

5. Orchestration & Memory Layer
Central controller to manage agent collaboration
Shared short-term and long-term memory
Continuous learning and performance optimization


The above flow is not always fix. User may ask only 1-2 above tasks not full flow. It’s the main
agent who has to decide agent(s) will be activated and their flow will be decided.


Make chat interface where user can put any kind of query and orchestrator reads that query identify the intent, make relevant agents ready, do routing, make relevant tools ready.
Don’t make it like a SaaS product it’s digital FTE (means one window solution)


In order to keep track what exactly agents are doing you can make separate tabs for example I want to see what jobs the scrapper has fetched from linkedin or indeed i just click on that tab and see the list or I want to see how many applications I have sent via email it should have that track record and similiar for other tracking.


Make it Human In The Loop (HITL), means before sending emails and agent should show me that I have modified your CV in this this way, do you approve it to send to HR? I may say to make changes in CV before sending or any kind of action. It’s up to you where you show these
editable CVs either in chatbot interface or create a separate section or tab or whatever where user will click and see the newly designed CVs built by agent.


Don’t forget to use lanchain’s libraries like langfuse, langsmith for observability and controllability. Agents should not work anything as hidden. It should clearly show what it is doing, all the traces, handoffs and middleware and user can interrupt any time in the middle if anything is going wrong.

**Some important external links for you:**


1. Efficient CV building prompt:
Go to my Github and take the source code of BowJob I am going to make it public for this week
only for you guys to see how CV making prompts look like, just clone it into your repo and first
see how full project is working and then CV parsing and CV JD matching.
https://github.com/rurahim/BowJob.git
Also Starred button to save it
2. Jobs fetching APIs and HR emails
Searching any kind of API market on Google for this purpose, make account n get your API
https://apify.com/
3. Gmail integration
Go to google developer and get your API key to attach gmail and other google products