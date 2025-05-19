🧪 JMeter Project - REST API Load Testing

This repository contains JMeter test plans for conducting performance and load testing on REST APIs. It allows you to simulate users, run various HTTP scenarios (GET, POST, etc.), and analyze results through detailed reports.

📁 Project Structure

├── plans/

|   ├── Test Plan httpbin.org.jmx

│   └── Test Plan reqres.in.jmx

├── datasets/

|   ├── auth_dataset.csv

│   └── create_user_dataset.csv

├── logs/

│   └── TestPlanHttpbinErrorLogs.xml # Errors only

├── results/

│   └── results.jtl

├── README.md

└── .gitignore

🚀 Features

Multi-user load simulation (Thread Group)

Custom HTTP requests (GET, POST)

CSV-based data input

Response assertions

Detailed results via HTML reports

🛠 Prerequisites

Apache JMeter (version 5.6.3 or higher)

Java 8 or newer

🧭 Quick Start

1. Clone the repository

git clone https://github.com/Paxman-developer/JMeter.git
cd jmeter

2. Launch JMeter GUI

jmeter

3. Open a test plan

Go to the plans/ folder

Open a .jmx file

Click Start to execute the test

🧑‍💻 Run via Command Line

jmeter -n -t plans/firstPlan.jmx -l results/results.jtl -e -o results/html-report

-n = non-GUI mode

-t = JMX test plan to run

-l = results log file

-e -o = generate HTML report

📊 Viewing Reports

Open results/html-report/index.html in your browser to view detailed performance statistics.
