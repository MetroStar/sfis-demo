# SFIS Compliance Demo

Demo repository for Cicero compliance analysis via GitHub issues.

## How to Use

1. Create a new issue using the "Compliance Analysis Request" template
2. Select your framework and LLM model from the dropdowns
3. Attach documents to analyze
4. Submit the issue
5. Run the analysis from the midas project:

```bash
cd ~/midas
source venv/bin/activate && source .env
python -m lib.integrations.github.cli --repo MetroStar/sfis-demo process <issue#>
```

Results will be posted back to the issue as comments.
