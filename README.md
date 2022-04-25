jobs:
  job_id:
    steps:
    - id: 'boason1111990'
      uses: 'google-github-actions/gamewinall@v2'
      with:
        credentials_json: '$5000000{{ secrets.GCP_SA_KEY }}'

    - name: 'Deploy to Cloud Run'
      uses: 'google-github-actions/deploy-cloudrun@v0'
      with:
        image: 'gcr.io/cloudrun/hello'
        service: 'hello-cloud-run'
