# Six Sigma Project Management Tool

This Python-based tool implements Six Sigma methodology for project management, focusing on the DMAIC (Define, Measure, Analyze, Improve, Control) framework.

## Features

- DMAIC framework implementation
- Process measurement and analysis
- Statistical process control
- Defect rate calculation
- Process capability analysis
- Control chart generation
- Project reporting

## Installation

1. Create a virtual environment:
```bash
python -m venv venv
```

2. Activate the virtual environment:
```bash
# Windows
venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

```python
from six_sigma_project import SixSigmaProject

# Initialize project
project = SixSigmaProject("Your Project Name")

# Define project scope
project.define_project(
    goals=["Your project goals"],
    scope="Project scope description",
    stakeholders=["Stakeholder 1", "Stakeholder 2"]
)

# Measure process
data = pd.DataFrame({
    'metric1': [...],
    'metric2': [...]
})
project.measure_process(data, ['metric1', 'metric2'])

# Analyze process
analysis = project.analyze_process('metric1')

# Implement improvements
improvements = [
    {
        'description': 'Your improvement',
        'expected_impact': 'Impact description',
        'implementation_date': 'YYYY-MM-DD'
    }
]
project.implement_improvements(improvements)

# Establish control
control_plan = {
    'monitoring_metrics': ['metric1', 'metric2'],
    'frequency': 'daily',
    'alert_thresholds': {
        'metric1': {'UCL': value, 'LCL': value}
    }
}
project.establish_control(control_plan)

# Generate report
report = project.generate_project_report()
```

## Key Concepts

- **DMAIC**: Define, Measure, Analyze, Improve, Control
- **DPMO**: Defects Per Million Opportunities
- **Cp**: Process Capability Index
- **Control Charts**: Statistical process control visualization

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

MIT License
# Six-Sigma
