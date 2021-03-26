#To execute locally

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


#To execute remotely
- log in to https://portal.azure.com/ 
- select "azure databricks"
- select existing "resource group" (you should see at least 1)
- press 'launch workspace in the bottom'. you should see 'databricks user interface'

Within databricks User Interface
- click 'create cluster' (import spark-config.json)
- Wait until cluster is created
- Create notebook, select created cluster
- copy content of "main.py" excluding line where cluster is stated manually

