## 🇬🇧 Explanation in English

# 🧪 QA & Testing Tools Overview

Complete overview of the main **QA and testing tools**, their uses, differences, and recommendations.

---

## 🔹 Main Tools

| Tool          | Type                             | Main Use                             | Details and Advantages |
|---------------|---------------------------------|-------------------------------------|----------------------|
| **SonarQube** | Static Code Analysis             | Evaluate code quality, detect bugs and vulnerabilities. | Allows measuring technical debt, duplications, unit test coverage, and code complexity. Integrable with CI/CD pipelines. |
| **Jenkins**   | CI/CD and Automation             | Automate builds, tests, and deployments. | Compatible with multiple languages and tools. Supports declarative or freestyle pipelines. Widely used in DevOps. |
| **JMeter**    | Load and Performance Testing     | Simulate user load, measure performance and stability. | Ideal for stress, performance, and benchmarking tests of APIs or web applications. Supports multiple protocols: HTTP, SOAP, JDBC, etc. |
| **LoadRunner**| Performance Testing              | Evaluate capacity and scalability of critical systems. | Allows modeling complex load scenarios, measuring response times, and generating detailed reports. Compatible with web, mobile, and mainframe applications. |

---

## 🔹 Key Differences

- **SonarQube vs Jenkins:** SonarQube analyzes the code, while Jenkins executes full integration and deployment pipelines.  
- **JMeter vs LoadRunner:** Both measure performance, but JMeter is open-source and more flexible for simple tests, while LoadRunner is paid, with more support and complex scenarios.  
- **CI/CD Integration:** SonarQube and JMeter/LoadRunner can integrate with Jenkins for reporting and automation.  

---

## 🔹 Conceptual Pipeline

A basic CI/CD flow with QA is recommended:

1. **Code commit** → 2. **Build and Unit Tests (Jenkins)** → 3. **Quality Analysis (SonarQube)** → 4. **Performance Testing (JMeter/LoadRunner)** → 5. **Reporting and Deployment**

> This structure allows detecting errors and performance issues before production.

---

## 🔹 Usage Recommendations

1. **SonarQube:** Integrate into the pipeline to measure quality metrics on each commit.  
2. **Jenkins:** Automate build, test, and deployment to minimize manual errors.  
3. **JMeter:** Run periodic load tests to identify bottlenecks.  
4. **LoadRunner:** Use for high-impact critical tests and realistic traffic simulations.  

---

## 🔹 References

- [SonarQube](https://www.sonarqube.org/)  
- [Jenkins](https://www.jenkins.io/)  
- [JMeter](https://jmeter.apache.org/)  
- [LoadRunner](https://docs.microfocus.com/doc/123/9.60/configrunloadtest)  

---

## 🔹 Contributions

PRs are welcome to add new tools or improve descriptions.

---

## 🔹 License

MIT License © 2025