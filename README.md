# HAPI FHIR Playground: Basic Test App

This project is a skeleton project for querying data from the [HAPI FHIR public test server](http://hapi.fhir.org/baseR4)

### Getting Started:

* [ ] Take a few minutes to familiarize yourself with the [FHIR Standard](http://hl7.org/fhir/) for health data exchange. In particular, you might want to read the [Executive Summary](http://hl7.org/fhir/summary.html) and the [Developer Introduction](http://hl7.org/fhir/overview-dev.html)

* [ ] Use whatever library & framework you're most comfortable with.
  
* [ ] Create your own GitHub project and copy the contents of this repository into your own project.

* [ ] **Please, do not fork this repo.** Create your own private GitHub repository to do your work in.

### Basic Tasks:

* [ ] Create a patient view with patients fetched from `https://try.smilecdr.com/baseR4/Patient`. The patients should be sorted by name & birthdate (if a birthdate is in the record). 

* [ ] Display the first & last names, date of birth, address, gender & phone number.
 
* [ ] Ensure the table is responsive. Ensure there is proper error handling for missing elements in the data.

* [ ] Time the request. Output the time on the footer of the page in a human readable format.

* [ ] Add a search function to the page. Add two inputs to your view - one for first name, and one for last name.  Make an API call to `https://try.smilecdr.com/baseR4/Patient?given=<userinput>&family=<userinput>` that searches for a `Patient` based on the names passed in. Replace `<userinput>` with the data from the inputs. If only one name is entered in the inputs, modify the query to only use either the first or last name entered.

* [ ] Add a function to reset the search results in the table.

* [ ] Apply validation to the inputs - the boxes cannot contain non-alphabetic characters.

* [ ] Commit your work.

### Intermediate Tasks:

* [ ] All tasks in the [Basic Tasks](#basic-tasks) section must be completed.

* [ ] Create a navbar, implement routing from the patient view to another view, the questionnaire view.

* [ ] In the questionnaire view, _dynamically_ generate a form using the `questionnaire.json` file in the `assests` folder. The form should have validation applied to each input. 

* [ ] Using the results from the form, generate a [`QuestionnaireResponse`](https://www.hl7.org/fhir/questionnaireresponse.html). The `QuestionnaireResponse` should follow the structure outlined in the [Resource Content Section](https://www.hl7.org/fhir/questionnaireresponse.html#resource)

* [ ] Display your results at the bottom of the page.

* [ ] Commit your work.
