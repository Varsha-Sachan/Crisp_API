# ASSIGMENT SOLUTION
## Author
### Varsha Sachan
## Clone the Repository
git clone https://github.com/Varsha-Sachan/Crisp_API   # Repository URL <br/>
cd "Crisp_API"                                         # Repository name 
# Install the dependencies
npm install newman <br/>
npm install newman-html-extra
# Run the newman tests:
newman run CrispAPI.postman_collection.json 
-d testdata.csv 
-e UAT-ENV.postman_environment.json 
-r cli,htmlextra 
For the automation purpose I have integrated it with the github actions.

CI/CD Workflow The GitHub Actions workflow automates testing and archiving of reports.

Named newman-html-report-success on success Named newman-html-report-failure on failure
