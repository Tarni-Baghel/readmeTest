# BookingZone Admin App
BookingZone’s wants to create a premier platform for multi-entertainment facilities to manage their entertainment options and connect with their consumers.  BookingZone’s Multi-tainment Centre Management System (MCMS) shall provide convenience for vendors to manage their entertainment options and allows consumers the ability to schedule, book and pay for the services.  By connecting consumers directly with venues that have the entertainment options they are looking for and allowing them to have control over their entertainment options.  For the vendor, BookingZone’s MCMS shall allow less time managing schedules, events and payments and allows them more to focus on revenue generating activities.

## Front-End Technology
We are using react js library for creating front-end UI. Here is the list of major libraries

| S No. | Libraray | Version |
| ------ | ------ | ------ | 
| 1 | **React Js** | 16.x | 
| 2 | **Typescript** | 3.x |  
| 3 | **Redux** | 4.x |

## Project Dependency installation
- Install node js globally (node version should be >= 12.x)
  ```sh
  sudo apt install nodejs
  check node version (node -v or node –version)
  ```
- Install npm (node package manager) (node version should be >=6.x)
  ```sh
  sudo apt install npm
  check npm version (npm -v or npm –version)
  ```
- Install Git
  ```sh
  sudo apt install git-all
  check git version (git --version)
  ```
## Project Install
- Clone the repo using ssh
  ```sh
  git clone ssh://bz/v1/repos/bz-admin-app
  ```
- Clone the rep using https
  ```sh
  https://git-codecommit.us-east-1.amazonaws.com/v1/repos/bz-admin-app
   ```
- Go to project directory 
  ```sh
  cd bz-admin-app
  ```
- Run npm install command
  ```sh
   ~bz-admin-app $ npm install
   ```
- After install the project dependancy we run the project locally (port 3000)
  ```sh
  ~bz-admin-app $ npm start
   ```
Verify the development 
```sh
Navigate to [http://localhost:3000]. The app will automatically reload if you change any of the source files.
```
- For build the project
  ```sh
  ~bz-admin-app $ npm run build
  ```
How to deploy

1 Manual deployment
```sh
After successful build creation copy build folder on S3 bucket
```

OR

2 Using AWS cli
```sh
step1: Install aws cli
[https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html]

step2: AWS configure

step3: use cmd
aws s3 sync build/ s3://your-bucket-name
```

## How to update API url (Update .env file)
```sh
REACT_APP_API_DEV_URL=<api_server_url>
```

Use following credentials to login:
```sh
Admin:
Email - admin@gmail.com
Password - 1234

Business:
Email - business@gmail.com
Password - 1234
```

Login screen will look like:
![Screenshot](https://bookingzone-bucket.s3.ap-south-1.amazonaws.com/git_images/login.png)

After successful login dashboard screen will look like:
![Screenshot](https://bookingzone-bucket.s3.ap-south-1.amazonaws.com/git_images/successfullogin.png)

## Useful links
Here is the links
- [Node Js](https://nodejs.org/en/)
- [React Js](https://reactjs.org/)
- [npm](https://www.npmjs.com/)
