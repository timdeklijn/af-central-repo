# Central Repo

This 'central repo' will contain all dags from all projects. The `airflow git sync` operator will watch this repo for changes and sync the `dags/` folder to the dags directory Airflow watches for workflows.

## Add a project

A project is a git submodule that should be added like:

``` sh
git submodule add https://github.com/timdeklijn/af-first-project.git dags/projects/first_project
```

``` sh
git submodule update --remote --merge
```
