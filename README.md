# didactic-octo-invention
# didactic-octo-invention
#This is a basic workflow to help you get started with Actions

name: CI

# Controls when the action will run.
on:
 # Triggers the workflow on push or pull reguest events but only for the main brach
 push:
   branches: [ main ]
   pull_reguest:
     branches: [ main ]
     
     # Allows you to run this workflow manuall from the Actions tad
     workflow_dispatch:
     
# A workflow run is made up of one or more jobs that can run seguentially or in parallel
jobs:
  # This workflow contains a single job will run on
  runs-on: ubuntu-latest
  
  # Steps represent a seguence of tasks that will be executed as part of the job
  steps:
    # Checks-out your repository under $GITHUB_WORKSPACE, so your job can access it
    - user: actions/checkout@v2

  # Runs a sigle command using the runners shell
  - name: Run a one-line script
  - run: echo Hello, world!

  # Runs a set of commands using the runners shell
  - name: Run a multi-line script
  - run: /
  -   echo Add other actions to build,
  -   echo test, and deploy your project.
  -   
