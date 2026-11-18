# DevOps Practices and CI/CD Pipelines

**USN:** NB25CSE182
**Subject:** Software Engineering
**Unit:** V - Software Applications and Emerging Trends

---

## Problem Statement

A software company develops an online shopping application. Developers frequently
update the application to introduce new features and fix bugs. However, manual testing
and deployment are causing delays and errors. DevOps practices and a CI/CD pipeline
are applied to automate the development and deployment process.

---

## 1. Introduction to DevOps

DevOps is a set of cultural practices and tools that increases an organisation's
ability to deliver applications and services fast. It unifies the **Development** and
**Operations** teams, which traditionally worked in separate silos.

Earlier, developers threw the code "over the wall" to the operations team, who then
struggled to deploy it. In DevOps the same team owns the code from the first commit up
to production and monitoring.

**The DevOps infinite loop:**

```
Plan -> Code -> Build -> Test -> Release -> Deploy -> Operate -> Monitor -> back to Plan
```

**Core DevOps practices**

| Practice | Meaning |
|---|---|
| Continuous Integration (CI) | Developers merge code into a shared repository often. Each merge triggers an automated build and test. |
| Continuous Delivery | Code is always ready to release, but the final deployment is triggered manually. |
| Continuous Deployment | Every change that passes the tests goes to production automatically. |
| Infrastructure as Code (IaC) | Infrastructure is defined and provisioned through code, for example Terraform. |
| Continuous Monitoring | Live systems are monitored for performance and errors, feeding back into planning. |

Containers also support DevOps. **Docker** packages the app with everything it needs so
it runs the same on any machine, and **Kubernetes** deploys and scales many containers.

---

## 2. Meaning of Continuous Integration and Continuous Delivery / Deployment

**Continuous Integration (CI):** developers merge their code into a shared repository
several times a day, and every merge automatically starts a build and runs the tests.
Since the mainline is rebuilt often after small changes, integration problems are found
early. If any test fails the pipeline stops, which is called **breaking the build**, and
the team is alerted at once.

**Continuous Delivery:** the code is always kept in a releasable state and is pushed
automatically up to staging, but a human clicks the button for the final production
deployment.

**Continuous Deployment:** every change that passes all the tests goes straight into
production automatically, with no manual approval at all.

> **Memory tip - the two CDs:** Delivery = a human clicks the button.
> Deployment = no human click.

---

## 3. CI/CD Pipeline Stages

A CI/CD pipeline is an automated chain of stages that takes code from a developer's
commit, through build and test, to deployment and monitoring in production.

| # | Stage | What happens | Tools |
|---|---|---|---|
| 1 | Source | Developer commits and pushes code, which triggers the pipeline. | Git, GitHub |
| 2 | Build | Code is compiled and packaged automatically. | Maven, Gradle |
| 3 | Test | Automated unit and integration tests run on the build. | JUnit, Selenium |
| 4 | Package | The build artifact is containerised. | Docker |
| 5 | Staging | Deployed to a test-like environment for further checks. | Jenkins, GitHub Actions |
| 6 | Production | The approved build goes live. | Kubernetes, ArgoCD |
| 7 | Monitor | Logs, metrics and alerts feed back into planning. | Prometheus, Grafana |

The pipeline has two halves. The **CI half** (Source, Build, Test, Package) builds and
tests the code, and the **CD half** (Staging, Production, Monitor) releases it.

> **Memory tip - SBTPSPM:** *"Smart Boys Test Packages So Production Moves"*

---

## 4. CI/CD Pipeline Diagram

```
            CONTINUOUS INTEGRATION (CI)              CONTINUOUS DELIVERY / DEPLOYMENT (CD)
 |-----------------------------------------------|  |--------------------------------------|

 +-------------+  +-------+  +------+  +---------+  +---------+  +------------+  +---------+
 | Source Code |->| Build |->| Test |->| Package |->| Staging |->| Production |->| Monitor |
 +-------------+  +-------+  +------+  +---------+  +---------+  +------------+  +---------+
        ^                                                                             |
        +--------------------------------- Feedback ----------------------------------+
```

The feedback arrow from Monitor back to Source Code is what makes it a loop. Whatever is
observed in production becomes the input for the next change.

---

## 5. Explanation of Build, Test and Deployment

**Build:** as soon as the developer pushes code, the pipeline checks out the mainline
and compiles it automatically. The source files, libraries and dependencies are put
together into one artifact. For the shopping application the catalogue, cart and payment
modules are compiled together, so the build fails immediately if one module does not fit
with another.

**Test:** automated unit tests and integration tests run on every build. Unit tests check
each function on its own and integration tests check that the modules work together. If
even one test fails the pipeline stops and alerts the team, so a bug in the discount
coupon feature is caught in minutes instead of being found by a customer.

**Deployment:** the tested build is containerised with Docker and deployed first to
staging, which looks exactly like production, and then to production using Jenkins along
with Kubernetes. Since it is the same container image in both places, the application
behaves identically, and automated rollback restores the previous version if anything
goes wrong.

---

## 6. Three Benefits of Automation

1. **Faster and more frequent releases with lower risk.** The application can be updated
   several times a day instead of once a month, and each release is small, so there is
   very little code to search through when something breaks.

2. **Early bug detection on every commit.** Every push is built and tested automatically,
   so defects are found in minutes rather than weeks, and fixing a bug early is far
   cheaper than fixing it after release.

3. **Better collaboration and faster recovery.** Dev and Ops share the same pipeline and
   the same ownership, and automated rollback with continuous monitoring restores the
   system quickly if a bad build reaches production.

---

## 7. Conclusion

The manual testing and deployment are the real cause of the delays and errors. A CI/CD
pipeline is the right DevOps practice for the company. The CI half automatically builds,
tests and packages the code on every commit and the CD half releases it to staging and
production, turning build, test and release into one automated flow that is fast,
reliable and repeatable.

---

### References

1. Unit 5 Notes
2. Sommerville, *Software Engineering*, 9th Edition - pp. 697-698, Figure 25.12
