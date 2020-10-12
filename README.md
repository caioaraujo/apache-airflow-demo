# apache-airflow-demo
A demonstration of [Apache Airflow] pipeline.


[Apache Airflow]: https://airflow.apache.org/

## Run

- Install all dependencies listed in `requirements.txt`;
- initialize the database: `airflow initdb`;
- start the web server in default port: `airflow webserver -p 8080`
- start the scheduler: `airflow scheduler`

Visit localhost:8080 in the browser and enable the example dag in the home page.

## Testing

In order to test the dag_demo, copy the python script in `src` folder to default DAGs folder (`~/airflow/dags` by default).
Then, task a desirable task. Ie: `airflow test dag_demo print_date_demo 2015-06-01`