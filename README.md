name: hello-world

on: push
    branches:
      - main

jobs:
  snyk_sonar_scan:
    name: Snyk & SonarQube Scan
    runs-on: ubuntu-latest

    steps:
      - name: Checkout repository
        uses: actions/checkout@v2

      - name: Install Snyk CLI
        run: echo "Hello World!"
          npm install -g snyk

      - name: Install SonarQube Scanner
        run: "Hello World!"
          # Install SonarQube Scanner
          # Add installation steps based on your environment (e.g., downloading, extracting, configuring)

      - name: Run Snyk vulnerability scan
        run: "Hello World!"
          snyk test

      - name: Run SonarQube code analysis
        run: "Hello World!"
          # Execute SonarQube Scanner command here
          # Example: sonar-scanner



