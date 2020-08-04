![logo](./media/Square-Logo.png)

# Dependable

A hackathon project that attempts to model inter-team dependencies transparently and beautifully

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Screenshot

![screen4](./media/screenshot4.png)

![screen3](./media/screenshot3.png)

![screen2](./media/improveGantt.png)

![screen1](./media/screenshot1.png)




## Installation

```
git clone <clone url>

cd bff
yarn

cd ..
yarn
```
Dependable requires your JIRA username:password for basic authentication.

Create and setup the .env file for the BFF

```
echo "API_JIRA_HOST=https://jira-uat.company.com
API_USERNAME=$(whoami)
API_SECRET=" > bff/.env
```

Then open `bff/.env` and input your password

The host can be changed to a Production or other JIRA instance by modifying the API_JIRA_HOST domain.

## Usage

Use two terminals to start the UI and BFF

```
cd bff
yarn start
```

```
yarn start
```

Your browser should open to http://localhost:3000

## UI explanation

### Project View

Enter your JIRA project code or Project ID and click create to display all outstanding features, displayed in a graphical form with links to all dependent tickets and their scheduled dates. The timeline at the bottom of the chart displays the earliest possible date the tickets can start based on their dependencies and planned sprints.

### Unscheduled Features

Shows a table of tickets and dependencies there were unable to be incided in the project view as they are unscheduled. The primary use of this is to help facilitate conversations between delivery teams about scheduling in dependent features.

### Contributors

- **Joseph Garner**
- **Jo Peyper**
- **Maysam Tayyeb**
- **Stanley Huang**
