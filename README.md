<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Linux Server with PuTTY | AWS EC2</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, Helvetica, sans-serif;
        }

        body {
            background: #0d1117;
            color: #e6edf3;
            line-height: 1.7;
        }

        .container {
            width: 90%;
            max-width: 1100px;
            margin: auto;
        }

        .hero {
            text-align: center;
            padding: 70px 20px;
            border-bottom: 1px solid #30363d;
        }

        .hero h1 {
            font-size: 42px;
            margin-bottom: 15px;
        }

        .hero h1 span {
            color: #58a6ff;
        }

        .hero p {
            color: #8b949e;
            font-size: 18px;
        }

        .badges {
            margin-top: 25px;
        }

        .badge {
            display: inline-block;
            padding: 6px 14px;
            margin: 5px;
            border: 1px solid #30363d;
            border-radius: 20px;
            color: #58a6ff;
            font-size: 13px;
        }

        section {
            padding: 45px 0;
            border-bottom: 1px solid #21262d;
        }

        h2 {
            color: #58a6ff;
            margin-bottom: 20px;
            font-size: 28px;
        }

        h3 {
            margin-bottom: 10px;
        }

        .card-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 20px;
        }

        .card {
            background: #161b22;
            border: 1px solid #30363d;
            border-radius: 12px;
            padding: 25px;
            transition: 0.3s;
        }

        .card:hover {
            transform: translateY(-5px);
            border-color: #58a6ff;
        }

        .card p {
            color: #8b949e;
        }

        ul {
            padding-left: 25px;
        }

        li {
            margin: 8px 0;
        }

        .workflow {
            display: flex;
            align-items: center;
            justify-content: center;
            flex-wrap: wrap;
            gap: 15px;
            margin-top: 25px;
        }

        .flow-box {
            background: #161b22;
            border: 1px solid #58a6ff;
            border-radius: 10px;
            padding: 18px 25px;
            text-align: center;
            min-width: 150px;
        }

        .arrow {
            color: #58a6ff;
            font-size: 25px;
        }

        pre {
            background: #010409;
            border: 1px solid #30363d;
            border-radius: 10px;
            padding: 20px;
            overflow-x: auto;
            color: #79c0ff;
        }

        .outcome {
            background: #161b22;
            border-left: 4px solid #58a6ff;
            padding: 25px;
            border-radius: 8px;
        }

        footer {
            text-align: center;
            padding: 35px 10px;
            color: #8b949e;
        }

        footer strong {
            color: #e6edf3;
        }
    </style>
</head>

<body>

    <!-- HERO -->
    <header class="hero">
        <div class="container">

            <h1>🐧 Linux Server with <span>PuTTY</span></h1>

            <p>
                AWS EC2 Linux Server Administration & Remote SSH Access
            </p>

            <div class="badges">
                <span class="badge">AWS EC2</span>
                <span class="badge">Linux</span>
                <span class="badge">PuTTY</span>
                <span class="badge">SSH</span>
                <span class="badge">Cloud Computing</span>
            </div>

        </div>
    </header>


    <main class="container">

        <!-- PROJECT OVERVIEW -->
        <section>

            <h2>📌 Project Overview</h2>

            <p>
                This project demonstrates the deployment and administration
                of a Linux server using Amazon EC2 and remote connectivity
                through PuTTY. The project focuses on practical Linux
                administration, SSH connectivity, security configuration,
                file management, users, permissions, processes and networking.
            </p>

        </section>


        <!-- ARCHITECTURE -->
        <section>

            <h2>☁️ Architecture & Workflow</h2>

            <div class="workflow">

                <div class="flow-box">
                    💻<br>
                    <strong>Windows PC</strong>
                </div>

                <div class="arrow">→</div>

                <div class="flow-box">
                    🔐<br>
                    <strong>PuTTY</strong>
                </div>

                <div class="arrow">→</div>

                <div class="flow-box">
                    🌐<br>
                    <strong>Internet</strong>
                </div>

                <div class="arrow">→</div>

                <div class="flow-box">
                    ☁️<br>
                    <strong>AWS EC2</strong>
                </div>

                <div class="arrow">→</div>

                <div class="flow-box">
                    🐧<br>
                    <strong>Linux Server</strong>
                </div>

            </div>

        </section>


        <!-- TECHNOLOGIES -->
        <section>

            <h2>🛠️ Technologies Used</h2>

            <div class="card-grid">

                <div class="card">
                    <h3>☁️ Amazon EC2</h3>
                    <p>
                        Used to deploy and run the Linux cloud server.
                    </p>
                </div>

                <div class="card">
                    <h3>🐧 Linux</h3>
                    <p>
                        Used for server administration and command-line operations.
                    </p>
                </div>

                <div class="card">
                    <h3>🔐 PuTTY</h3>
                    <p>
                        Used to establish a remote SSH connection with EC2.
                    </p>
                </div>

                <div class="card">
                    <h3>🛡️ Security Group</h3>
                    <p>
                        Used to control inbound and outbound network traffic.
                    </p>
                </div>

            </div>

        </section>


        <!-- IMPLEMENTATION -->
        <section>

            <h2>⚙️ Implementation</h2>

            <div class="card-grid">

                <div class="card">
                    <h3>01. Launch EC2</h3>
                    <p>
                        Created and configured a Linux EC2 instance.
                    </p>
                </div>

                <div class="card">
                    <h3>02. Configure Security</h3>
                    <p>
                        Configured the Security Group for SSH access.
                    </p>
                </div>

                <div class="card">
                    <h3>03. Configure PuTTY</h3>
                    <p>
                        Converted the key pair into PPK format and configured PuTTY.
                    </p>
                </div>

                <div class="card">
                    <h3>04. SSH Connection</h3>
                    <p>
                        Connected remotely to the Linux EC2 server.
                    </p>
                </div>

            </div>

        </section>


        <!-- COMMANDS -->
        <section>

            <h2>⌨️ Linux Commands Practiced</h2>

            <pre>
# File & Directory Management
pwd
ls
cd
mkdir
touch
cp
mv
rm

# File Operations
cat
vi
less
head
tail

# Permissions
chmod
chown

# Process Management
ps
top
kill

# System Monitoring
df -h
free -m
uptime

# Service Management
systemctl

# Administrative Access
sudo
            </pre>

        </section>


        <!-- SECURITY -->
        <section>

            <h2>🔒 Security Configuration</h2>

            <ul>
                <li>Configured AWS Security Group for SSH access.</li>
                <li>Used key-based authentication.</li>
                <li>Connected securely using SSH through PuTTY.</li>
                <li>Used sudo for administrative operations.</li>
                <li>Allowed only required network ports.</li>
            </ul>

        </section>


        <!-- LEARNING -->
        <section>

            <h2>🎯 Key Learning Outcomes</h2>

            <div class="card-grid">

                <div class="card">
                    <h3>Linux Administration</h3>
                    <p>
                        Learned essential Linux commands and server management.
                    </p>
                </div>

                <div class="card">
                    <h3>AWS EC2</h3>
                    <p>
                        Gained practical experience launching and managing EC2 instances.
                    </p>
                </div>

                <div class="card">
                    <h3>SSH</h3>
                    <p>
                        Learned secure remote access to cloud servers.
                    </p>
                </div>

                <div class="card">
                    <h3>Networking</h3>
                    <p>
                        Understood Security Groups, ports and basic connectivity.
                    </p>
                </div>

            </div>

        </section>


        <!-- OUTCOME -->
        <section>

            <h2>🚀 Project Outcome</h2>

            <div class="outcome">

                <p>
                    Successfully deployed a Linux server on AWS EC2 and
                    established secure remote access using PuTTY and SSH.
                    This project provided hands-on experience with cloud
                    infrastructure, Linux administration, networking and
                    AWS security configuration.
                </p>

            </div>

        </section>


        <!-- AUTHOR -->
        <section>

            <h2>👨‍💻 Author</h2>

            <div class="card">

                <h3>Darshan Patil</h3>

                <p>
                    B.Sc. Computer Science Graduate |
                    AWS & DevOps Learner
                </p>

                <br>

                <p>
                    Focus Areas:
                    AWS • Linux • DevOps • Docker • Git • CI/CD
                </p>

            </div>

        </section>

    </main>


    <footer>

        <p>
            ⭐ <strong>Linux-With-PuTTY</strong> |
            AWS EC2 | Linux | SSH | PuTTY
        </p>

        <p>
            Built for learning and practical cloud experience.
        </p>

    </footer>

</body>
</html>
