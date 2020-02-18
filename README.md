# My Life

## 1. Inception Phase

### 1.1. Context

The use of information and communication technologies in the health area is being explored in the most diverse scenarios of diagnosis and treatment of patients.

In the last decade, there has been a proliferation of mobile devices for monitoring vital signs and physical activity of citizens, thus enhancing the emergence of a new paradigm for monitoring clinical conditions and behavioural habits.

On the other hand, it is known that patterns of food consumption have a major impact on health conditions and that more and more citizens are concerned with monitoring their diet, recording the calories and macronutrients they consume and also the calories they spend on physical exercise.



### 1.2. Problem

Due to the growing demand of the labour market, the day-to-day tasks that increasingly fill citizens' schedules and other activities that make up daily life, people have less and less time to monitor their health and perform activities to promote a good lifestyle.

Various technologies on the market try to assist people in this area by providing tools where it is possible to insert the foods consumed daily, but manual insertion is still time-consuming and takes up a large amount of time.

Gymnasiums and personal trainers try to instil a culture of exercise and a healthy lifestyle in citizens, but the prices and the high number of people who frequent this space end up discouraging many citizens from practising a healthy lifestyle.


### 1.3. Personas
- **Medic**

António Silva, 35 years old, born in Ovar,Aveiro, lives in Porto where he currently works as a medic in Hospital de Sao João.

António feels the need to have more information about his patients daily food routine, workout routine, clinical context and other metrics, but he feels that the 5 to 10 min medical appointments aren't enough to gather all this information.

António feels that with an easy-to-use application, where he can access all daily-life details of his patients, he could have more productive appointments and pay more atention to his patients.

- **Patient**

Francisca Barros, 25 years old, born in Águeda, Aveiro, lives in Porto where she works as a Test Enginner in Blip.

Francisca cares about her health, so she tries to have a healthy life, keeping track of her daily food intake and a balanced weekly workout routine. She also likes technology and uses a bunch of high-end gadgets to help her track health metrics like: heart rate and steps taken in a day.

Unfortunately, giving her tight schedule related to work, she doesn't always have the time to track her daily food consuptions or track if she is complying to her workout plan and doing the exercises in a correct way.

Therefore, Francisca feels that with an easy-to-use system, that enables her to track her food consumption in an easy and fast way and also helps her make sure she is complying with her workout schedule and executing the exercises in the correct way, she could have a healthier lifestyle and follow her workout plan in a more rigorous way.

### 1.4. Goal

This project aims to provide an intuitive and effective way to monitor a person's diet and further assist them in the practice of physical exercise, correcting the user when necessary.

With this objective in mind, we intend to develop a web information system that allows the integrated collection and visualization of clinical data sources, physical activity and eating habits related to a citizen's daily life.

The solution should proceed to the automatic collection of different types of data, such as vital signs, regular motor activity, specific physical exercises and ingested food.

On the other hand, the application should allow simplified registration of basic physical and mental health conditions of the person, such as pain in the organ or limb, depression, anxiety, fatigue, etc.

### 1.5. Task List

**Module: OpenPose (Tiago Mendes, João Vasconcelos and Tomás Costa)**
- **Task 1:** Investigate and learn how to use the software [Tiago Mendes, João Vasconcelos and Tomás Costa]
- **Task 2:** Implement a simpler use case of OpenPose [Tiago Mendes,Tomás Costa]

**Module: Computer Vision (ML Food Recognition) (João Vasconcelos, Vasco Ramos and Tomás Costa)**
- **Task 1:** Search and analyse for ml and pattern recognition tools [João Vasconcelos, Vasco Ramos and Tomás Costa]
- **Task 2:** Search for a dataset of foods and respective properties (protein,calories,carbohydrates) [Tomás Costa]

**Module: Service Broker (To connect sensors to our system) (Tiago Mendes and João Marques)**
- **Task 1:** Search viability of using Kafka vs RabbitMq [João Marques and Tiago Mendes]
- **Task 2:** Implement the 1st version of communication [João Marques]
- **Task 3:** Investigate how to connect and retrieve information of FitBit Band [Tiago Mendes]

**Module: Backend (João Vasconcelos, João Marques and Vasco Ramos)**

- **Task 1:** Define what database to use for each cenario [Vasco Ramos and João Vasconcelos]
- **Sub-module: Sensor logic**
    - **Task 1:** Create the database schema [João Marques and Vasco Ramos]
    - **Task 2:** Define the endpoints necessary to the api [João Marques and Vasco Ramos]
- **Sub-module: Operation logic**
    - **Task 1:** Create the database schema [João Vasconcelos]
    - **Task 2:** Define the endpoints necessary to the api [João Vasconelos and Vasco Ramos]
    
**Module: Frontend (Tiago Mendes and Tomás Costa)**
- **Task 1:** Creation of static homepage with minimum information and details of the Project [Tomás Costa e Tiago Mendes]
- **Task 2:** Creation of the login and registration interface (integrations with login apis) [Tomás Costa]

**Module: CI/CD Pipeline (João Marques and Vasco Ramos)**
- **Task 1:** CI Pipeline [Vasco Ramos and João Marques]
- **Task 2:** CD Pipeline [João Marques]

### 1.6. Expected Results

At the end of this project, we expect to have a fully functional application capable of tracking eating habits and physical activity of an individual.

This product will be capable of connecting with fitness trackers (Fitbit Charge 3) and other instruments that will measure data such as the number of steps walked, heart rate, quality of sleep, steps climbed, and other personal metrics involved in fitness.

The user will have the opportunity to track calories, macronutrients and other metrics. By taking a picture of the food, the app will automatically log the calories, proteins, carbohydrates and other metrics for future review by the user. 

The application will be capable of recording workout plans and give you feedback about your performance and posture at the end of the training.

Besides that our users will be connected to a medic that will have access to all the food and workout history of the patient so he can give more precise feedback.

### 1.7. Key system functionalities

- Tracking of calories, macronutrients and other food metrics  through computer vision, enabled by a photo taken by the user.
- Connection with fitness monitoring systems, like fitbit, for more accurate health metrics 
- Movement analysis (OpenPose) for controlling and correcting physical exercises done by the user.

### 1.8. Related work

The following systems, technologies and applications are interesting within the context of our project:
- **Freeletics:** [https://www.freeletics.com/pt/](https://www.freeletics.com/pt/)
- **BiteAI:** [https://bite.ai/](https://bite.ai/)
- **MyFitnessPal:** [https://www.myfitnesspal.com/](https://www.myfitnesspal.com/)
- **OpenPose:** [https://github.com/CMU-Perceptual-Computing-Lab/openpose](https://github.com/CMU-Perceptual-Computing-Lab/openpose)

### 1.9. Communication Plan
 - **Backlog Management** For backlog management we are using [Jira](https://my-life.atlassian.net/secure/RapidBoard.jspa?rapidView=1) (an issue tracker and agile project management application) since it is a widely used tool and provides great project tracking for teams, it ranks number one for software project management tools with requirement tracking, task tracking and version tracking.
 
 - **Git Platform:** For the Git platform we chose [GitLab](https://gitlab.com/_mylife/mylife)  since it has easier CI/CD Integration and several others tools we find useful, as opposed to GitHub.
    - Git Standards:
        - For each new feature create a new branch.
        - For each fix create a new branch
        - Never merge directly, always make pull requests and identify at least one person to check (review) that pull request before merging the PR.  
        - **New feature branch:** or each new feature create a branch following the standard: `feature/<feature_name>`.  
        - **New Issue branch:** For each fix create a branch following the standard: `hotfix/<fix-name`.


### 1.10. Team Roles

- **Product Owner:** [João Vasconcelos](https://jmnmv12.github.io/AboutMePT)
- **DevOps Master:** [João Marques](https://jmarques.icu/)
- **General Developer:** [Tomás Costa](https://github.com/TomasCostaK)
- **Architect:** [Tiago Mendes](htytps://github.com/tiagocmendes)
- **Project Manager:** [Vasco Ramos](https://vascoalramos.me)
- **Advisor:** [Carlos Costa](http://sweet.ua.pt/carlos.costa/)