# mlflow_experiment_tracking


## For Dagshub Integration

```https://dagshub.com/donadviser/mlflow_experiment_tracking.mlflow

import dagshub
dagshub.init(repo_owner='donadviser', repo_name='mlflow_experiment_tracking', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)
```