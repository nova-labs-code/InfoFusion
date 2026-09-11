# InfoFusion

InfoFusion is a web-based information assistant designed to understand natural-language questions, determine what information is needed, retrieve it from appropriate public APIs, and present the results in a simple interface.

## Features

- Natural-language question understanding
- Automatic intent detection
- Entity and location detection
- Source selection based on the question
- Weather information
- Book searches
- Wikipedia information
- Wikidata entity lookup
- Dictionary definitions
- TV show information
- Pokémon information
- SpaceX information
- Currency conversion
- Holiday information
- Jokes
- Trivia
- GitHub information
- D&D information
- Food information
- General web-search fallback
- Advanced mathematical calculations

## How It Works

InfoFusion does not simply match a question to one fixed command.

A question is first analyzed to create a request brief containing information such as:

- Intent
- Entity
- Location
- Variable
- Mathematical operation
- Required information
- Source confidence scores

The source selector then determines which APIs are most appropriate for the request.

The selected sources are queried and their results are combined into the final response.

### Basic Flow

```text
User Question
      ↓
Request Understanding
      ↓
Request Brief
      ↓
Source Selection
      ↓
API Requests
      ↓
Result Processing
      ↓
Final Answer