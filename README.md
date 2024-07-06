Setup Steps

### Project Structure and Setup

```
vip-crud-app/
│
├── data/
│   └── guests.json
│
├── src/
│   ├── controllers/
│   │   └── guestController.js
│   ├── helpers/
│   │   └── fileHelper.js
│   └── index.js
│
├── .gitignore
├── package.json
└── README.md

```
### Setup Steps

1. **Project Initialization:**
   - Initialize a Node.js project with `npm init -y`.
   - Create necessary directories and files:

     ```
     mkdir vip-crud-app
     cd vip-crud-app
     touch .gitignore index.js README.md
     npm install nanoid@4
     ```

     ```sh
     mkdir src
     mkdir src/controllers
     touch src/controllers/guestController.js
     mkdir src/helpers
     touch src/helpers/fileHelper.js
     touch src/index.js

     mkdir data
     touch data/guests.json
     ```

   - Setup `package.json` with appropriate scripts:
     ```json
     "scripts": {
       "index": "node src/index.js index",
       "create": "node src/index.js create",
       "show": "node src/index.js show",
       "update": "node src/index.js update",
       "destroy": "node src/index.js destroy",
       "vip": "node src/index.js vip"
     }
     ```

    - Setup `.gitignore` with appropriate details:
     ```
     # Node.js dependencies
     /node_modules
     .DS_STORE
     
     #Log files
     npm-debug.log*
     yarn-debug.log*
     yarn-error.log*
     
     # Environment variables
     .env
    
    # Data files
    /data/guests.json

     ```


   - Setup `.env` file with appropriate details:
     ```sh
     npm install dotenv
     touch .env

     # Example .env file
     # This is where you can put your environment variables
     # e.g., DATABASE_URL, API_KEY, etc.
     # For now, let's leave it empty
     ```



     ```

2. **File Contents and Directories/Dependencies:**

   - **index.js:** Main entry point handling CLI commands.
   - **helpers.js:** Utility functions for reading and writing JSON files.
   - **guestController.js:** Functions for CRUD operations for guests
   - **guests.json:** Stores the guest list.
   - **.gitignore:** Specifies files and directories to be ignored by Git.
   - **package.json:** Manages project dependencies and scripts.
   **README.md:** Describes the project and provides instructions.




