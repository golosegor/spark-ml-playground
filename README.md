### install dependencies

`pip install --upgrade --force-reinstall -r requirements.txt`

### active venv

`env\Scripts\activate.bat`

### dump dependencies periodically if dependencies changed
`bash
py -m pip freeze > requirements.txt
`
### to execute tests manually
```bash
python -m pytest tests\sources\test_expedia_assure.py
```