# Skytrion Tech

The company website for **Skytrion Tech**, a studio that designs and builds digital products: websites, custom software, mobile apps and point of sale (POS) systems.

## Pages

| Page | File | What it covers |
|------|------|----------------|
| Home | `index.html` | Hero, an overview of the four core services, and a call to action |
| About Us | `about.html` | Who we are and what makes us different |
| Services | `services.html` | Each service in detail, POS features and our process |
| Projects | `projects.html` | Portfolio of past client work |
| Contact | `contact.html` | Contact details and a message form |

All pages are in `src/main/webapp/`.

## Tech stack

- HTML and CSS for the site itself
- Java 11 with Jakarta EE (Servlet 5.0, JAX-RS 3.0, CDI 3.0)
- Maven, packaged as a `.war` file

## Getting started

### Prerequisites

- JDK 11 or newer
- A Jakarta EE 9+ server such as Apache Tomcat 10, GlassFish 6 or Payara 6

Maven itself is optional, because the project includes the Maven Wrapper (`mvnw`).

### Build

```bash
# macOS / Linux
./mvnw clean package

# Windows
mvnw.cmd clean package
```

This creates `target/Skytrion-1.0-SNAPSHOT.war`.

### Run

Deploy the `.war` file to your server. With Tomcat 10, for example, copy it into the `webapps/` folder, start Tomcat, then open:

```
http://localhost:8080/Skytrion-1.0-SNAPSHOT/
```

The pages are plain HTML, so you can also preview them by opening `src/main/webapp/index.html` directly in a browser.

## Project structure

```
Skytrion/
├── pom.xml
├── mvnw, mvnw.cmd
└── src/main/
    ├── resources/META-INF/beans.xml
    └── webapp/
        ├── index.html
        ├── about.html
        ├── services.html
        ├── projects.html
        └── contact.html
```

## Author

**Anthony Francis** ([@AnthonyFrancisSharu](https://github.com/AnthonyFrancisSharu))
