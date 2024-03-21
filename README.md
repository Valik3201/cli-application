# Contacts Management Node.js Project

This project provides a simple command-line interface (CLI) for managing contacts stored in a JSON file. It allows users to list contacts, add new contacts, retrieve a specific contact by ID, and remove contacts.

## Features

- List all contacts
- Add a new contact
- Retrieve a contact by ID
- Remove a contact by ID

## Installation

1. Clone the repository:

```bash
git clone https://github.com/valik3201/contacts-node-project.git
```

2. Navigate into the project directory:

```bash
cd contacts-node-project
```

3. Install dependencies:

```bash
npm install
```

## Usage

The CLI supports the following actions:

- **List Contacts**: View all contacts.

```bash
node index.js --action list
```

- **Add Contact**: Add a new contact. Specify name, email, and phone.

```bash
node index.js --action add --name "John Doe" --email "john@example.com" --phone "123-456-7890"
```

- **Get Contact by ID**: Retrieve a contact by providing its ID.

```bash
node index.js --action get --id "contact_id_here"
```

- **Remove Contact by ID**: Remove a contact by providing its ID.

```bash
node index.js --action remove --id "contact_id_here"
```

## Development

During development, you can use nodemon to automatically restart the application when changes are detected:

```bash
npm run start:dev
```

This command will start the application with nodemon, enabling hot reloading for faster development.

## File Structure

- `contacts.js`: Contains functions for managing contacts (list, get by ID, add, remove).
- `index.js`: Entry point for the CLI application.
- `db/contacts.json`: JSON file to store contacts.

## Dependencies

- `fs/promises`: For file system operations with promises.
- `path`: For handling file paths.
- `uuid`: For generating unique IDs for contacts.
- `commander`: For building command-line interfaces.

## Dev Dependencies

- `nodemon`: For automatic restarting of the application during development.

## Contributing

Contributions are welcome! Please feel free to open an issue or submit a pull request.
