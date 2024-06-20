# Universal Data Bridge

**Universal Data Bridge** is a comprehensive data integration and management platform designed to streamline and unify data flows within the logistics industry. The platform provides a centralized hub for handling customer information, shipping details, return processes, carrier contacts, and communication methods, enabling seamless data exchange and real-time visibility across various stakeholders such as customers, shippers, merchants, payors, brokers, and carriers.

## Key Features

- **Customer Information Management**: Store and manage detailed customer information, including addresses, contact methods, and preferences.
- **Shipping and Return Management**: Efficiently handle shipping details, track shipments in real-time, and manage return processes.
- **Unified Contact Information**: Support multiple communication methods including phone, SMS, email, video chat, and social media handles, ensuring comprehensive and flexible contact management.
- **Broker Management**: Manage broker details with the same comprehensive contact and address information as other stakeholders, facilitating better coordination and communication.
- **Carrier Contacts Management**: Store and manage detailed carrier contact information, including customer service and technical support details, to facilitate quick and effective communication.
- **Scalability and Performance**: Built using Go, a high-performance, compiled language designed for efficient concurrency, ensuring the platform can handle high volumes of data and numerous simultaneous operations with ease.
- **Modular and Extensible Architecture**: Designed with a modular structure, allowing for easy extension and customization to meet specific business needs and integrate with existing systems.
- **Robust API Support**: Provides RESTful APIs for seamless integration with external systems, enabling automation and interoperability with various logistics and e-commerce platforms.
- **Real-Time Data Synchronization**: Ensures that all integrated systems have access to the most up-to-date information, reducing errors and improving decision-making capabilities.
- **Enhanced Communication Capabilities**: Facilitates efficient and effective communication between different stakeholders through various supported methods, enhancing customer service and operational coordination.

## Project Structure

The project is organized into several directories, each serving a specific purpose within the platform:

- **controllers/**: Contains the logic for handling API requests and responses, managing different entities like customers, products, returns, shipping, brokers, and carriers.
  - `customer_controller.go`: Manages customer-related operations.
  - `product_controller.go`: Manages product-related operations.
  - `return_controller.go`: Manages return-related operations.
  - `shipping_controller.go`: Manages shipping-related operations.
  - `broker_controller.go`: Manages broker-related operations.
  - `carrier_controller.go`: Manages carrier-related operations.
- **models/**: Defines the data structures and models used within the platform.
  - `contact.go`: Defines the `ContactInfo` structure for various communication methods.
  - `customer.go`: Defines the `Customer` structure and associated data operations.
  - `product.go`: Defines the `Product` structure and associated data operations.
  - `return.go`: Defines the `Return` structure and associated data operations.
  - `shipping.go`: Defines the `Shipping` structure and associated data operations.
  - `broker.go`: Defines the `Broker` structure and associated data operations.
  - `carrier.go`: Defines the `Carrier` structure and associated data operations.
- **routers/**: Sets up the routing and API endpoints.
  - `router.go`: Initializes and manages the API routes for the application.
- **utils/**: Contains utility functions and common code used across the platform.
  - `response.go`: Provides utilities for formatting and sending API responses.
- **main.go**: The entry point of the application, initializing the server and setting up routes.
- **go.mod**: The Go module file, managing dependencies for the project.
- **.gitignore**: Specifies files and directories to be ignored by Git, such as build artifacts and temporary files.

## Getting Started

### Prerequisites

- [Go](https://golang.org/dl/)
- [Git](https://git-scm.com/downloads)

### Installation

1. **Clone the Repository**:
   ```sh
   git clone https://github.com/yourusername/universal-data-bridge.git
   cd universal-data-bridge
