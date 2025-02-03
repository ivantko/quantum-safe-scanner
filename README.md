# quantum-safe-scanner

## Project Overview
A proof-of-concept Post-Quantum Cryptography (PQC) analysis tool that helps organizations assess their cryptographic readiness for the quantum computing era. This tool provides agentless network analysis and actionable recommendations based on NIST PQC standards.

## Features
- Agentless network traffic analysis
- Cryptographic algorithm detection
- PQC readiness assessment
- Risk scoring and recommendations
- Comprehensive reporting

## Repository Structure
```
quantum-safe-scanner/
├── .github/
│   ├── workflows/         # GitHub Actions workflows
│   └── ISSUE_TEMPLATE/    # Issue templates
├── docs/                  # Documentation
│   ├── architecture/      # Architecture diagrams and docs
│   ├── setup/            # Setup guides
│   └── api/              # API documentation
├── notebooks/            # Jupyter notebooks for analysis and demos
│   ├── prototypes/       # Analysis prototypes
│   └── demos/            # Stakeholder demonstrations
├── src/                  # Source code
│   ├── analyzer/         # Core analysis engine
│   ├── capture/          # Network capture module
│   ├── crypto/           # Cryptographic analysis
│   ├── reporting/        # Report generation
│   └── utils/            # Utility functions
├── tests/                # Test suite
│   ├── unit/
│   └── integration/
├── terraform/            # Infrastructure as Code
│   ├── modules/
│   └── environments/
├── .gitignore
├── LICENSE
├── README.md
├── requirements.txt
└── setup.py
```

## Getting Started

### Prerequisites
- Python 3.8+
- AWS Account
- Git
- VS Code or PyCharm
- Docker Desktop

### Development Setup
1. Clone the repository
```bash
git clone https://github.com/yourusername/quantum-safe-scanner.git
cd quantum-safe-scanner
```

2. Create and activate virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies
```bash
pip install -r requirements.txt
```

4. Configure AWS credentials
```bash
aws configure
```

## Project Board Structure

### GitHub Projects Columns
1. **Backlog**
   - Future features and improvements
   - Unrefined issues

2. **To Do**
   - Well-defined tasks
   - Ready for development

3. **In Progress**
   - Currently being worked on
   - Assigned to team members

4. **Review**
   - Code review
   - Testing
   - Documentation review

5. **Done**
   - Completed tasks
   - Merged to main branch

### Labels
- `feature`: New functionality
- `bug`: Something isn't working
- `documentation`: Documentation improvements
- `security`: Security-related changes
- `enhancement`: Improvements to existing features
- `infrastructure`: AWS/infrastructure changes
- `testing`: Testing-related tasks
- `pqc`: Post-quantum cryptography specific items

## Development Workflow
1. Create a new branch for each feature/fix
```bash
git checkout -b feature/descriptive-name
```

2. Make changes and commit with meaningful messages
```bash
git add .
git commit -m "feat: add crypto algorithm detection"
```

3. Push changes and create pull request
```bash
git push origin feature/descriptive-name
```

4. Ensure tests pass and address review comments
5. Merge after approval

## Security Considerations
- No sensitive credentials in repository
- AWS credentials managed via environment variables
- Regular dependency updates
- Security scanning enabled
- Code signing enforced
