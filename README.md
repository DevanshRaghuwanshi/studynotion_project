<h1>StudyNotion</h1>

<h2>Project Description</h2>
<p>
  StudyNotion is a full-featured ed-tech platform built using the MERN stack. It allows students to learn, purchase, and rate courses, and instructors to create, manage, and track content. It includes authentication, course management, payment, and media handling.
</p>

<h2>Technology Used</h2>
<h3>Frontend</h3>
<ul>
  <li>HTML, CSS, JavaScript</li>
  <li>React.js</li>
  <li>Tailwind CSS</li>
  <li>Redux</li>
</ul>

<h3>Backend</h3>
<ul>
  <li>Node.js</li>
  <li>Express.js</li>
  <li>MongoDB</li>
  <li>Mongoose</li>
  <li>JWT, Bcrypt</li>
</ul>

<h2>Data Models</h2>
<ul>
  <li><strong>Student:</strong> name, email, password, enrolled courses</li>
  <li><strong>Instructor:</strong> name, email, password, created courses</li>
  <li><strong>Course:</strong> title, description, instructor, content, media, ratings</li>
</ul>

<h2>API Endpoints</h2>
<pre>
POST   /api/auth/signup        - Register new user
POST   /api/auth/login         - Login and return token
POST   /api/auth/verify-otp    - Verify email OTP
POST   /api/auth/forgot-password - Password reset link

GET    /api/courses            - List all courses
GET    /api/courses/:id        - Course by ID
POST   /api/courses            - Create new course
PUT    /api/courses/:id        - Update course
DELETE /api/courses/:id        - Delete course
POST   /api/courses/:id/rate   - Rate course
</pre>

<h2>How to Install</h2>
<ol>
  <li>Clone the repo:<br/>
    <code>git clone https://github.com/DevanshRaghuwanshi/studynotion_project.git/</code>
  </li>
  <li>Navigate to the directory:<br/>
    <code>cd StudyNotion</code>
  </li>
  <li>Install dependencies:<br/>
    <code>npm install</code>
  </li>
  <li>Setup environment variables in <code>/server/.env</code> (See below)</li>
  <li>Run the project:
    <ul>
      <li><code>npm run dev</code> for development</li>
    </ul>
  </li>
</ol>

<h2>Environment Variables</h2>
<p>Create a <code>.env</code> file inside your <code>/server</code> folder and add the following:</p>
<pre>
PORT=5000
MONGODB_URL=mongodb+srv://&lt;username&gt;:&lt;password&gt;@&lt;cluster-url&gt;/studynotion?retryWrites=true&w=majority

JWT_SECRET=your_jwt_secret
JWT_EXPIRY=2d

CLOUDINARY_CLOUD_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret

MAIL_HOST=smtp.mailtrap.io
MAIL_PORT=2525
MAIL_USER=your_mail_user
MAIL_PASS=your_mail_pass

FRONTEND_URL=http://localhost:3000
</pre>

<h2>Screenshots</h2>
<div class="screenshots">
  <img src="images/screenshot1.png" alt="Login page">
  <img src="images/screenshot2.png" alt="home page">
  <img src="images/screenshot3.png" alt="Instructor Course">
</div>

</body>
</html>
