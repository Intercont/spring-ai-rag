# Spring AI RAG

## Project Goals

This project aims to build an application using Retrieval-Augmented Generation (RAG) patterns in the Spring ecosystem. It leverages the latest features from Spring AI to integrate large language models (LLMs) with vector stores and document readers, supporting advanced AI-powered applications such as intelligent search, summarization, or AI assistants.

## Technologies Used

The project is built with the following core technologies:

- **Java 21**
- **Spring Boot 3.5.0**
- **Spring AI 1.0.0** (via BOM)
  - `spring-ai-starter-model-openai`
  - `spring-ai-vector-store`
  - `spring-ai-tika-document-reader`
- **Lombok** (for boilerplate code reduction)
- **Spring Boot Devtools** (for development convenience)
- **Spring Boot Starter Web** (for web APIs)
- **Spring Boot Starter Test** (for testing)

All dependencies and their versions are managed via the [`pom.xml`](pom.xml).

## Getting Started

### Prerequisites

- **Java 21** or newer
- **Maven 3.8+**

### Running Locally

1. **Clone the Repository**

   ```bash
   git clone https://github.com/Intercont/spring-ai-rag.git
   cd spring-ai-rag
   ```

2. **Configure your OpenAI API Key**
    - Create or edit the file `src/main/resources/application.yml` and add:
      ```
      spring:
        ai:
          openai:
            api-key:YOUR_OPENAI_API_KEY
      ```
    - It is recommended to set the API key as an environment variable instead of having it on your properties file:
      ```bash
      export OPENAI_API_KEY=YOUR_OPENAI_API_KEY
      ```

3. **Build the Project**

   ```bash
   mvn clean install
   ```

4. **Run the Application on cmd or on your local IDE**

   ```bash
   mvn spring-boot:run
   ```

   The application will start on the default port (usually `8080`).

### Running Tests

```bash
mvn test
```

## Project Structure

- `src/main/java` — Application source code
- `src/test/java` — Test code
- `pom.xml` — Maven build file

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

## License

This project is licensed under standard open source terms. See [`pom.xml`](pom.xml) for details.

---
*Built with [Spring Boot](https://spring.io/projects/spring-boot) and [Spring AI](https://github.com/spring-projects/spring-ai).*
**Subscribe at [igorfragadev.com](igorfragadev.com) for more**
