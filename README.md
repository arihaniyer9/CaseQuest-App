# CaseQuest App

## Description
**CaseQuest App** is a scalable challenge platform designed to support over 100 students, built using the MERN stack. The app facilitates a collaborative challenge experience with interactive features such as polls, quizzes, forms, a virtual post-it wall, and a leaderboard system. 

### Key Features:
- **Admin Role**:
  - Manage participants and allocate/deallocate points.
  - Create and manage:
    - Polls
    - Quizzes
    - Forms
    - Voting mechanisms
    - Virtual post-it wall (participants can add posts to it publicly).
  - View graphical statistics for forms, polls, and quizzes.
  - Randomize teams (2 online + 2 offline students) with no repeats.
- **Participant Role**:
  - Interact with polls, quizzes, and forms.
  - Add content to the virtual post-it wall.
  - View their ranking on the leaderboard.

The platform is deployed on AWS EC2 with load balancing to handle high traffic efficiently.

---

## Tech Stack
- **Frontend**: ReactJS
- **Backend**: NodeJS, ExpressJS
- **Database**: MongoDB
- **Deployment**: AWS EC2 with Load Balancing

---

## Installation and Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/CaseQuest-App.git
   ```
2. Navigate to the project directory:
   ```bash
   cd CaseQuest-App
   ```
3. Install dependencies:
   - For the frontend:
     ```bash
     cd frontend
     npm install
     ```
   - For the backend:
     ```bash
     cd ../backend
     npm install
     ```
4. Set up environment variables:
   - In the `backend` folder, create a `.env` file with the following variables:
     ```plaintext
     MONGO_URI=your_mongodb_connection_string
     AWS_ACCESS_KEY_ID=your_aws_access_key
     AWS_SECRET_ACCESS_KEY=your_aws_secret_key
     PORT=5000
     ```
5. Start the development environment:
   - Backend:
     ```bash
     cd backend
     npm start
     ```
   - Frontend:
     ```bash
     cd ../frontend
     npm start
     ```
6. Deploy the app on AWS EC2:
   - Launch an EC2 instance with a load balancer.
   - Configure security groups and scaling policies for high availability.
   - Push the project to the instance and set up NodeJS, MongoDB, and NGINX.

---

## Screenshots

![Home Page](/CaseQuestApp-ss/main-page.png)
![Home Page](/CaseQuestApp-ss/main-page-2.png)
*Landing Page for all users*

![User Dashboard](/CaseQuestApp-ss/main-dashboard.png)
*User dashboard for participating in the Challenge*

![Admin Dashboard](/CaseQuestApp-ss/main-admin-page.png)
*Admin dashboard for managing users and features*

![Virtual Post-it Wall](/CaseQuestApp-ss/main-postwall-page.png)
*Interactive virtual post-it wall for participants*

![Leaderboard](/CaseQuestApp-ss/main-leaderboard.png)
*Leaderboard displaying participant rankings*

