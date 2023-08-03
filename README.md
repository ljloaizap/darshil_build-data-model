# Build data model and database
 
Learning by doing with **Darshil Parmar** and his series of _data modeling_ in [Complete a project with me! - Building Data Model and Database | #LearnByDoing (Part ⅓)](https://www.youtube.com/watch?v=2xyoz0T47Bs&list=PLBJe2dFI4sgukOW6O0B-OVyX9c6fQKJ2N&index=1&ab_channel=DarshilParmar
) video 


## Postgres dabatase
Run a container with messup intentions to learn data modeling
```bash
docker run -d --name postgres_messup --env-file .env -p 5432:5432 postgres
```

Connect to the db using `psql` tool
```bash
psql -h localhost -d postgres -U postgres -W
```

DDL: run the following script 
```sql
CREATE TABLE student (
    id SERIAL PRIMARY KEY,
    name varchar(100) NOT NULL,
    age INT NOT NULL,
    gender varchar(20) NOT NULL,
    subject varchar(50),
    marks INT
)
```

## Jupyter
From [my pandas](https://github.com/ljloaizap/pandas) repo, Jupyter section, just replaced:
```sh
pipenv run python -m ipykernel install --user --name=coding_with_darshil
```
