name: CI de Locos por la Crema

on:
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - name: Instalación de dependencias
        run: echo "Instalando dependencias del proyecto..."
      - name: Verificación de archivos
        run: ls -R
