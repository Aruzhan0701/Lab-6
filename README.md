name: Lab-6 Workflow

on:
  push:          
    branches:
      - main    
jobs:
  say_hello:
    runs-on: ubuntu-latest

    steps:
      - name: Репозиторийді көшіру
        uses: actions/checkout@v4

      - name: Hello хабарын шығару
        run: echo "Hello from Аружан 👋"

      - name: Жүйе туралы ақпарат шығару
        run: uname -a
