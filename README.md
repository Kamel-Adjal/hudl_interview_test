# Hudl Serenity BDD Test Suite

## Run Tests

```bash
mvn clean verify -Dusername=your.email@domain.com -Dpassword=yourSecurePassword
```
# HUDL Serenity BDD Test Suite

This project is a sample UI automation framework developed as part of a technical interview for a QA Manager position. 
It uses **Java**, **Serenity BDD**, **Cucumber**, and **Maven** to automate and validate the login, account creation, 
and password reset features on the HUDL platform.

## 🔧 Tech Stack

- **Java** 11+
- **Serenity BDD**
- **Cucumber (Gherkin)**
- **Maven**
- **JUnit**

## 🚀 Getting Started

### Prerequisites
Make sure the following tools are installed and available in your system's PATH:

- **Java JDK 11 or higher**: [Download JDK](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html)
- **Apache Maven 3.6 or later**: [Download Maven](https://maven.apache.org/download.cgi)
- **IntelliJ IDEA or any Java IDE**

You can verify installations via terminal:

```bash
java -version
mvn -version

```
## 💻 Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/Kamel-Adjal/hudl_interview_test.git
cd hudl_interview_test
```

### 2. Import Project into IntelliJ IDEA
- Open IntelliJ IDEA
- Click on **File > Open...** and select the project folder
- IntelliJ will detect it as a Maven project and automatically import dependencies
- If not, click **View > Tool Windows > Maven**, then click the refresh icon

### 3. Build the Project
```bash
mvn clean install
```
This will compile the code and run the tests.

---

## ▶️ Running the Tests

To execute all tests:
```bash
mvn clean verify
```
To run a specific feature or tag:
```bash
mvn verify -Dcucumber.filter.tags="@login"
```
> Serenity reports will be generated in:
```
target/site/serenity/index.html
```
Open it in your browser to view detailed test results and screenshots.

---

## 📁 Project Structure

```
src
├── test
│   ├── java
│   │   ├── pages                  # Page Object Models
│   │   ├── runners                # Test Runner
│   │   └── stepdefinitions        # Step Definitions for BDD
│   └── resources
│       └── features               # Gherkin feature files
```

---

## ✅ Scenarios Automated

### Login Feature
- Valid login with email/password
- Login with invalid email format
- Login with Google button visibility

### Account Creation
- Successful account registration flow

### Password Reset
- Request password reset link with valid/invalid email

---

## 📊 Reports

After test execution, a detailed Serenity HTML report is generated:
```
target/site/serenity/index.html
```

---

## 📌 Notes

- Element locators are managed via Serenity's `@FindBy` with `WebElementFacade`.
- Tests follow the Page Object Model and BDD best practices.
- Modular and easy to scale.

---

## 🧑‍💻 Author
**Kamel Adjal**  
[LinkedIn](https://www.linkedin.com/in/kameladjal/)

---

## 📄 License
This project is for demonstration/interview purposes only.

