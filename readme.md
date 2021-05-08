# Lambda Function with python using serverless

## Steps:

 ### 1.
 ``` serverless create --template aws-python3 ```

 ### 2. update handler.py
 ``` import numpy  ```

 ### 3. install virtual python env If not exist 
 ```  sudo apt install python3-virtualenv ```

 ### 4. Run virtual env
 ``` virtualenv pvenv --python=python3 ```

 ### 5. installing a package using pip
 ```  pip install numpy ```

 ### 6. adding package to requirements.txt file 
 ```  pip freeze > requirements.txt ```

 ### 7. creating package json file to add serverless plugin
 ``` npm init -y ```

 ### 8. Adding plugin

 ``` npm install --save serverless-python-requirements ```

 ### 9. updating serverless.yml
 ``` 
plugins:
  - serverless-python-requirements 
  
```

### 10. Serverless deploy
``` serverless deploy ```

