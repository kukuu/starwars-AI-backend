# Starwars AI Backend

This full-stack application leverages a modern technology stack with NestJS and Next.js at its core. The backend is built with Node.js, NestJS framework, and TypeScript, utilizing Prisma ORM with SQLite for database management. The AI capabilities are powered by OpenAI's GPT models through LangChain, with fallback to traditional database queries when API keys are unavailable. The frontend employs Next.js 15 with React, TypeScript, and Tailwind CSS, providing a responsive user interface for character exploration and AI-powered search functionality.

The application's architecture is organized around several key services referenced in the AppModule. The DatabaseService manages all Prisma operations and SQLite connections, while CharactersService handles CRUD operations for Star Wars character data. The LikesService manages user engagement through character liking functionality, and UsersService coordinates user-related operations. Most notably, the OpenAIService processes natural language queries, attempting AI-powered responses first before falling back to traditional database searches using the other services.

The handshake between frontend and backend occurs through RESTful API endpoints defined in the AppController. When users submit queries through the Next.js search interface, requests are routed to the NestJS backend's /search endpoint, which delegates to the OpenAIService. This service intelligently processes prompts - either leveraging OpenAI's LLM for complex queries or using the CharactersService for structured database searches. The backend services collaborate through dependency injection, with the OpenAIService utilizing DatabaseService for data access and returning formatted responses that the frontend displays in an intuitive, styled interface using Tailwind CSS components. 

## Project Structure

https://github.com/kukuu/starwars-AI-backend/blob/main/project-structure.md

## Architecture

https://github.com/kukuu/starwars-AI-backend/blob/main/architecture.md

# Service Flow


https://github.com/kukuu/starwars-AI-backend/blob/main/service-flow.md

## Repository

https://github.com/kukuu/Node-NestJS-TypeScript-PrismaORM-OpenAI-LLM (**PRIVATE**)
