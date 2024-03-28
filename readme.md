<h1>Member Management Server</h1>

<p>This Node.js application serves as a RESTful API for managing member data and balances. It allows users to perform various operations such as adding new members, searching for members, updating member information, collecting money from members, and retrieving total balance information.</p>

<h2>Getting Started</h2>

<ol>
  <li>Clone the repository:</li>
  <pre><code>git clone &lt;repository_url&gt;</code></pre>

  <li>Navigate to the project directory:</li>
  <pre><code>cd member-management-server</code></pre>

  <li>Install dependencies:</li>
  <pre><code>npm install</code></pre>

  <li>Start the server:</li>
  <pre><code>npm start</code></pre>
  <p>The server will start running on port 3000 by default.</p>
</ol>

<h2>API Endpoints</h2>

<p>The following endpoints are available:</p>

<ul>
  <li><code>GET /members/add</code>: Add a new member.</li>
  <li><code>GET /members/search</code>: Search for members by name.</li>
  <li><code>GET /members/:serialNumber</code>: Retrieve a specific member's information by serial number.</li>
  <li><code>GET /collectmoney</code>: Collect money from a member.</li>
  <li><code>GET /member/all</code>: Retrieve information for all members.</li>
  <li><code>GET /members/balance/:serialNumber</code>: Retrieve a member's balance by serial number.</li>
  <li><code>GET /member/new</code>: Add a new member with private key validation.</li>
  <li><code>GET /member/remove</code>: Remove a member.</li>
  <li><code>GET /members/update/name/:serialNumber</code>: Update a member's name by serial number.</li>
  <li><code>GET /member/totalbalance</code>: Retrieve the total balance of all members.</li>
</ul>

<h2>Usage</h2>

<h3>Adding a New Member</h3>

<p>To add a new member, make a GET request to <code>/members/add</code> with the following query parameters:</p>

<ul>
  <li><strong>name</strong>: Name of the member.</li>
  <li><strong>mobileNumber</strong>: Mobile number of the member.</li>
  <li><strong>nidNumber</strong>: National ID number of the member.</li>
</ul>

<p>Example:</p>

<pre><code>curl -X GET 'http://localhost:3000/members/add?name=Xanvir&amp;mobileNumber=1234567890&amp;nidNumber=ABCD1234'</code></pre>

<!-- Other endpoint usage examples -->

<h2>License</h2>

<p>This project is licensed under the MIT License - see the <a href="LICENSE">LICENSE</a> file for details.</p>
