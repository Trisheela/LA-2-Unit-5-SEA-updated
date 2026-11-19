Question 3: DevOps Practices and CI/CD Pipelines
A software company develops an online shopping application. Developers frequently update the application to introduce new features and fix bugs. However, manual testing and deployment are causing delays and errors.
Apply DevOps practices and a CI/CD pipeline to automate the software development and deployment process. Explain the stages involved and identify the benefits of automation.
Expected contribution:
●	Introduction to DevOps
●	Meaning of Continuous Integration and Continuous Delivery/Deployment
●	CI/CD pipeline stages
●	Explanation of build, test, and deployment
●	Three benefits of automation
●	CI/CD pipeline diagram
1. Introduction to DevOps
DevOps is a combination of Development (Dev) and Operations (Ops). It is a software development approach that combines development and operations teams to improve software development, testing, and deployment.

In an online shopping application, developers frequently update the application to add new features and fix bugs. DevOps helps automate these processes, reduce manual work, minimize errors, and deliver software faster.
2. Meaning of Continuous Integration and Continuous Delivery/Deployment
a) Continuous Integration (CI):

Continuous Integration is the practice of frequently merging developers' code changes into a shared repository. Whenever new code is uploaded, it is automatically built and tested to identify errors.

b) Continuous Delivery (CD):

Continuous Delivery is the process of automatically preparing tested software for release. The application is kept ready for deployment, but final deployment to production usually requires manual approval.

c) Continuous Deployment:

Continuous Deployment automatically deploys every code change that successfully passes all testing stages into the production environment without manual approval.
3. CI/CD Pipeline Stages
The following are the stages involved in a CI/CD pipeline:
1. Code: Developers write application code and upload it to a shared repository such as GitHub.
2. Build: The source code is compiled and packaged into an executable application.
3. Test: Automated tests are performed to identify bugs and errors in the application.
4. Release: The successfully tested application is prepared and stored for deployment.
5. Deploy: The application is automatically deployed to the production server or cloud platform.
6. Monitor: The application is continuously monitored to identify errors and performance issues.
4. Explanation of Build, Test and Deployment
a) Build:
- Developers upload the updated source code to GitHub.
- Tools such as Jenkins or GitHub Actions automatically trigger the build process.
- The source code is compiled and converted into a deployable package.
- Any build errors are reported to developers.
Example: Building the shopping application after adding a new payment feature.

b) Test:
- Automated testing is performed on the newly built application.
- Unit testing checks individual components.
- Integration testing checks whether different modules work together.
- Functional testing checks features such as login, shopping cart, and payment.
- If errors are found, developers are notified to fix them.
Example: Testing whether customers can successfully add products to the cart and complete payments.

c) Deployment:
- After successful testing, the application is deployed to the production server.
- Updated features become available to customers.
- Deployment tools automate the release process.
- The application is monitored after deployment.
Example: Deploying the updated shopping application with a new payment option for customers.
5. Three Benefits of Automation
1. Faster Software Delivery:

Automation reduces manual work and speeds up the building, testing, and deployment processes. New features and bug fixes can be delivered quickly.

2. Reduced Human Errors:

Automated testing and deployment reduce mistakes caused by manual operations and improve software quality and reliability.

3. Improved Productivity:

Automation reduces repetitive tasks and allows developers to focus on developing new features. It also provides quick feedback about errors, helping developers fix problems faster.
6. CI/CD Pipeline Diagram
       +----------------------+
       |         CODE         |
       |  Developers upload  |
       |    code to GitHub   |
       +----------------------+
                 |
                 v
       +----------------------+
       |        BUILD         |
       | Compile and package  |
       |    source code       |
       +----------------------+
                 |
                 v
       +----------------------+
       |         TEST         |
       | Unit, Integration &  |
       |   Functional Tests   |
       +----------------------+
                 |
                 v
       +----------------------+
       |        RELEASE       |
       | Prepare application  |
       |    for release       |
       +----------------------+
                 |
                 v
       +----------------------+
       |        DEPLOY        |
       | Deploy application   |
       |  to production       |
       +----------------------+
                 |
                 v
       +----------------------+
       |       MONITOR        |
       | Monitor performance  |
       |  and detect errors   |
       +----------------------+
                 |
                 v
          USER ACCESS
