# Postman API Automation Integration with Github Actions
This repository is a demonstration for POC for integrating postman tests with github actions. The tests are written in Postman and they are executed on the VM with the help of newman and newman-reporter-htmlextra.
Github actions will trigger the project execution on every push to the main branch. You can also execute the project manually workflow_dispatch. Thr Project runs on a scheduled time using cron job. 


The HTML reports are archieved and kept in the artifact section for the team to download it. Along with that they can view the report directly from the github page : https://somok96.github.io/Phoenix-In-Warranty-Flow/
The latest report is mailed to the team members using GMAIL SMTP.

## About Me ## 
Hi My Name is Somok Mukherjee. I have 4+ years of experience in Automation and Manual Testing. My Skillset includes UI Automation with Selenium and for API Testing I use Rest Assured and Postman. 

You can connect with me over : www.linkedin.com/in/somok-mukherjee

## Testing Coverage ##
1. Happy Flow Testing
2. Negative Testing and Edge Case Testing
3. Token Testing
4. Schema Validation
5. Secrets Management with Github secrets

## HTML Report ##
The report will be created in the newman folder 
![Postman Report](https://github.com/somok96/Phoenix-In-Warranty-Flow/blob/static-content/newman-report.jpg)

## Project Structure ##
```
Phoenix In Warranty Flow
├─ Inwarranty flow collection Copy.postman_collection.json # Colletion File
└─ QA.postman_environment.json # Environment File

```

## Tech Stack ##
1. Postman
2. NodeJS 22
3. Newman
4. Newman-Reporter-Htmlextra
5. Github Actions
6. Gmail SMTP
7. Github Pages
8. AWS EC2 for Self Hosted Github Runner

## How to run the project? ## 
You can run the project on your local system for that : 
1. Clone the Project on Local System : https://github.com/somok96/Phoenix-In-Warranty-Flow.git
2. Install NodeJS and NPM from https://nodejs.org/en
3. Install Newman using npm install -g newman
4. Install Newman-reporter-htmlextra npm install -g newman-reporter-htmlextra
5. Run the Newman Command :
   ```
              newman run 'Inwarranty flow collection Copy.postman_collection.json' \
             -e QA.postman_environment.json \
             -r cli,htmlextra \
             --reporter-htmlextra-export ./newman/index.html
   ```

## Github Pages ##
You can directly view the latest test report of the Postman Test at the Github Page Link: https://somok96.github.io/Phoenix-In-Warranty-Flow/





