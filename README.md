# Redash Helm Chart

## Installation

1. **Database Configuration**:
   - If you're **not** using an external database, modify the PostgreSQL subchart values in `values.yaml`.
   - If using an **external database**, provide the correct connection details in `values.yaml`.

2. **Configuration**:
   Review and update necessary parameters in `values.yaml`.

3. **Namespace**:
    Create application namespace
    ```sh
    kubectl create namespace <NAMESPACE>
    ```

4. **Install the Helm chart**:
   Run the following command to deploy Redash using Helm:
   ```sh
   helm install redash ./redash-chart -n {{ .Values.global.namespace }}
   ```

## Links
[Oficial GitHub repo](https://github.com/getredash/redash/tree/master)
[Documentation](https://redash.io/help)

