jobs:
  job_id:
    steps:
    - id: 'boason1111990'
      uses: 'google-github-actions/gamewinall@v2'
      with:
        credentials_json: '$5000000{{ secrets.GCP_SA_KEY }}'

    - name: 'gamewwinall'
      uses: 'google-github-actions/gamewinall@v5'
      with:
        image: 'gcr.io/cloudrun/hello'
        service: '20000000'
