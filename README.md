# Asst Telegram Bot

Asst is a personal assistant bot on the telegram platform designed to provide specialized assistance tailored to the user. It connects to your own APIs and leverages OpenAI's natural language processing capabilities. This project is built using the Spring framework and integrates with the Telegram Bot API. The bot can be containerized using Docker and deployed on AWS Lambda for serverless execution.

## Features

- Personalized assistance: Asst provides personalized recommendations and assistance based on the user's preferences and needs.
- API integration: Asst connects to your custom APIs to fetch data and perform specialized tasks.
- OpenAI's integration: Asst leverages OpenAI's powerful natural language processing capabilities for enhanced functionality.
- Telegram Bot: The bot interacts with users through the Telegram messaging platform, providing a seamless user experience.
- Spring framework: The project is built using Spring Boot, making it easy to configure and extend.
- Docker: The bot can be containerized using Docker for easy deployment and scalability.
- AWS Lambda: The bot can be deployed on AWS Lambda for serverless execution, reducing operational overhead.

## Prerequisites

Before running Asst Telegram Bot, ensure you have the following prerequisites:

- Java Development Kit (JDK) 17 or higher
- Maven
- Docker
- AWS CLI
- Telegram account and API token
- OpenAI API key

## Installation

Follow these steps to install and set up Asst Telegram Bot:

1. Clone the repository: `git clone https://github.com/Banji-07/Asst.git`
2. Navigate to the project directory: `cd Asst`
3. Build the project using Maven: `mvn clean install`

## Configuration

To configure Asst Telegram Bot, follow these steps:

1. Create a new bot on Telegram by following the instructions at [https://core.telegram.org/bots#3-how-do-i-create-a-bot](https://core.telegram.org/bots#3-how-do-i-create-a-bot). Note down the API token provided.
2. Obtain an OpenAI API key by signing up for an account at [https://www.openai.com/](https://www.openai.com/).
3. Modify the `application.properties` file and set the following properties:
    - `telegram.bot.token`: Your Telegram bot API token.
    - `openai.api.key`: Your OpenAI API key.

## Dockerization

To containerize Asst Telegram Bot using Docker, follow these steps:

1. Build the Docker image: `docker build -t asst-telegram-bot .`
2. Run the Docker container: `docker run -d asst-telegram-bot`

## Deployment on AWS Lambda

To deploy Asst Telegram Bot on AWS Lambda, follow these steps:

1. Set up an AWS Lambda function and ensure it is configured to handle Java applications.
2. Build the project using Maven: `mvn clean package -DskipTests`
3. Deploy the built JAR file to AWS Lambda.
4. Configure the necessary environment variables in the Lambda function, including the `telegram.bot.token` and `openai.api.key` properties.
5. Set up the appropriate triggers and permissions for the Lambda function.

## Usage

To start using Asst Telegram Bot, follow these steps:

1. Run the application: `mvn spring-boot:run` (for local development)
2. Open Telegram and search for your bot by the username you provided during bot creation.
3. Start a conversation with your bot and interact with it using commands or messages, depending on your bot's functionality.

## API Integration

To integrate your own APIs with Asst Telegram Bot, follow these steps:

1. Create your custom APIs to provide the required functionality.
2. Modify the bot's implementation (`BotService` class) to include API calls and process the responses accordingly.

## Contributing

Contributions to Asst Telegram Bot are welcome! If you have any ideas, improvements, or bug fixes, please submit a pull request or open an issue in the GitHub repository.

## License

This project is licensed under the [MIT License].

## Acknowledgments

- The Asst Telegram Bot project leverages the Telegram Bot API and OpenAI's powerful natural language processing capabilities. Thank you to the respective teams for providing such valuable tools and platforms.

Feel free to customize this README.md file according to your project's specific details and requirements. Good luck with your Telegram bot project!